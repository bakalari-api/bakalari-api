# Modul suplovani
Suplování ve specifikovaném týdnu

Název modulu v URL: `suplovani` Příklad: `https://www.example.com/login.aspx?hx=token&pm=suplovani`
## XML
### Příklad
```xml
<?xml version="1.0" encoding="utf-8"?>
<results>
  <suplovani>
    <den>
      <oznaceni>Po 4.12.</oznaceni>
      <seznam>
        <supl>
          <text>1. hod - změna místnosti (VT1) (TED, U22)</text>
        </supl>
        <supl>
          <text>2. hod - změna místnosti (VT1) (TED, U22)</text>
        </supl>
      </seznam>
    </den>
    <den>
      <oznaceni>Út 5.12.</oznaceni>
      <seznam>
        <supl>
          <text>1. hod - odstraněná hodina: MAT, U31</text>
        </supl>
        <supl>
          <text>3. hod - přesun z 5.12., 6. hod (TED, U21i)</text>
        </supl>
        <supl>
          <text>6. hod - přesun z 5.12., 1. hod (MAT, U12)</text>
        </supl>
        <supl>
          <text>8. hod - výměna z 5.12., 9. hod (CJL, U23i)</text>
        </supl>
        <supl>
          <text>9. hod - výměna z 5.12., 8. hod (ZAE, U22)</text>
        </supl>
      </seznam>
    </den>
    <den>
      <oznaceni>Čt 7.12.</oznaceni>
      <seznam>
        <supl>
          <text>1. hod - přesun z 8.12., 2. hod (CJL, U22)</text>
        </supl>
        <supl>
          <text>6. hod - přesun z 7.12., 1. hod (FYZ, U12)</text>
        </supl>
      </seznam>
    </den>
    <den>
      <oznaceni>Pá 8.12.</oznaceni>
      <seznam>
        <supl>
          <text>1. hod - přesun z 8.12., 6. hod (CHK, U23i)</text>
        </supl>
        <supl>
          <text>2. hod - přesun z 7.12., 1. hod (CJL, U01i)</text>
        </supl>
        <supl>
          <text>3. hod - přidáno do rozvrhu (FYZ, U12)</text>
        </supl>
        <supl>
          <text>4. hod - přesun z 8.12., 5. hod (DEJ, U22)</text>
        </supl>
        <supl>
          <text>5. hod - odstraněná hodina: DEJ, U12</text>
        </supl>
        <supl>
          <text>6. hod - odstraněná hodina: CHK, U01i</text>
        </supl>
      </seznam>
    </den>
  </suplovani>
  <result>01</result>
</results>
```
