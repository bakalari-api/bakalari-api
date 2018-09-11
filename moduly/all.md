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
    <results>
      <predmety>
        <predmet>
          <nazev>český jazyk a literatura</nazev>
          <zkratka>ČEJ</zkratka>
          <prumer>1</prumer>
          <numprumer>1</numprumer>
          <prepocet></prepocet>
          <bodytoznm></bodytoznm>
          <ctvrt></ctvrt>
          <pozn></pozn>
          <globpozn></globpozn>
          <znamky>
            <znamka>
              <pred>ČEJ</pred>
              <maxb>0</maxb>
              <znamka>1</znamka>
              <zn>1</zn>
              <bd></bd>
              <datum>180911</datum>
              <udeleno>1809111438</udeleno>
              <vaha>10</vaha>
              <caption>Lorem</caption>
              <poznamka>Lorem ipsum</poznamka>
              <typ>A</typ>
              <ozn>známka váhy 10 z 10</ozn>
            </znamka>
          </znamky>
        </predmet>
        <predmet>
          <nazev>zeměpis</nazev>
          <zkratka>ZEM</zkratka>
          <prumer>2</prumer>
          <numprumer>2</numprumer>
          <prepocet></prepocet>
          <bodytoznm></bodytoznm>
          <ctvrt></ctvrt>
          <pozn></pozn>
          <globpozn></globpozn>
          <znamky>
            <znamka>
              <pred>ZEM</pred>
              <maxb>0</maxb>
              <znamka>2</znamka>
              <zn>2</zn>
              <bd></bd>
              <datum>180911</datum>
              <udeleno>1809110815</udeleno>
              <vaha>6</vaha>
              <caption>T1</caption>
              <poznamka>Lorem ipsum</poznamka>
              <typ>E</typ>
              <ozn>známka váhy 6 z 10</ozn>
            </znamka>
          </znamky>
        </predmet>
      </predmety>
    </results>
  </xmlznamky>
  <xmlukoly>
    <results>
      <ukoly>
        <ukol>
          <predmet>český jazyk a literatura</predmet>
          <zkratka>ČEJ</zkratka>
          <zadano>1809100000</zadano>
          <nakdy>1809170000</nakdy>
          <popis>Lorem ipsum</popis>
          <status>aktivni</status>
          <typ>20</typ>
          <id>SWSMSJKHKO</id>
          <attachments />
        </ukol>
        <ukol>
          <predmet>mediální výchova</predmet>
          <zkratka>MeVv</zkratka>
          <zadano>1809070000</zadano>
          <nakdy>1809210000</nakdy>
          <popis>Lorem ipsum</popis>
          <status>aktivni</status>
          <typ>20</typ>
          <id>SW15SJHIEQ</id>
          <attachments />
        </ukol>
      </ukoly>
    </results>
  </xmlukoly>
  <xmlakce>
    <results>
      <akceall>
        <akce>
          <nazev>Lorem ipsum</nazev>
          <datum>20180912</datum>
          <cas>10:55 - 12:35</cas>
          <popis></popis>
          <zobrazit>1</zobrazit>
          <proucitele>Nm</proucitele>
          <protridy>IIIP</protridy>
          <promistnosti></promistnosti>
        </akce>
        <akce>
          <nazev>Lorem ipsum</nazev>
          <datum>20190318</datum>
          <cas>10:00 - 11:40</cas>
          <popis></popis>
          <zobrazit>1</zobrazit>
          <proucitele>Lg, Šá, To</proucitele>
          <protridy>IIIP, IVP</protridy>
          <promistnosti></promistnosti>
        </akce>
      </akceall>
    </results>
  </xmlakce>
  <xmlsuplovani>
    <results>
      <suplovani>
        <den>
          <oznaceni>Út 11.9.</oznaceni>
          <seznam>
            <supl>
              <text>Lorem ipsum</text>
            </supl>
          </seznam>
        </den>
        <den>
          <oznaceni>St 12.9.</oznaceni>
          <seznam>
            <supl>
              <text>Lorem ipsum</text>
            </supl>
          </seznam>
        </den>
      </suplovani>
    </results>
  </xmlsuplovani>
  <xmlabsence>
    <results>
      <absence>
        <hranice>0,2</hranice>
        <seznam>
          <abs>
            <datum>20180906</datum>
            <den>Čt</den>
            <A>5</A>
            <AOk>0</AOk>
            <AMiss>0</AMiss>
            <ALate>0</ALate>
            <ASoon>0</ASoon>
            <ASchool>0</ASchool>
          </abs>
        </seznam>
        <zameskanost>
          <nadpis>Zameškanost 1.9. - 31.1</nadpis>
          <predmet>
            <nazev>třídnická hodina</nazev>
            <oduceno>1</oduceno>
            <absbase>0</absbase>
            <absschool>0</absschool>
            <abssoon>0</abssoon>
            <abslate>0</abslate>
          </predmet>
          <predmet>
            <nazev>český jazyk a literatura</nazev>
            <oduceno>82</oduceno>
            <absbase>1</absbase>
            <absschool>0</absschool>
            <abssoon>0</abssoon>
            <abslate>0</abslate>
          </predmet>
          <predmet>
            <nazev>anglický jazyk</nazev>
            <oduceno>61</oduceno>
            <absbase>0</absbase>
            <absschool>0</absschool>
            <abssoon>0</abssoon>
            <abslate>0</abslate>
          </predmet>
          <predmet>
            <nazev>německý jazyk</nazev>
            <oduceno>40</oduceno>
            <absbase>0</absbase>
            <absschool>0</absschool>
            <abssoon>0</abssoon>
            <abslate>0</abslate>
          </predmet>
          <predmet>
            <nazev>matematika</nazev>
            <oduceno>81</oduceno>
            <absbase>0</absbase>
            <absschool>0</absschool>
            <abssoon>0</abssoon>
            <abslate>0</abslate>
          </predmet>
          <predmet>
            <nazev>občanská výchova</nazev>
            <oduceno>21</oduceno>
            <absbase>0</absbase>
            <absschool>0</absschool>
            <abssoon>0</abssoon>
            <abslate>0</abslate>
          </predmet>
          <predmet>
            <nazev>dějepis</nazev>
            <oduceno>41</oduceno>
            <absbase>0</absbase>
            <absschool>0</absschool>
            <abssoon>0</abssoon>
            <abslate>0</abslate>
          </predmet>
          <predmet>
            <nazev>fyzika</nazev>
            <oduceno>40</oduceno>
            <absbase>0</absbase>
            <absschool>0</absschool>
            <abssoon>0</abssoon>
            <abslate>0</abslate>
          </predmet>
          <predmet>
            <nazev>chemie</nazev>
            <oduceno>63</oduceno>
            <absbase>1</absbase>
            <absschool>0</absschool>
            <abssoon>0</abssoon>
            <abslate>0</abslate>
          </predmet>
          <predmet>
            <nazev>biologie</nazev>
            <oduceno>62</oduceno>
            <absbase>1</absbase>
            <absschool>0</absschool>
            <abssoon>0</abssoon>
            <abslate>0</abslate>
          </predmet>
          <predmet>
            <nazev>zeměpis</nazev>
            <oduceno>21</oduceno>
            <absbase>1</absbase>
            <absschool>0</absschool>
            <abssoon>0</abssoon>
            <abslate>0</abslate>
          </predmet>
          <predmet>
            <nazev>výtvarná výchova</nazev>
            <oduceno>20</oduceno>
            <absbase>0</absbase>
            <absschool>0</absschool>
            <abssoon>0</abssoon>
            <abslate>0</abslate>
          </predmet>
          <predmet>
            <nazev>hudební výchova</nazev>
            <oduceno>20</oduceno>
            <absbase>0</absbase>
            <absschool>0</absschool>
            <abssoon>0</abssoon>
            <abslate>0</abslate>
          </predmet>
          <predmet>
            <nazev>tělesná výchova</nazev>
            <oduceno>42</oduceno>
            <absbase>1</absbase>
            <absschool>0</absschool>
            <abssoon>0</abssoon>
            <abslate>0</abslate>
          </predmet>
          <predmet>
            <nazev>mediální výchova</nazev>
            <oduceno>22</oduceno>
            <absbase>0</absbase>
            <absschool>0</absschool>
            <abssoon>0</abssoon>
            <abslate>0</abslate>
          </predmet>
          <predmet>
            <nazev>finanční matematika</nazev>
            <oduceno>21</oduceno>
            <absbase>0</absbase>
            <absschool>0</absschool>
            <abssoon>0</abssoon>
            <abslate>0</abslate>
          </predmet>
        </zameskanost>
      </absence>
    </results>
  </xmlabsence>
  <xmlpredmety>
    <results>
      <predmety>
        <predmet>
          <nazev>český jazyk a literatura</nazev>
          <zkratka>ČEJ</zkratka>
          <kod_pred> 2</kod_pred>
          <ucitel>Lorem ipsum</ucitel>
          <zkratkauc>Ne</zkratkauc>
        </predmet>
        <predmet>
          <nazev>anglický jazyk</nazev>
          <zkratka>ANJ</zkratka>
          <kod_pred>0W</kod_pred>
          <ucitel>Lorem ipsum</ucitel>
          <zkratkauc>Če</zkratkauc>
        </predmet>
        <predmet>
          <nazev>německý jazyk</nazev>
          <zkratka>NEJ</zkratka>
          <kod_pred>0Y</kod_pred>
          <ucitel>Lorem ipsum</ucitel>
          <zkratkauc>Rn</zkratkauc>
        </predmet>
        <predmet>
          <nazev>matematika</nazev>
          <zkratka>MAT</zkratka>
          <kod_pred>10</kod_pred>
          <ucitel>Lorem ipsum</ucitel>
          <zkratkauc>Wo</zkratkauc>
        </predmet>
        <predmet>
          <nazev>občanská výchova</nazev>
          <zkratka>OBV</zkratka>
          <kod_pred>SR</kod_pred>
          <ucitel>Lorem ipsum</ucitel>
          <zkratkauc>Fi</zkratkauc>
        </predmet>
        <predmet>
          <nazev>dějepis</nazev>
          <zkratka>DĚJ</zkratka>
          <kod_pred> 8</kod_pred>
          <ucitel>Lorem ipsum</ucitel>
          <zkratkauc>Šp</zkratkauc>
        </predmet>
        <predmet>
          <nazev>fyzika</nazev>
          <zkratka>FYZ</zkratka>
          <kod_pred>11</kod_pred>
          <ucitel>Lorem ipsum</ucitel>
          <zkratkauc>Dn</zkratkauc>
        </predmet>
        <predmet>
          <nazev>chemie</nazev>
          <zkratka>CHE</zkratka>
          <kod_pred>12</kod_pred>
          <ucitel>Lorem ipsum</ucitel>
          <zkratkauc>Nm</zkratkauc>
        </predmet>
        <predmet>
          <nazev>biologie</nazev>
          <zkratka>BIO</zkratka>
          <kod_pred>13</kod_pred>
          <ucitel>Lorem ipsum</ucitel>
          <zkratkauc>Nm</zkratkauc>
        </predmet>
        <predmet>
          <nazev>zeměpis</nazev>
          <zkratka>ZEM</zkratka>
          <kod_pred>0I</kod_pred>
          <ucitel>Lorem ipsum</ucitel>
          <zkratkauc>Sk</zkratkauc>
        </predmet>
        <predmet>
          <nazev>výtvarná výchova</nazev>
          <zkratka>VYV</zkratka>
          <kod_pred>56</kod_pred>
          <ucitel>Lorem ipsum</ucitel>
          <zkratkauc>Pz</zkratkauc>
        </predmet>
        <predmet>
          <nazev>hudební výchova</nazev>
          <zkratka>HUV</zkratka>
          <kod_pred>57</kod_pred>
          <ucitel>Lorem ipsum</ucitel>
          <zkratkauc>To</zkratkauc>
        </predmet>
        <predmet>
          <nazev>tělesná výchova</nazev>
          <zkratka>TEV</zkratka>
          <kod_pred>0O</kod_pred>
          <ucitel>Lorem ipsum</ucitel>
          <zkratkauc>Šs</zkratkauc>
        </predmet>
        <predmet>
          <nazev>mediální výchova</nazev>
          <zkratka>MeVv</zkratka>
          <kod_pred>2A</kod_pred>
          <ucitel>Lorem ipsum</ucitel>
          <zkratkauc>Pz</zkratkauc>
        </predmet>
        <predmet>
          <nazev>finanční matematika</nazev>
          <zkratka>FIM</zkratka>
          <kod_pred>1X</kod_pred>
          <ucitel>Lorem ipsum</ucitel>
          <zkratkauc>Hi</zkratkauc>
        </predmet>
      </predmety>
    </results>
  </xmlpredmety>
  <xmlpololetni>
    <results>
      <tabulka>
        <pololeti>
          <polo>
            <sloupec>1</sloupec>
            <rok>2016</rok>
            <rocnik>1</rocnik>
            <rocnikslovy>první</rocnikslovy>
            <pololeti>1.</pololeti>
            <opak>N</opak>
          </polo>
          <polo>
            <sloupec>2</sloupec>
            <rok>2016</rok>
            <rocnik>1</rocnik>
            <rocnikslovy>první</rocnikslovy>
            <pololeti>2.</pololeti>
            <opak>N</opak>
          </polo>
          <polo>
            <sloupec>3</sloupec>
            <rok>2017</rok>
            <rocnik>2</rocnik>
            <rocnikslovy>druhý</rocnikslovy>
            <pololeti>1.</pololeti>
            <opak>N</opak>
          </polo>
          <polo>
            <sloupec>4</sloupec>
            <rok>2017</rok>
            <rocnik>2</rocnik>
            <rocnikslovy>druhý</rocnikslovy>
            <pololeti>2.</pololeti>
            <opak>N</opak>
          </polo>
          <polo>
            <sloupec>5</sloupec>
            <rok>2018</rok>
            <rocnik>3</rocnik>
            <rocnikslovy>třetí</rocnikslovy>
            <pololeti>1.</pololeti>
            <opak>N</opak>
          </polo>
          <polo>
            <sloupec>6</sloupec>
            <rok>2018</rok>
            <rocnik>3</rocnik>
            <rocnikslovy>třetí</rocnikslovy>
            <pololeti>2.</pololeti>
            <opak>N</opak>
          </polo>
        </pololeti>
        <predmety>
          <predmet>
            <nazev>chování</nazev>
            <znamky>
              <znamka>
                <sloupec>1</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>2</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>3</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>4</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>5</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>6</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
            </znamky>
          </predmet>
          <predmet>
            <nazev>český jazyk a literatura</nazev>
            <znamky>
              <znamka>
                <sloupec>1</sloupec>
                <value>2</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>2</sloupec>
                <value>2</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>3</sloupec>
                <value>2</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>4</sloupec>
                <value>2</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>5</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>6</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
            </znamky>
          </predmet>
          <predmet>
            <nazev>anglický jazyk</nazev>
            <znamky>
              <znamka>
                <sloupec>1</sloupec>
                <value>2</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>2</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>3</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>4</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>5</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>6</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
            </znamky>
          </predmet>
          <predmet>
            <nazev>německý jazyk</nazev>
            <znamky>
              <znamka>
                <sloupec>1</sloupec>
                <value>-</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>2</sloupec>
                <value>-</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>3</sloupec>
                <value>2</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>4</sloupec>
                <value>3</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>5</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>6</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
            </znamky>
          </predmet>
          <predmet>
            <nazev>matematika</nazev>
            <znamky>
              <znamka>
                <sloupec>1</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>2</sloupec>
                <value>2</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>3</sloupec>
                <value>2</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>4</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>5</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>6</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
            </znamky>
          </predmet>
          <predmet>
            <nazev>informatika a výpočetní technika</nazev>
            <znamky>
              <znamka>
                <sloupec>1</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>2</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>3</sloupec>
                <value>-</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>4</sloupec>
                <value>-</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>5</sloupec>
                <value>-</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>6</sloupec>
                <value>-</value>
                <opak>N</opak>
              </znamka>
            </znamky>
          </predmet>
          <predmet>
            <nazev>občanská výchova</nazev>
            <znamky>
              <znamka>
                <sloupec>1</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>2</sloupec>
                <value>2</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>3</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>4</sloupec>
                <value>2</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>5</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>6</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
            </znamky>
          </predmet>
          <predmet>
            <nazev>dějepis</nazev>
            <znamky>
              <znamka>
                <sloupec>1</sloupec>
                <value>2</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>2</sloupec>
                <value>2</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>3</sloupec>
                <value>4</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>4</sloupec>
                <value>3</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>5</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>6</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
            </znamky>
          </predmet>
          <predmet>
            <nazev>fyzika</nazev>
            <znamky>
              <znamka>
                <sloupec>1</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>2</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>3</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>4</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>5</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>6</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
            </znamky>
          </predmet>
          <predmet>
            <nazev>biologie</nazev>
            <znamky>
              <znamka>
                <sloupec>1</sloupec>
                <value>2</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>2</sloupec>
                <value>3</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>3</sloupec>
                <value>2</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>4</sloupec>
                <value>2</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>5</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>6</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
            </znamky>
          </predmet>
          <predmet>
            <nazev>zeměpis</nazev>
            <znamky>
              <znamka>
                <sloupec>1</sloupec>
                <value>2</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>2</sloupec>
                <value>2</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>3</sloupec>
                <value>2</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>4</sloupec>
                <value>2</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>5</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>6</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
            </znamky>
          </predmet>
          <predmet>
            <nazev>hudební výchova</nazev>
            <znamky>
              <znamka>
                <sloupec>1</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>2</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>3</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>4</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>5</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>6</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
            </znamky>
          </predmet>
          <predmet>
            <nazev>chemie</nazev>
            <znamky>
              <znamka>
                <sloupec>1</sloupec>
                <value>-</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>2</sloupec>
                <value>-</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>3</sloupec>
                <value>-</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>4</sloupec>
                <value>-</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>5</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>6</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
            </znamky>
          </predmet>
          <predmet>
            <nazev>výtvarná výchova</nazev>
            <znamky>
              <znamka>
                <sloupec>1</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>2</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>3</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>4</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>5</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>6</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
            </znamky>
          </predmet>
          <predmet>
            <nazev>tělesná výchova</nazev>
            <znamky>
              <znamka>
                <sloupec>1</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>2</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>3</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>4</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>5</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>6</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
            </znamky>
          </predmet>
          <predmet>
            <nazev>mediální výchova</nazev>
            <znamky>
              <znamka>
                <sloupec>1</sloupec>
                <value>-</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>2</sloupec>
                <value>-</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>3</sloupec>
                <value>-</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>4</sloupec>
                <value>-</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>5</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>6</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
            </znamky>
          </predmet>
          <predmet>
            <nazev>aplikovaná matematika</nazev>
            <znamky>
              <znamka>
                <sloupec>1</sloupec>
                <value>-</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>2</sloupec>
                <value>-</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>3</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>4</sloupec>
                <value>1</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>5</sloupec>
                <value>-</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>6</sloupec>
                <value>-</value>
                <opak>N</opak>
              </znamka>
            </znamky>
          </predmet>
          <predmet>
            <nazev>finanční matematika</nazev>
            <znamky>
              <znamka>
                <sloupec>1</sloupec>
                <value>-</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>2</sloupec>
                <value>-</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>3</sloupec>
                <value>-</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>4</sloupec>
                <value>-</value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>5</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
              <znamka>
                <sloupec>6</sloupec>
                <value></value>
                <opak>N</opak>
              </znamka>
            </znamky>
          </predmet>
        </predmety>
      </tabulka>
      <souhrny>
        <souhrn>
          <rocnik>1</rocnik>
          <rocnikslovy>první</rocnikslovy>
          <pololeti>1.</pololeti>
          <prumer>1,42</prumer>
          <zameskane>8</zameskane>
          <neomluvene>0</neomluvene>
          <hodnoceni>prospěl s vyznamenáním</hodnoceni>
          <vysvedceni>20170131</vysvedceni>
          <opak>N</opak>
        </souhrn>
        <souhrn>
          <rocnik>1</rocnik>
          <rocnikslovy>první</rocnikslovy>
          <pololeti>2.</pololeti>
          <prumer>1,58</prumer>
          <zameskane>2</zameskane>
          <neomluvene>0</neomluvene>
          <hodnoceni>prospěl</hodnoceni>
          <vysvedceni>20170630</vysvedceni>
          <opak>N</opak>
        </souhrn>
        <souhrn>
          <rocnik>2</rocnik>
          <rocnikslovy>druhý</rocnikslovy>
          <pololeti>1.</pololeti>
          <prumer>1,62</prumer>
          <zameskane>4</zameskane>
          <neomluvene>0</neomluvene>
          <hodnoceni>prospěl</hodnoceni>
          <vysvedceni>20180131</vysvedceni>
          <opak>N</opak>
        </souhrn>
        <souhrn>
          <rocnik>2</rocnik>
          <rocnikslovy>druhý</rocnikslovy>
          <pololeti>2.</pololeti>
          <prumer>1,62</prumer>
          <zameskane>29</zameskane>
          <neomluvene>0</neomluvene>
          <hodnoceni>prospěl</hodnoceni>
          <vysvedceni>20180629</vysvedceni>
          <opak>N</opak>
        </souhrn>
        <souhrn>
          <rocnik>3</rocnik>
          <rocnikslovy>třetí</rocnikslovy>
          <pololeti>1.</pololeti>
          <prumer></prumer>
          <zameskane></zameskane>
          <neomluvene></neomluvene>
          <hodnoceni></hodnoceni>
          <vysvedceni></vysvedceni>
          <opak>N</opak>
        </souhrn>
        <souhrn>
          <rocnik>3</rocnik>
          <rocnikslovy>třetí</rocnikslovy>
          <pololeti>2.</pololeti>
          <prumer></prumer>
          <zameskane></zameskane>
          <neomluvene></neomluvene>
          <hodnoceni></hodnoceni>
          <vysvedceni></vysvedceni>
          <opak>N</opak>
        </souhrn>
      </souhrny>
      <vychovna>
        <vychovne>
          <rok>2017/18</rok>
          <pololeti>2</pololeti>
          <nazev>pochvala ředitele školy</nazev>
          <datum>20180627</datum>
          <text>za reprezentaci školy na Robosoutěži</text>
        </vychovne>
        <vychovne>
          <rok>2016/17</rok>
          <pololeti>2</pololeti>
          <nazev>pochvala třídního učitele</nazev>
          <datum>20170630</datum>
          <text>za reprezentaci GJP v Robosoutěži a ve ScratchCupu 2017 v ČR kategorii 6. tříd</text>
        </vychovne>
      </vychovna>
    </results>
  </xmlpololetni>
  <xmlpredvidac>
    <results>
      <typypru>
        <typ>
          <zkratka>A</zkratka>
          <nazev>známka váhy 10 z 10</nazev>
          <vaha>10</vaha>
        </typ>
        <typ>
          <zkratka>B</zkratka>
          <nazev>známka váhy 9 z 10</nazev>
          <vaha>9</vaha>
        </typ>
        <typ>
          <zkratka>C</zkratka>
          <nazev>známka váhy 8 z 10</nazev>
          <vaha>8</vaha>
        </typ>
        <typ>
          <zkratka>D</zkratka>
          <nazev>známka váhy 7 z 10</nazev>
          <vaha>7</vaha>
        </typ>
        <typ>
          <zkratka>E</zkratka>
          <nazev>známka váhy 6 z 10</nazev>
          <vaha>6</vaha>
        </typ>
        <typ>
          <zkratka>F</zkratka>
          <nazev>známka váhy 5 z 10</nazev>
          <vaha>5</vaha>
        </typ>
        <typ>
          <zkratka>G</zkratka>
          <nazev>známka váhy 4 z 10</nazev>
          <vaha>4</vaha>
        </typ>
        <typ>
          <zkratka>H</zkratka>
          <nazev>známka váhy 3 z 10</nazev>
          <vaha>3</vaha>
        </typ>
        <typ>
          <zkratka>I</zkratka>
          <nazev>známka váhy 2 z 10</nazev>
          <vaha>2</vaha>
        </typ>
        <typ>
          <zkratka>J</zkratka>
          <nazev>známka váhy 1 z 10</nazev>
          <vaha>1</vaha>
        </typ>
      </typypru>
    </results>
  </xmlpredvidac>
  <xmlrozvrhperm>
    <results>
      <rozvrh>
        <typ>perm</typ>
        <kodcyklu>0</kodcyklu>
        <zkratkacyklu>S</zkratkacyklu>
        <nazevcyklu>sudý týden</nazevcyklu>
        <hodiny>
          <pocet>9</pocet>
          <hod>
            <caption>1</caption>
            <begintime>8:00</begintime>
            <endtime>8:45</endtime>
          </hod>
          <hod>
            <caption>2</caption>
            <begintime>8:55</begintime>
            <endtime>9:40</endtime>
          </hod>
          <hod>
            <caption>3</caption>
            <begintime>10:00</begintime>
            <endtime>10:45</endtime>
          </hod>
          <hod>
            <caption>4</caption>
            <begintime>10:55</begintime>
            <endtime>11:40</endtime>
          </hod>
          <hod>
            <caption>5</caption>
            <begintime>11:50</begintime>
            <endtime>12:35</endtime>
          </hod>
          <hod>
            <caption>6</caption>
            <begintime>12:45</begintime>
            <endtime>13:30</endtime>
          </hod>
          <hod>
            <caption>7</caption>
            <begintime>13:35</begintime>
            <endtime>14:20</endtime>
          </hod>
          <hod>
            <caption>8</caption>
            <begintime>14:25</begintime>
            <endtime>15:10</endtime>
          </hod>
          <hod>
            <caption>9</caption>
            <begintime>15:15</begintime>
            <endtime>16:00</endtime>
          </hod>
        </hodiny>
        <dny>
          <pocet>5</pocet>
          <den>
            <zkratka>Po</zkratka>
            <datum></datum>
            <hodiny>
              <hod>
                <idcode>       0 3SWSMSRUZBNC</idcode>
                <typ>H</typ>
                <zkrpr>OBV</zkrpr>
                <pr>občanská výchova</pr>
                <zkruc>Fi</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>206</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>1</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       0 4SWSM13UI2TE</idcode>
                <typ>H</typ>
                <zkrpr>BIO</zkrpr>
                <pr>biologie</pr>
                <zkruc>Nm</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>431</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>2</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       0 5SWSV0YU  16</idcode>
                <typ>H</typ>
                <zkrpr>NEJ</zkrpr>
                <pr>německý jazyk</pr>
                <zkruc>Rn</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>301</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>sk3</zkrskup>
                <skup>NEJ/Rn</skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>3</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       0 6SWSM 2U  34</idcode>
                <typ>H</typ>
                <zkrpr>ČEJ</zkrpr>
                <pr>český jazyk a literatura</pr>
                <zkruc>Ne</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>206</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>4</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       0 7SWSM12UI2TE</idcode>
                <typ>H</typ>
                <zkrpr>CHE</zkrpr>
                <pr>chemie</pr>
                <zkruc>Nm</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>431</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>5</caption>
                <notice></notice>
              </hod>
              <hod>
                <typ>X</typ>
                <zkratka></zkratka>
              </hod>
              <hod>
                <idcode>       0 9SWSM 8UQBPV</idcode>
                <typ>H</typ>
                <zkrpr>DĚJ</zkrpr>
                <pr>dějepis</pr>
                <zkruc>Šp</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>407</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>7</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       010SWSM56U  15</idcode>
                <typ>H</typ>
                <zkrpr>VYV</zkrpr>
                <pr>výtvarná výchova</pr>
                <zkruc>Pz</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>413</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>8</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       011SWSM11U   5</idcode>
                <typ>H</typ>
                <zkrpr>FYZ</zkrpr>
                <pr>fyzika</pr>
                <zkruc>Dn</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>435</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>9</caption>
                <notice></notice>
              </hod>
            </hodiny>
          </den>
          <den>
            <zkratka>Út</zkratka>
            <datum></datum>
            <hodiny>
              <hod>
                <idcode>       1 3SWSM0IU  33</idcode>
                <typ>H</typ>
                <zkrpr>ZEM</zkrpr>
                <pr>zeměpis</pr>
                <zkruc>Sk</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>353</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>1</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       1 4SWSM 2U  34</idcode>
                <typ>H</typ>
                <zkrpr>ČEJ</zkrpr>
                <pr>český jazyk a literatura</pr>
                <zkruc>Ne</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>206</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>2</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       1 5SWWX0WURBQ0</idcode>
                <typ>H</typ>
                <zkrpr>ANJ</zkrpr>
                <pr>anglický jazyk</pr>
                <zkruc>Če</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>404</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>sk1</zkrskup>
                <skup>ANJ/Če</skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>3</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       1 6SWSM13UI2TE</idcode>
                <typ>H</typ>
                <zkrpr>BIO</zkrpr>
                <pr>biologie</pr>
                <zkruc>Nm</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>359</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>4</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       1 7SWSN0OUMBPF</idcode>
                <typ>H</typ>
                <zkrpr>TEV</zkrpr>
                <pr>tělesná výchova</pr>
                <zkruc>Šs</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>TEL</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>chl</zkrskup>
                <skup>chlapci</skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>5</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       1 8SWSM10USBQ9</idcode>
                <typ>H</typ>
                <zkrpr>MAT</zkrpr>
                <pr>matematika</pr>
                <zkruc>Wo</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>201</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle></cycle>
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
            <zkratka>St</zkratka>
            <datum></datum>
            <hodiny>
              <hod>
                <idcode>       2 3SWSM10USBQ9</idcode>
                <typ>H</typ>
                <zkrpr>MAT</zkrpr>
                <pr>matematika</pr>
                <zkruc>Wo</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>201</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>1</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       2 4SWSM 8UQBPV</idcode>
                <typ>H</typ>
                <zkrpr>DĚJ</zkrpr>
                <pr>dějepis</pr>
                <zkruc>Šp</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>407</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>2</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       2 5SWSM12UI2TE</idcode>
                <typ>H</typ>
                <zkrpr>CHE</zkrpr>
                <pr>chemie</pr>
                <zkruc>Nm</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>431</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>3</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       2 6SWSM57UAMPY</idcode>
                <typ>H</typ>
                <zkrpr>HUV</zkrpr>
                <pr>hudební výchova</pr>
                <zkruc>To</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>121</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>4</caption>
                <notice></notice>
              </hod>
              <hod>
                <typ>X</typ>
                <zkratka></zkratka>
              </hod>
              <hod>
                <idcode>       2 8SWWX0WURBQ0</idcode>
                <typ>H</typ>
                <zkrpr>ANJ</zkrpr>
                <pr>anglický jazyk</pr>
                <zkruc>Če</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>406</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>sk1</zkrskup>
                <skup>ANJ/Če</skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>6</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       2 9SWSV0YU  16</idcode>
                <typ>H</typ>
                <zkrpr>NEJ</zkrpr>
                <pr>německý jazyk</pr>
                <zkruc>Rn</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>301</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>sk3</zkrskup>
                <skup>NEJ/Rn</skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>7</caption>
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
            </hodiny>
          </den>
          <den>
            <zkratka>Čt</zkratka>
            <datum></datum>
            <hodiny>
              <hod>
                <idcode>       3 3SWSM10USBQ9</idcode>
                <typ>H</typ>
                <zkrpr>MAT</zkrpr>
                <pr>matematika</pr>
                <zkruc>Wo</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>206</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>1</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       3 4SWSM13UI2TE</idcode>
                <typ>H</typ>
                <zkrpr>BIO</zkrpr>
                <pr>biologie</pr>
                <zkruc>Nm</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>359</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>2</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       3 5SWSM 2U  34</idcode>
                <typ>H</typ>
                <zkrpr>ČEJ</zkrpr>
                <pr>český jazyk a literatura</pr>
                <zkruc>Ne</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>206</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>3</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       3 6SWSM12UI2TE</idcode>
                <typ>H</typ>
                <zkrpr>CHE</zkrpr>
                <pr>chemie</pr>
                <zkruc>Nm</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>431</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>4</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       3 7SWWO1XU65XX</idcode>
                <typ>H</typ>
                <zkrpr>FIM</zkrpr>
                <pr>finanční matematika</pr>
                <zkruc>Hi</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>201</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>sk5</zkrskup>
                <skup>FiM</skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>5</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       3 8SWSN0OUMBPF</idcode>
                <typ>H</typ>
                <zkrpr>TEV</zkrpr>
                <pr>tělesná výchova</pr>
                <zkruc>Šs</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>HALA</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>chl</zkrskup>
                <skup>chlapci</skup>
                <cycle></cycle>
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
            <zkratka>Pá</zkratka>
            <datum></datum>
            <hodiny>
              <hod>
                <idcode>       4 3SWSM10USBQ9</idcode>
                <typ>H</typ>
                <zkrpr>MAT</zkrpr>
                <pr>matematika</pr>
                <zkruc>Wo</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>201</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>1</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       4 4SWSM 2U  34</idcode>
                <typ>H</typ>
                <zkrpr>ČEJ</zkrpr>
                <pr>český jazyk a literatura</pr>
                <zkruc>Ne</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>206</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>2</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       4 5SWSM11U   5</idcode>
                <typ>H</typ>
                <zkrpr>FYZ</zkrpr>
                <pr>fyzika</pr>
                <zkruc>Dn</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>435</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>3</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       4 6SWWX0WURBQ0</idcode>
                <typ>H</typ>
                <zkrpr>ANJ</zkrpr>
                <pr>anglický jazyk</pr>
                <zkruc>Če</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>423</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>sk1</zkrskup>
                <skup>ANJ/Če</skup>
                <cycle></cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>4</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       4 7SW152AU  15</idcode>
                <typ>H</typ>
                <zkrpr>MeVv</zkrpr>
                <pr>mediální výchova</pr>
                <zkruc>Pz</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>413</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>sk8</zkrskup>
                <skup>MeV</skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>5</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>       4 8SW152AU  15</idcode>
                <typ>H</typ>
                <zkrpr>MeVv</zkrpr>
                <pr>mediální výchova</pr>
                <zkruc>Pz</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>413</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>sk8</zkrskup>
                <skup>MeV</skup>
                <cycle>L</cycle>
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
        </dny>
      </rozvrh>
    </results>
  </xmlrozvrhperm>
  <xmlrozvrhakt>
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
            <begintime>8:00</begintime>
            <endtime>8:45</endtime>
          </hod>
          <hod>
            <caption>2</caption>
            <begintime>8:55</begintime>
            <endtime>9:40</endtime>
          </hod>
          <hod>
            <caption>3</caption>
            <begintime>10:00</begintime>
            <endtime>10:45</endtime>
          </hod>
          <hod>
            <caption>4</caption>
            <begintime>10:55</begintime>
            <endtime>11:40</endtime>
          </hod>
          <hod>
            <caption>5</caption>
            <begintime>11:50</begintime>
            <endtime>12:35</endtime>
          </hod>
          <hod>
            <caption>6</caption>
            <begintime>12:45</begintime>
            <endtime>13:30</endtime>
          </hod>
          <hod>
            <caption>7</caption>
            <begintime>13:35</begintime>
            <endtime>14:20</endtime>
          </hod>
          <hod>
            <caption>8</caption>
            <begintime>14:25</begintime>
            <endtime>15:10</endtime>
          </hod>
          <hod>
            <caption>9</caption>
            <begintime>15:15</begintime>
            <endtime>16:00</endtime>
          </hod>
        </hodiny>
        <dny>
          <pocet>5</pocet>
          <den>
            <zkratka>Po</zkratka>
            <datum>20180910</datum>
            <hodiny>
              <hod>
                <idcode>20180910 3SWSMSRUZBNC</idcode>
                <typ>H</typ>
                <zkrpr>OBV</zkrpr>
                <pr>občanská výchova</pr>
                <zkruc>Fi</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>206</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema>Jsem člověk, ale jaký</tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>S</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>1</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180910 4SWSM13UI2TE</idcode>
                <typ>H</typ>
                <zkrpr>BIO</zkrpr>
                <pr>biologie</pr>
                <zkruc>Nm</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>431</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema>Etologie živočichů</tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>S</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>2</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180910 5SWSV0YU  16</idcode>
                <typ>H</typ>
                <zkrpr>NEJ</zkrpr>
                <pr>německý jazyk</pr>
                <zkruc>Rn</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>301</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema>Rád, raději, nejraději</tema>
                <zkrskup>sk3</zkrskup>
                <skup>NEJ/Rn</skup>
                <cycle>S</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>3</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180910 6SWSM 2U  34</idcode>
                <typ>H</typ>
                <zkrpr>ČEJ</zkrpr>
                <pr>český jazyk a literatura</pr>
                <zkruc>Ne</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>206</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema>Práce s beletrií</tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>S</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>4</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180910 7SWSM12UI2TE</idcode>
                <typ>H</typ>
                <zkrpr>CHE</zkrpr>
                <pr>chemie</pr>
                <zkruc>Nm</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>431</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema>Zjišťování vlastností látek</tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>S</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>5</caption>
                <notice></notice>
              </hod>
              <hod>
                <typ>X</typ>
                <zkratka></zkratka>
              </hod>
              <hod>
                <idcode>20180910 9SWSM 8UQBPV</idcode>
                <typ>H</typ>
                <zkrpr>DĚJ</zkrpr>
                <pr>dějepis</pr>
                <zkruc>Šp</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>407</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>S</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>7</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>2018091010SWSM56U  15</idcode>
                <typ>H</typ>
                <zkrpr>VYV</zkrpr>
                <pr>výtvarná výchova</pr>
                <zkruc>Pz</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>413</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema>Úvod do předmětu; kresba</tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>S</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>8</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>2018091011SWSM11U   5</idcode>
                <typ>H</typ>
                <zkrpr>FYZ</zkrpr>
                <pr>fyzika</pr>
                <zkruc>Dn</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>435</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema>Mechanická práce</tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>S</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>9</caption>
                <notice></notice>
              </hod>
            </hodiny>
          </den>
          <den>
            <zkratka>Út</zkratka>
            <datum>20180911</datum>
            <hodiny>
              <hod>
                <idcode>20180911 3SWSM0IU  33</idcode>
                <typ>H</typ>
                <zkrpr>ZEM</zkrpr>
                <pr>zeměpis</pr>
                <zkruc>Sk</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>353</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema>Evropa - povrch</tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>S</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>1</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180911 4SWSM 2U  34</idcode>
                <typ>H</typ>
                <zkrpr>ČEJ</zkrpr>
                <pr>český jazyk a literatura</pr>
                <zkruc>Ne</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>206</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema>Slovní zásoba</tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>S</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>2</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180911 5SWWX0WURBQ0</idcode>
                <typ>H</typ>
                <zkrpr>ANJ</zkrpr>
                <pr>anglický jazyk</pr>
                <zkruc>Če</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>404</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema>Minulý prběhový - cvičení WB U3A</tema>
                <zkrskup>sk1</zkrskup>
                <skup>ANJ/Če</skup>
                <cycle>S</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>3</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180911 6SWSM13URBQ2</idcode>
                <typ>H</typ>
                <zkrpr>BIO</zkrpr>
                <pr>biologie</pr>
                <zkruc>Šl</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>359</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema>Dronte mauricijský, opakování eukaryotické buňky</tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>S</cycle>
                <uvol></uvol>
                <chng>suplování (Niemcová Romana)</chng>
                <caption>4</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180911 7SWSN0OUMBPF</idcode>
                <typ>H</typ>
                <zkrpr>TEV</zkrpr>
                <pr>tělesná výchova</pr>
                <zkruc>Šs</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>TEL</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>chl</zkrskup>
                <skup>chlapci</skup>
                <cycle>S</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>5</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180911 8SWSM10USBQ9</idcode>
                <typ>H</typ>
                <zkrpr>MAT</zkrpr>
                <pr>matematika</pr>
                <zkruc>Wo</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>201</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema>Číselné výrazy</tema>
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
            <zkratka>St</zkratka>
            <datum>20180912</datum>
            <hodiny>
              <hod>
                <idcode>20180912 3SWSM10USBQ9</idcode>
                <typ>H</typ>
                <zkrpr>MAT</zkrpr>
                <pr>matematika</pr>
                <zkruc>Wo</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>201</zkrmist>
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
                <idcode>20180912 4SWSM 8UQBPV</idcode>
                <typ>H</typ>
                <zkrpr>DĚJ</zkrpr>
                <pr>dějepis</pr>
                <zkruc>Šp</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>407</zkrmist>
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
                <idcode>20180912 5SWSM12UI2TE</idcode>
                <typ>H</typ>
                <zkrpr>CHE</zkrpr>
                <pr>chemie</pr>
                <zkruc>Nm</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>431</zkrmist>
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
                <idcode>20180912 6           </idcode>
                <typ>A</typ>
                <zkratka>j.č.</zkratka>
                <nazev>jiná činnost</nazev>
              </hod>
              <hod>
                <idcode>20180912 7           </idcode>
                <typ>A</typ>
                <zkratka>j.č.</zkratka>
                <nazev>jiná činnost</nazev>
              </hod>
              <hod>
                <idcode>20180912 8SWWX0WURBQ0</idcode>
                <typ>H</typ>
                <zkrpr>ANJ</zkrpr>
                <pr>anglický jazyk</pr>
                <zkruc>Če</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>406</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>sk1</zkrskup>
                <skup>ANJ/Če</skup>
                <cycle>S</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>6</caption>
                <notice></notice>
              </hod>
              <hod>
                <chng>vyjmuto z rozvrhu</chng>
                <idcode>20180912 9SWSV0YU  16</idcode>
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
            <datum>20180913</datum>
            <hodiny>
              <hod>
                <idcode>20180913 3SWSM10USBQ9</idcode>
                <typ>H</typ>
                <zkrpr>MAT</zkrpr>
                <pr>matematika</pr>
                <zkruc>Wo</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>206</zkrmist>
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
                <idcode>20180913 4SWSM13UI2TE</idcode>
                <typ>H</typ>
                <zkrpr>BIO</zkrpr>
                <pr>biologie</pr>
                <zkruc>Nm</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>359</zkrmist>
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
                <idcode>20180913 5SWSM 2U  34</idcode>
                <typ>H</typ>
                <zkrpr>ČEJ</zkrpr>
                <pr>český jazyk a literatura</pr>
                <zkruc>Ne</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>206</zkrmist>
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
                <idcode>20180913 6SWSM12UI2TE</idcode>
                <typ>H</typ>
                <zkrpr>CHE</zkrpr>
                <pr>chemie</pr>
                <zkruc>Nm</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>431</zkrmist>
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
                <idcode>20180913 7SWWO1XU65XX</idcode>
                <typ>H</typ>
                <zkrpr>FIM</zkrpr>
                <pr>finanční matematika</pr>
                <zkruc>Hi</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>201</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>sk5</zkrskup>
                <skup>FiM</skup>
                <cycle>S</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>5</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180913 8SWSN0OUMBPF</idcode>
                <typ>H</typ>
                <zkrpr>TEV</zkrpr>
                <pr>tělesná výchova</pr>
                <zkruc>Šs</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>HALA</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>chl</zkrskup>
                <skup>chlapci</skup>
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
            <zkratka>Pá</zkratka>
            <datum>20180914</datum>
            <hodiny>
              <hod>
                <idcode>20180914 3SWSM10USBQ9</idcode>
                <typ>H</typ>
                <zkrpr>MAT</zkrpr>
                <pr>matematika</pr>
                <zkruc>Wo</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>201</zkrmist>
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
                <idcode>20180914 4SWSM 2U  34</idcode>
                <typ>H</typ>
                <zkrpr>ČEJ</zkrpr>
                <pr>český jazyk a literatura</pr>
                <zkruc>Ne</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>206</zkrmist>
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
                <idcode>20180914 5SWSM11U   5</idcode>
                <typ>H</typ>
                <zkrpr>FYZ</zkrpr>
                <pr>fyzika</pr>
                <zkruc>Dn</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>435</zkrmist>
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
                <idcode>20180914 6SWWX0WURBQ0</idcode>
                <typ>H</typ>
                <zkrpr>ANJ</zkrpr>
                <pr>anglický jazyk</pr>
                <zkruc>Če</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>423</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>sk1</zkrskup>
                <skup>ANJ/Če</skup>
                <cycle>S</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>4</caption>
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
    </results>
  </xmlrozvrhakt>
  <xmlrozvrhnext>
    <results>
      <rozvrh>
        <typ>akt</typ>
        <kodcyklu>1</kodcyklu>
        <zkratkacyklu>L</zkratkacyklu>
        <nazevcyklu>Lichy tyden</nazevcyklu>
        <hodiny>
          <pocet>9</pocet>
          <hod>
            <caption>1</caption>
            <begintime>8:00</begintime>
            <endtime>8:45</endtime>
          </hod>
          <hod>
            <caption>2</caption>
            <begintime>8:55</begintime>
            <endtime>9:40</endtime>
          </hod>
          <hod>
            <caption>3</caption>
            <begintime>10:00</begintime>
            <endtime>10:45</endtime>
          </hod>
          <hod>
            <caption>4</caption>
            <begintime>10:55</begintime>
            <endtime>11:40</endtime>
          </hod>
          <hod>
            <caption>5</caption>
            <begintime>11:50</begintime>
            <endtime>12:35</endtime>
          </hod>
          <hod>
            <caption>6</caption>
            <begintime>12:45</begintime>
            <endtime>13:30</endtime>
          </hod>
          <hod>
            <caption>7</caption>
            <begintime>13:35</begintime>
            <endtime>14:20</endtime>
          </hod>
          <hod>
            <caption>8</caption>
            <begintime>14:25</begintime>
            <endtime>15:10</endtime>
          </hod>
          <hod>
            <caption>9</caption>
            <begintime>15:15</begintime>
            <endtime>16:00</endtime>
          </hod>
        </hodiny>
        <dny>
          <pocet>5</pocet>
          <den>
            <zkratka>Po</zkratka>
            <datum>20180917</datum>
            <hodiny>
              <hod>
                <idcode>20180917 3SWSMSRUZBNC</idcode>
                <typ>H</typ>
                <zkrpr>OBV</zkrpr>
                <pr>občanská výchova</pr>
                <zkruc>Fi</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>206</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>1</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180917 4SWSM13UI2TE</idcode>
                <typ>H</typ>
                <zkrpr>BIO</zkrpr>
                <pr>biologie</pr>
                <zkruc>Nm</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>431</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>2</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180917 5SWSV0YU  16</idcode>
                <typ>H</typ>
                <zkrpr>NEJ</zkrpr>
                <pr>německý jazyk</pr>
                <zkruc>Rn</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>301</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>sk3</zkrskup>
                <skup>NEJ/Rn</skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>3</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180917 6SWSM 2U  34</idcode>
                <typ>H</typ>
                <zkrpr>ČEJ</zkrpr>
                <pr>český jazyk a literatura</pr>
                <zkruc>Ne</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>206</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>4</caption>
                <ukolodevzdat>Přinést knihu, kterou chci představit spolužákům; vybrat vhodné úryvky</ukolodevzdat>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180917 7SWSM12UI2TE</idcode>
                <typ>H</typ>
                <zkrpr>CHE</zkrpr>
                <pr>chemie</pr>
                <zkruc>Nm</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>431</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>5</caption>
                <notice></notice>
              </hod>
              <hod>
                <typ>X</typ>
                <zkratka></zkratka>
              </hod>
              <hod>
                <idcode>20180917 9SWSM 8UQBPV</idcode>
                <typ>H</typ>
                <zkrpr>DĚJ</zkrpr>
                <pr>dějepis</pr>
                <zkruc>Šp</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>407</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>7</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>2018091710SWSM56U  15</idcode>
                <typ>H</typ>
                <zkrpr>VYV</zkrpr>
                <pr>výtvarná výchova</pr>
                <zkruc>Pz</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>413</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>8</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>2018091711SWSM11U   5</idcode>
                <typ>H</typ>
                <zkrpr>FYZ</zkrpr>
                <pr>fyzika</pr>
                <zkruc>Dn</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>435</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>9</caption>
                <notice></notice>
              </hod>
            </hodiny>
          </den>
          <den>
            <zkratka>Út</zkratka>
            <datum>20180918</datum>
            <hodiny>
              <hod>
                <idcode>20180918 3SWSM0IU  33</idcode>
                <typ>H</typ>
                <zkrpr>ZEM</zkrpr>
                <pr>zeměpis</pr>
                <zkruc>Sk</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>353</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>1</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180918 4SWSM 2U  34</idcode>
                <typ>H</typ>
                <zkrpr>ČEJ</zkrpr>
                <pr>český jazyk a literatura</pr>
                <zkruc>Ne</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>206</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>2</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180918 5SWWX0WURBQ0</idcode>
                <typ>H</typ>
                <zkrpr>ANJ</zkrpr>
                <pr>anglický jazyk</pr>
                <zkruc>Če</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>404</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>sk1</zkrskup>
                <skup>ANJ/Če</skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>3</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180918 6SWSM13UI2TE</idcode>
                <typ>H</typ>
                <zkrpr>BIO</zkrpr>
                <pr>biologie</pr>
                <zkruc>Nm</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>359</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>4</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180918 7SWSN0OUMBPF</idcode>
                <typ>H</typ>
                <zkrpr>TEV</zkrpr>
                <pr>tělesná výchova</pr>
                <zkruc>Šs</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>TEL</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>chl</zkrskup>
                <skup>chlapci</skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>5</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180918 8SWSM10USBQ9</idcode>
                <typ>H</typ>
                <zkrpr>MAT</zkrpr>
                <pr>matematika</pr>
                <zkruc>Wo</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>201</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>L</cycle>
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
            <zkratka>St</zkratka>
            <datum>20180919</datum>
            <hodiny>
              <hod>
                <idcode>20180919 3SWSM10USBQ9</idcode>
                <typ>H</typ>
                <zkrpr>MAT</zkrpr>
                <pr>matematika</pr>
                <zkruc>Wo</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>201</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>1</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180919 4SWSM 8UQBPV</idcode>
                <typ>H</typ>
                <zkrpr>DĚJ</zkrpr>
                <pr>dějepis</pr>
                <zkruc>Šp</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>407</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>2</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180919 5SWSM12UI2TE</idcode>
                <typ>H</typ>
                <zkrpr>CHE</zkrpr>
                <pr>chemie</pr>
                <zkruc>Nm</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>431</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>3</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180919 6SWSM57UAMPY</idcode>
                <typ>H</typ>
                <zkrpr>HUV</zkrpr>
                <pr>hudební výchova</pr>
                <zkruc>To</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>121</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>4</caption>
                <notice></notice>
              </hod>
              <hod>
                <typ>X</typ>
                <zkratka></zkratka>
              </hod>
              <hod>
                <idcode>20180919 8SWWX0WURBQ0</idcode>
                <typ>H</typ>
                <zkrpr>ANJ</zkrpr>
                <pr>anglický jazyk</pr>
                <zkruc>Če</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>406</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>sk1</zkrskup>
                <skup>ANJ/Če</skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>6</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180919 9SWSV0YU  16</idcode>
                <typ>H</typ>
                <zkrpr>NEJ</zkrpr>
                <pr>německý jazyk</pr>
                <zkruc>Rn</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>301</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>sk3</zkrskup>
                <skup>NEJ/Rn</skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>7</caption>
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
            </hodiny>
          </den>
          <den>
            <zkratka>Čt</zkratka>
            <datum>20180920</datum>
            <hodiny>
              <hod>
                <idcode>20180920 3SWSM10USBQ9</idcode>
                <typ>H</typ>
                <zkrpr>MAT</zkrpr>
                <pr>matematika</pr>
                <zkruc>Wo</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>206</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>1</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180920 4SWSM13UI2TE</idcode>
                <typ>H</typ>
                <zkrpr>BIO</zkrpr>
                <pr>biologie</pr>
                <zkruc>Nm</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>359</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>2</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180920 5SWSM 2U  34</idcode>
                <typ>H</typ>
                <zkrpr>ČEJ</zkrpr>
                <pr>český jazyk a literatura</pr>
                <zkruc>Ne</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>206</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>3</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180920 6SWSM12UI2TE</idcode>
                <typ>H</typ>
                <zkrpr>CHE</zkrpr>
                <pr>chemie</pr>
                <zkruc>Nm</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>431</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>4</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180920 7SWWO1XU65XX</idcode>
                <typ>H</typ>
                <zkrpr>FIM</zkrpr>
                <pr>finanční matematika</pr>
                <zkruc>Hi</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>201</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>sk5</zkrskup>
                <skup>FiM</skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>5</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180920 8SWSN0OUMBPF</idcode>
                <typ>H</typ>
                <zkrpr>TEV</zkrpr>
                <pr>tělesná výchova</pr>
                <zkruc>Šs</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>HALA</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>chl</zkrskup>
                <skup>chlapci</skup>
                <cycle>L</cycle>
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
            <zkratka>Pá</zkratka>
            <datum>20180921</datum>
            <hodiny>
              <hod>
                <idcode>20180921 3SWSM10USBQ9</idcode>
                <typ>H</typ>
                <zkrpr>MAT</zkrpr>
                <pr>matematika</pr>
                <zkruc>Wo</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>201</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>1</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180921 4SWSM 2U  34</idcode>
                <typ>H</typ>
                <zkrpr>ČEJ</zkrpr>
                <pr>český jazyk a literatura</pr>
                <zkruc>Ne</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>206</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>2</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180921 5SWSM11U   5</idcode>
                <typ>H</typ>
                <zkrpr>FYZ</zkrpr>
                <pr>fyzika</pr>
                <zkruc>Dn</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>435</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup></zkrskup>
                <skup></skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>3</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180921 6SWWX0WURBQ0</idcode>
                <typ>H</typ>
                <zkrpr>ANJ</zkrpr>
                <pr>anglický jazyk</pr>
                <zkruc>Če</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>423</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>sk1</zkrskup>
                <skup>ANJ/Če</skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>4</caption>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180921 7SW152AU  15</idcode>
                <typ>H</typ>
                <zkrpr>MeVv</zkrpr>
                <pr>mediální výchova</pr>
                <zkruc>Pz</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>413</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>sk8</zkrskup>
                <skup>MeV</skup>
                <cycle>L</cycle>
                <uvol></uvol>
                <chng></chng>
                <caption>5</caption>
                <ukolodevzdat>Esej o sobě.</ukolodevzdat>
                <notice></notice>
              </hod>
              <hod>
                <idcode>20180921 8SW152AU  15</idcode>
                <typ>H</typ>
                <zkrpr>MeVv</zkrpr>
                <pr>mediální výchova</pr>
                <zkruc>Pz</zkruc>
                <uc>Lorem ipsum</uc>
                <zkrmist>413</zkrmist>
                <mist></mist>
                <zkrabs></zkrabs>
                <abs></abs>
                <tema></tema>
                <zkrskup>sk8</zkrskup>
                <skup>MeV</skup>
                <cycle>L</cycle>
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
        </dny>
      </rozvrh>
    </results>
  </xmlrozvrhnext>
  <result>01</result>
</results>

```
