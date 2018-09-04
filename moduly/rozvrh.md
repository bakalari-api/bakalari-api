# Modul rozvrh
Rozvrh

Název modulu v URL: `rozvrh` Příklad: `https://www.example.com/login.aspx?hx=token&pm=rozvrh`
## Další parametry
### pmd
Datum které udává týden, je doporučeno předávát jen pondělí.

Formát YYYYMMDD

Příklad: `?pmd=20180305`



Je také možné získat stálý rozvrh pomocí hodnoty `perm`

Příklad: `?pmd=perm`
## XML
### Příklad
```xml
<?xml version="1.0" encoding="utf-8"?>
<results>
  <rozvrh>
    <typ>akt</typ>
    <kodcyklu>0</kodcyklu>
    <zkratkacyklu>S</zkratkacyklu>
    <nazevcyklu>sudý týden</nazevcyklu>
    <hodiny>
      <pocet>9</pocet>
      <hod>
        <caption>1</caption>
        <begintime>7:45</begintime>
        <endtime>8:30</endtime>
      </hod>
      <hod>
        <caption>2</caption>
        <begintime>8:35</begintime>
        <endtime>9:20</endtime>
      </hod>
      <hod>
        <caption>3</caption>
        <begintime>9:25</begintime>
        <endtime>10:10</endtime>
      </hod>
      <hod>
        <caption>4</caption>
        <begintime>10:30</begintime>
        <endtime>11:15</endtime>
      </hod>
      <hod>
        <caption>5</caption>
        <begintime>11:25</begintime>
        <endtime>12:10</endtime>
      </hod>
      <hod>
        <caption>6</caption>
        <begintime>12:20</begintime>
        <endtime>13:05</endtime>
      </hod>
      <hod>
        <caption>7</caption>
        <begintime>13:15</begintime>
        <endtime>14:00</endtime>
      </hod>
      <hod>
        <caption>8</caption>
        <begintime>14:10</begintime>
        <endtime>14:55</endtime>
      </hod>
      <hod>
        <caption>9</caption>
        <begintime>15:00</begintime>
        <endtime>15:45</endtime>
      </hod>
    </hodiny>
    <dny>
      <pocet>5</pocet>
      <den>
        <zkratka>Po</zkratka>
        <datum>20171204</datum>
        <hodiny>
          <hod>
            <idcode>20171204 31GOX86U000L</idcode>
            <typ>H</typ>
            <zkrpr>TED</zkrpr>
            <pr>Technická dokumentace</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>U22</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup>P1</zkrskup>
            <skup>Lo</skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng>změna místnosti (VT1)</chng>
            <caption>1</caption>
            <notice></notice>
          </hod>
          <hod>
            <idcode>20171204 41GOX86U000L</idcode>
            <typ>H</typ>
            <zkrpr>TED</zkrpr>
            <pr>Technická dokumentace</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>U22</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup>P1</zkrskup>
            <skup>Lo</skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng>změna místnosti (VT1)</chng>
            <caption>2</caption>
            <notice></notice>
          </hod>
          <hod>
            <idcode>20171204 51GOX97UL02N</idcode>
            <typ>H</typ>
            <zkrpr>IKT</zkrpr>
            <pr>Informační a komunikační technologie</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>VT3</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup>P1</zkrskup>
            <skup>Lo</skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng></chng>
            <caption>3</caption>
            <notice></notice>
          </hod>
          <hod>
            <idcode>20171204 61GOX97UL02N</idcode>
            <typ>H</typ>
            <zkrpr>IKT</zkrpr>
            <pr>Informační a komunikační technologie</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>VT3</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup>P1</zkrskup>
            <skup>Lo</skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng></chng>
            <caption>4</caption>
            <notice></notice>
          </hod>
          <hod>
            <idcode>20171204 71GOE 8UR031</idcode>
            <typ>H</typ>
            <zkrpr>DEJ</zkrpr>
            <pr>Dějepis</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>U21i</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup></zkrskup>
            <skup></skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng></chng>
            <caption>5</caption>
            <notice></notice>
          </hod>
          <hod>
            <idcode>20171204 81GOE7HU000F</idcode>
            <typ>H</typ>
            <zkrpr>ZAE</zkrpr>
            <pr>Základy elektrotechniky</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>U22</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup></zkrskup>
            <skup></skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng></chng>
            <caption>6</caption>
            <notice></notice>
          </hod>
          <hod>
            <typ>X</typ>
            <zkratka></zkratka>
          </hod>
          <hod>
            <typ>X</typ>
            <zkratka></zkratka>
          </hod>
          <hod>
            <typ>X</typ>
            <zkratka></zkratka>
          </hod>
        </hodiny>
      </den>
      <den>
        <zkratka>Út</zkratka>
        <datum>20171205</datum>
        <hodiny>
          <hod>
            <chng>přesun na 5.12., 6. hod</chng>
            <idcode>20171205 31GOE10U000C</idcode>
            <typ>X</typ>
            <zkratka></zkratka>
          </hod>
          <hod>
            <idcode>20171205 41GOX 4UR033</idcode>
            <typ>H</typ>
            <zkrpr>ANJ</zkrpr>
            <pr>Anglický jazyk</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>JAZ2</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup>P1</zkrskup>
            <skup>Lo</skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng></chng>
            <caption>2</caption>
            <notice></notice>
          </hod>
          <hod>
            <idcode>20171205 51GOE86U000L</idcode>
            <typ>H</typ>
            <zkrpr>TED</zkrpr>
            <pr>Technická dokumentace</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>U21i</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup></zkrskup>
            <skup></skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng>přesun z 5.12., 6. hod</chng>
            <caption>3</caption>
            <notice></notice>
          </hod>
          <hod>
            <idcode>20171205 61GOX 4UR033</idcode>
            <typ>H</typ>
            <zkrpr>ANJ</zkrpr>
            <pr>Anglický jazyk</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>U23i</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup>P1</zkrskup>
            <skup>Lo</skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng></chng>
            <caption>4</caption>
            <notice></notice>
          </hod>
          <hod>
            <idcode>20171205 71GOE11U000C</idcode>
            <typ>H</typ>
            <zkrpr>FYZ</zkrpr>
            <pr>Fyzika</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>U12</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup></zkrskup>
            <skup></skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng></chng>
            <caption>5</caption>
            <notice></notice>
          </hod>
          <hod>
            <idcode>20171205 81GOE10U000C</idcode>
            <typ>H</typ>
            <zkrpr>MAT</zkrpr>
            <pr>Matematika</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>U12</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup></zkrskup>
            <skup></skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng>přesun z 5.12., 1. hod</chng>
            <caption>6</caption>
            <notice></notice>
          </hod>
          <hod>
            <typ>X</typ>
            <zkratka></zkratka>
          </hod>
          <hod>
            <idcode>20171205101GOE 2U001W</idcode>
            <typ>H</typ>
            <zkrpr>CJL</zkrpr>
            <pr>Český jazyk a literatura</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>U23i</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup></zkrskup>
            <skup></skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng>výměna z 5.12., 9. hod</chng>
            <caption>8</caption>
            <notice></notice>
          </hod>
          <hod>
            <idcode>20171205111GOE7HU000F</idcode>
            <typ>H</typ>
            <zkrpr>ZAE</zkrpr>
            <pr>Základy elektrotechniky</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>U22</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup></zkrskup>
            <skup></skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng>výměna z 5.12., 8. hod</chng>
            <caption>9</caption>
            <notice></notice>
          </hod>
        </hodiny>
      </den>
      <den>
        <zkratka>St</zkratka>
        <datum>20171206</datum>
        <hodiny>
          <hod>
            <idcode>20171206 31GOE10U000C</idcode>
            <typ>H</typ>
            <zkrpr>MAT</zkrpr>
            <pr>Matematika</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>U02</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup></zkrskup>
            <skup></skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng></chng>
            <caption>1</caption>
            <notice></notice>
          </hod>
          <hod>
            <idcode>20171206 41GOE17U000D</idcode>
            <typ>H</typ>
            <zkrpr>TEV</zkrpr>
            <pr>Tělesná výchova</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>TEV</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup></zkrskup>
            <skup></skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng></chng>
            <caption>2</caption>
            <notice></notice>
          </hod>
          <hod>
            <idcode>20171206 51GOX 4UR033</idcode>
            <typ>H</typ>
            <zkrpr>ANJ</zkrpr>
            <pr>Anglický jazyk</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>U31</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup>P1</zkrskup>
            <skup>Lo</skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng></chng>
            <caption>3</caption>
            <notice></notice>
          </hod>
          <hod>
            <idcode>20171206 61GOE7HU000F</idcode>
            <typ>H</typ>
            <zkrpr>ZAE</zkrpr>
            <pr>Základy elektrotechniky</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>U22</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup></zkrskup>
            <skup></skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng></chng>
            <caption>4</caption>
            <notice></notice>
          </hod>
          <hod>
            <idcode>20171206 71GOE97UL02N</idcode>
            <typ>H</typ>
            <zkrpr>IKT</zkrpr>
            <pr>Informační a komunikační technologie</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>U33</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup></zkrskup>
            <skup></skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng></chng>
            <caption>5</caption>
            <notice></notice>
          </hod>
          <hod>
            <idcode>20171206 81GOE 2U001W</idcode>
            <typ>H</typ>
            <zkrpr>CJL</zkrpr>
            <pr>Český jazyk a literatura</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>U32</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup></zkrskup>
            <skup></skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng></chng>
            <caption>6</caption>
            <notice></notice>
          </hod>
          <hod>
            <typ>X</typ>
            <zkratka></zkratka>
          </hod>
          <hod>
            <typ>X</typ>
            <zkratka></zkratka>
          </hod>
          <hod>
            <typ>X</typ>
            <zkratka></zkratka>
          </hod>
        </hodiny>
      </den>
      <den>
        <zkratka>Čt</zkratka>
        <datum>20171207</datum>
        <hodiny>
          <hod>
            <idcode>20171207 31GOE 2U001W</idcode>
            <typ>H</typ>
            <zkrpr>CJL</zkrpr>
            <pr>Český jazyk a literatura</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>U22</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup></zkrskup>
            <skup></skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng>přesun z 8.12., 2. hod</chng>
            <caption>1</caption>
            <notice></notice>
          </hod>
          <hod>
            <idcode>20171207 41GOX 4UR033</idcode>
            <typ>H</typ>
            <zkrpr>ANJ</zkrpr>
            <pr>Anglický jazyk</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>U22</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup>P1</zkrskup>
            <skup>Lo</skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng></chng>
            <caption>2</caption>
            <notice></notice>
          </hod>
          <hod>
            <idcode>20171207 51GOE17U000D</idcode>
            <typ>H</typ>
            <zkrpr>TEV</zkrpr>
            <pr>Tělesná výchova</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>TEV</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup></zkrskup>
            <skup></skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng></chng>
            <caption>3</caption>
            <notice></notice>
          </hod>
          <hod>
            <idcode>20171207 61GOE8FU000Q</idcode>
            <typ>H</typ>
            <zkrpr>CHK</zkrpr>
            <pr>Chemie a ekologie</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>U21i</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup></zkrskup>
            <skup></skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng></chng>
            <caption>4</caption>
            <notice></notice>
          </hod>
          <hod>
            <idcode>20171207 71GOE10U000C</idcode>
            <typ>H</typ>
            <zkrpr>MAT</zkrpr>
            <pr>Matematika</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>U22</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup></zkrskup>
            <skup></skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng></chng>
            <caption>5</caption>
            <notice></notice>
          </hod>
          <hod>
            <idcode>20171207 81GOE11U000C</idcode>
            <typ>H</typ>
            <zkrpr>FYZ</zkrpr>
            <pr>Fyzika</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>U12</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup></zkrskup>
            <skup></skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng>přesun z 7.12., 1. hod</chng>
            <caption>6</caption>
            <notice></notice>
          </hod>
          <hod>
            <typ>X</typ>
            <zkratka></zkratka>
          </hod>
          <hod>
            <typ>X</typ>
            <zkratka></zkratka>
          </hod>
          <hod>
            <typ>X</typ>
            <zkratka></zkratka>
          </hod>
        </hodiny>
      </den>
      <den>
        <zkratka>Pá</zkratka>
        <datum>20171208</datum>
        <hodiny>
          <hod>
            <idcode>20171208 31GOE8FU000Q</idcode>
            <typ>H</typ>
            <zkrpr>CHK</zkrpr>
            <pr>Chemie a ekologie</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>U23i</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup></zkrskup>
            <skup></skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng>přesun z 8.12., 6. hod</chng>
            <caption>1</caption>
            <notice></notice>
          </hod>
          <hod>
            <idcode>20171208 41GOE 2U001W</idcode>
            <typ>H</typ>
            <zkrpr>CJL</zkrpr>
            <pr>Český jazyk a literatura</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>U01i</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup></zkrskup>
            <skup></skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng>přesun z 7.12., 1. hod</chng>
            <caption>2</caption>
            <notice></notice>
          </hod>
          <hod>
            <idcode>20171208 51GOE11U001G</idcode>
            <typ>H</typ>
            <zkrpr>FYZ</zkrpr>
            <pr>Fyzika</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>U12</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup></zkrskup>
            <skup></skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng>přidáno do rozvrhu</chng>
            <caption>3</caption>
            <notice></notice>
          </hod>
          <hod>
            <idcode>20171208 61GOE 8UR031</idcode>
            <typ>H</typ>
            <zkrpr>DEJ</zkrpr>
            <pr>Dějepis</pr>
            <zkruc>Lo</zkruc>
            <uc>Lorem Ipsum</uc>
            <zkrmist>U22</zkrmist>
            <mist></mist>
            <zkrabs></zkrabs>
            <abs></abs>
            <tema></tema>
            <zkrskup></zkrskup>
            <skup></skup>
            <cycle>S</cycle>
            <uvol></uvol>
            <chng>přesun z 8.12., 5. hod</chng>
            <caption>4</caption>
            <notice></notice>
          </hod>
          <hod>
            <chng>přesun na 8.12., 4. hod</chng>
            <idcode>20171208 71GOE 8UR031</idcode>
            <typ>X</typ>
            <zkratka></zkratka>
          </hod>
          <hod>
            <chng>přesun na 8.12., 1. hod</chng>
            <idcode>20171208 81GOE8FU000Q</idcode>
            <typ>X</typ>
            <zkratka></zkratka>
          </hod>
          <hod>
            <typ>X</typ>
            <zkratka></zkratka>
          </hod>
          <hod>
            <typ>X</typ>
            <zkratka></zkratka>
          </hod>
          <hod>
            <typ>X</typ>
            <zkratka></zkratka>
          </hod>
        </hodiny>
      </den>
    </dny>
  </rozvrh>
  <result>01</result>
</results>
```