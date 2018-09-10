# Vypočítaní tokenu
## Získání soli, kódu a typu
Nejprve je potřeba získat určité komponenty pro vypočítání tokenu. Tyto komponenty získáme ze základní adresy popsané [v úvodu](https://github.com/JosefKuchar/bakalari-api/wiki) (např. `https://www.example.com/login.aspx`) a parametrem `gethx` s přihlašovacím (uživatelským) jménem: `https://www.example.com/login.aspx?gethx=JanNovak`. Vrátí se nám XML podobné tomuto:
```xml
<results>
    <res>01</res>
    <typ>R</typ>
    <ikod>GR10N</ikod>
    <salt>KWKG</salt>
    <pheslo/>
</results>
```
Zajímá nás jen: typ, ikod a salt

### Pozor!
Pokud jméno neexistuje vrátí se toto XML
```xml
<results>
    <res>02</res>
</results>
```

## Vypočítání hashe hesla
Heslo je zahashováno pomocí SHA-512 ve formátu base64. Osoleno je následovně: `salt + ikod + typ + heslo`.

Příklad: Heslo je "tajneheslo" => `SHA512(KWKGGR10NRtajneheslo)` => `v+X97lAKBbTUNOMtN1EcZho+qLJh97vlIyr8T+PvqLsLDLLTeqwc45EsIuMwas7ZOo14dE/yu1G8fycZYXL6yQ==`

## Vypočítání tokenu
Token je string zahashovaný pomocí SHA-512 v upraveném formátu base64, který je vysvětlen později. String před hashováním vypadá následovně: `*login* + jméno uživatele + *pwd* + zahashovaného hesla + *sgn*ANDR + data ve formátu YYYYMMDD`. Tento string normálně zahashujeme funkcí SHA-512 ve formátu base64, ve kterém ale nahradíme některé znaky:
```
\ => _
/ => _
+ => -
```

Příklad: `SHA512(*login*JanNovak*pwd*v+X97lAKBbTUNOMtN1EcZho+qLJh97vlIyr8T+PvqLsLDLLTeqwc45EsIuMwas7ZOo14dE/yu1G8fycZYXL6yQ==*sgn*ANDR20171209)` => `niGnyKbTc0xyChLYuMquVqIiqB/ZzaW0W5OQ6izXoKjHiXnYSpBc9qKJhprK54ZnbZb4fnZbqkwe7RhLRE/xZg==` => `niGnyKbTc0xyChLYuMquVqIiqB_ZzaW0W5OQ6izXoKjHiXnYSpBc9qKJhprK54ZnbZb4fnZbqkwe7RhLRE_xZg==`
