# Modul priloha
Příloha

Název modulu v URL: `priloha`

Pro získání přílohy je potřeba poslat ID požadovaného souboru v parametru `fileId`.

Příklad: `https://www.example.com/login.aspx?hx=token&pm=priloha&fileId=idPrilohy`

ID lze získat z modulu `ukoly`. Je potřeba ID přílohy, ne úkolu!

Pokud je v ID přílohy mezera, je potřeba ji nahradit řetězcem `%20`.  
Pozor, existují i ID jako `X   123ABC` – mezi X a 1 jsou tři mezery, ale např. Firefox vám XML obsahující toto ID zobrazí pouze s jednou mezerou (a GitHub to tak renderuje taky a nevím jak se tomu vyhnout)
