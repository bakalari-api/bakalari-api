# Modul komsend
Odeslání zpráv přes školní systém.

Název modulu v URL: `komsend`. Příklad: `https://www.example.com/login.aspx?hx=token&pm=komsend`

## Vstup

Je nutné poslat POST request. V body post requestu je nutné odeslat tato pole (jako formát form data).

| Key  | Value |
| ------------- | ------------- |
| ktext  | Ahoj, toto je testovací zpráva.  |
| knadpis  |   |
| kprochar  | U  |
| kpro | UKBNV |
| kmno | |
| kkdy | R |
| kre | |

Hodnotu klíče `kprochar` lze získat z [komenslisty](https://github.com/bakalari-api/bakalari-api/blob/master/moduly/komenslisty.md) (skupina, např. učitel), `kpro` je ze stejného zdroje, jedná se o konkrétní osobu.

Hodnota klíče `kkdy` značí, jestli je vyžadováno potvrzení přečtení. `P` - ano, `R` - ne.

## Výstup

Nepodařilo se získat kladnou odpověď serveru, pokud se vám ji podaří získat, tak [nám napište na GitHub](https://github.com/bakalari-api/bakalari-api/issues).

Příklad chybové odpovědi:
```
<?xml version="1.0" encoding="utf-8"?>
<error>
  <code>105</code>
  <message>interni chyba: Odeslání e-mailu se nezdařilo.</message>
</error>
```

Pozor, tato chybová odpověď nastane i v případě, kdy se zpráva bez problému odešle.
