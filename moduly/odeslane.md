# Odeslané

Tento modul zobrazí odeslané zprávy.

GET `https://www.example.com/loginpaspx?pm=odeslane&hx=token`

## Odpověď

```
<?xml version="1.0" encoding="utf-8"?>
<results>
  <zpravy>
    <zprava>
      <id>GM02EBBBCX</id>
      <text>
        <![CDATA[<strong>HTML</strong> pozor, tohle je opravdu HTML - dávejte při psaní vaší webové aplikace pozor na <script>alert('XSS');</alert> a podobná zvířátka]]>
      </text>
      <nadpis></nadpis>
      <cas>1901032330</cas>
      <odt>X</odt>
      <od>3.A, Josef Novák</od>
      <odid>GM34E</odid>
      <files>0</files>
      <attachments />
      <read>ano</read>
      <ok>ne</ok>
      <druh>OBECNA</druh>
      <mustok>1</mustok>
      <answer>0</answer>
    </zprava>
    <zprava>
      <id>GM02BBBCW</id>
      <text>
        <![CDATA[nějaké podivné HTML]]>
      </text>
      <nadpis></nadpis>
      <cas>1901021808</cas>
      <odt>X</odt>
      <od>3.A, Franta Novák</od>
      <odid>GM33E</odid>
      <files>0</files>
      <attachments />
      <read>ano</read>
      <ok>ne</ok>
      <druh>OBECNA</druh>
      <mustok>0</mustok>
      <answer>0</answer>
    </zprava>
  </zpravy>
</results>
```
