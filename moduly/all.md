# Modul all
Kombinace modulů.
Server vrací XML v tomto pořadí:
- `?pm=znamky`
- `?pm=ukoly`
- `?pm=akce`
- `?pm=suplovani`
- `?pm=absence`
- `?pm=predmety`
- `?pm=pololetni`
- `?pm=predvidac`
- `?pm=rozvrh&pmd=perm`
- `?pm=rozvrh`
- `?pm=rozvrh&pmd=` + datum následujícího pondělí ve formátu YYYYMMDD

Název modulu v URL: `all` Příklad: `https://www.example.com/login.aspx?hx=token&pm=all`
## XML
### Příklad
```xml
<?xml version="1.0" encoding="utf-8"?>
<results>
  <xmlznamky>
    <!--Modul znamky-->
  </xmlznamky>
  <xmlukoly>
    <!--Modul ukoly-->
  </xmlukoly>
  <xmlakce>
    <!--Modul akce-->
  </xmlakce>
  <xmlsuplovani>
    <!--Modul suplovani-->
  </xmlsuplovani>
  <xmlabsence>
    <!--Modul absence-->
  </xmlabsence>
  <xmlpredmety>
    <!--Modul predmety-->
  </xmlpredmety>
  <xmlpololetni>
    <!--Modul pololetni-->
  </xmlpololetni>
  <xmlpredvidac>
    <!--Modul predvidac-->
  </xmlpredvidac>
  <xmlrozvrhperm>
    <!--Modul rozvrhprem-->
  </xmlrozvrhperm>
  <xmlrozvrhakt>
    <!--Modul rozvrhakt-->
  </xmlrozvrhakt>
  <xmlrozvrhnext>
    <!--Modul rozvrhnext-->
  </xmlrozvrhnext>
  <result>01</result>
</results>

```
