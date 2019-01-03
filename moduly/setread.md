#Modul setread

Slouží k nastavení zprávy (ať už soukromé nebo zprávy na nástěnce) jako přečtené.

GET `https://www.example.com/login.aspx?pm=setread&hx=token&pmd=id`

Token slouží k přihlášení uživatele. Id (posílané v querystringu `pmd`) je ID zprávy, která je nově přečtená - něco jako `URRMWDAABC`

## Odpověď
```
<?xml version="1.0" encoding="utf-8"?>
<results />
```
