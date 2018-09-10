# Modul wlogin

Slouží k přihlášení do starší verze webové aplikace. Tento modul je specifický tím, že ho nepoužívá mobilní aplikace, ale přímo nové webové rozhraní Next.

Jedná se o odkaz „Původní aplikace“ v levém postranním menu Nextu. Díky tomu, že obsahuje vypočítaný hash uživatele, je užitečný při rychlých experimentech (hash není nutné počítat, pouze se zkopíruje.

Název modulu v URL: `wlogin` Příklad: `https://www.example.com/login.aspx?hx=token&pm=wlogin`

## Využití

U automatického přihlášení. Uživateli se zobrazí stránka, na které je neviditelný iframe s adresou odpovídající `https://www.example.com/login.aspx?hx=token&pm=wlogin`. Po načtení tento iframe spustí onload, který uživatele přesměruje (vyžaduje JavaScript).

### Poznámka:

K automatickému přihlášení je možné využít i ostatní moduly. Tento však dosahuje zdaleka nejrychlejšího načtení.
