# Nástěnka

GET `https://www.example.com/login.aspx?pm=nastenka&hx=token`

## Odpověď
```xml
<?xml version="1.0" encoding="utf-8"?>
<results>
  <zpravy>
    <zprava>
      <id>URRMWBCDCC</id>
      <text>
        <![CDATA[<strong>POZOR</strong> Toto je text zprávy. Stejně jako u osobních zpráv, i tady zacházíme s neenkódovaným HTML. Budeme proto tedy <span style="color: red">dávat pozor</span>, aby se někdo nerozhodl poslat něco ničemného. <script>alert('XSS');</script>]]>
      </text>
      <nadpis>Dávejte si pozor na HTML</nadpis>
      <cas>1812171132</cas>
      <odt>U</odt>
      <od>Mgr. Jméno Učitele</od>
      <odid>URKDW</odid>
      <files>2</files>
      <attachments>
        <attachment>
          <id>URYMBBBAAC</id>
          <name>xss-poc.pdf</name>
          <type>application/pdf</type>
        </attachment>
        <attachment>
          <id>URYMBBBAAD</id>
          <name>csrf=poc.pdf</name>
          <type>application/pdf</type>
        </attachment>
      </attachments>
      <read>ne</read>
      <ok>ne</ok>
      <druh>NASSKO</druh>
      <mustok>0</mustok>
      <answer>1</answer>
    </zprava>
    <!--
    <zprava>
    ...
    </zprava>
    -->
  </zpravy>


</results>
```
