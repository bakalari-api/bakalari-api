# KomDEL

Tento modul vymaže zprávu. Pokud už některý z příjemců zprávy zprávu četl, pošle mu zprávu o vymazání předchozí zprávy.

GET `https://www.example.com/login.aspx?pm=komdel&hx=token&pmd=id`

Kde `id` je ID mazané zprávy.

## Odpověď

V případě úspěchu:
```xml
<?xml version="1.0" encoding="utf-8"?>
<results>
    <result>01</result>
</results>
```

V případě chyby:

```xml
<?xml version="1.0" encoding="utf-8"?>
<error>
    <code>23</code>
    <message>chyba komens: zpravu muze smazat jen jeji odesilatel.</message>
    <result>01</result>
</error>
```
