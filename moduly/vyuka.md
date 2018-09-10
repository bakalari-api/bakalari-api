# Modul vyuka

Název modulu v URL: `vyuka` Příklad: `https://www.example.com/login.aspx?hx=token&pm=vyuka`
## Další parametry
### pmd
Kód předmětu, zjistí se v `predmety`, u každého předmětu je `<kod_pred>`. Mezera se nahradí plusem.

Příklad: `?pmd=+2` (pro `<kod_pred> 2</kod_pred>`)

## XML
### Příklad
```xml
<results>
  <vyuka>
    <vyhodina>
      <poradi>2</poradi>
      <datum>20180907</datum>
      <hodina>2</hodina>
      <cislo_hod>3</cislo_hod>
      <tema>Pravopis</tema>
      <poznamka/>
    </vyhodina>
    <vyhodina>
      <poradi>1</poradi>
      <datum>20180906</datum>
      <hodina>3</hodina>
      <cislo_hod>2</cislo_hod>
      <tema>Věty vedlejší</tema>
      <poznamka/>
    </vyhodina>
    <vyhodina>
      <poradi>0</poradi>
      <datum>20180904</datum>
      <hodina>2</hodina>
      <cislo_hod>1</cislo_hod>
      <tema>Úvodní hodina</tema>
      <poznamka/>
    </vyhodina>
  </vyuka>
  <result>01</result>
</results>
```
