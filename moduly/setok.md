# SetOK

Tento modul nastaví potvrzení o přečtení zprávy na přečteno.

GET `https://www.example.com/login.aspx?pm=setok&hx=token&pmd=id`

`id` je ID zprávy, které lze získat například z modulu `prijate`.

## Odpověď
```xml
<?xml version="1.0" encoding="utf-8"?>
<results>
    <result>01</result>
</results>
```
