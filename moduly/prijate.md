# Modul prijate
Přijaté zprávy.
Text zprávy je uveden v tagu `<text>`, formátován jako HTML pomocí `CDATA`. Príklad: `<text><![CDATA[Lorem<br />ipsum]]></text>`

Název modulu v URL: `prijate` Příklad: `https://www.example.com/login.aspx?hx=token&pm=prijate`
## XML
### Příklad
```xml
<?xml version="1.0" encoding="utf-8"?>
<results>
  <zpravy>
    <zprava>
      <id>UQBPTAAAEP</id>
      <text><![CDATA[Lorem ipsum]]></text>
      <nadpis/>
      <cas>1809111430</cas>
      <odt>U</odt>
      <od>Lorem ipusm</od>
      <odid>UQBPT</odid>
      <files>0</files>
      <attachments/>
      <read>ano</read>
      <ok>ne</ok>
      <druh>OBECNA</druh>
      <mustok>0</mustok>
      <answer>1</answer>
    </zprava>
    <zprava>
      <id>UZBN7AAAWG</id>
      <text><![CDATA[Lorem ipsum]]></text>
      <nadpis/>
      <cas>1809040819</cas>
      <odt>S</odt>
      <od>ředitelství</od>
      <odid>UZBN7</odid>
      <files>0</files>
      <attachments/>
      <read>ano</read>
      <ok>ne</ok>
      <druh>AKTUAL</druh>
      <mustok>0</mustok>
      <answer>1</answer>
    </zprava>
    <zprava>
  </zpravy>
  <result>01</result>
</results>

```
