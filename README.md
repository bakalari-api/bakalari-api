# Bakaláři API
Dokumentace mobilního API bakalářů

| ⚠️ Bakaláři nyní používají [API v3 (dokumentace zde)](https://github.com/bakalari-api/bakalari-api-v3). Tato dokumentace se týká API v1. ⚠️ |
| --- |

# URL
Vše se odehrává na adrese institutu (školy). Pro zjednodušení budu používat doménu www.example.com. Veškeré API dotazy směřují na `/login.aspx` a to i v případě, že adresa používá nové webové rozhraní next (např. `https://www.example.com/login.aspx`)

# Dotazy
Každý dotaz (vyjma získání tokenu) se skládá z [tokenu](vypocitani_tokenu.md) (`hx`) a názvu modulu (`pm`), případně dalších parametrů jako například data. Příklad: `https://www.example.com/login.aspx?hx=m_1dM0sdoUC3bKRkMdiyjc9IaOkOPyNvpq66zuwIu2eHUtYvkLwrUtHHPR6iNe1KOtA2HgSZtuoBWdido79VjQ==&pm=rozvrh`. Vrací XML, které je popsáno u jednotlivých modulů.

# Notifikace
V rámci aplikace Bakalářů fungují i [notifikace](moduly/notifikace.md).

# Programy postavené na tomto API
* co si na zítra přidat a co z tašky vyndat podle Bakalářů: https://github.com/kokolem/bakalari-next-day
* Bakalarium - neoficiální klient pro Android https://github.com/kokolem/Bakalarium
* Python knihovna: https://github.com/vakabus/pybakalib
* Dart knihovna: https://github.com/soptikha2/bakalari ([pub](https://pub.dartlang.org/packages/bakalari))
* Bakalab – neoficiální klient aplikace Bakaláři: [www.bakalab.org](https://www.bakalab.org)
* Průměr Známek - aplikace pro výpočet váženého průměru s možností předvídání známek (funkční offline): [Průměr Známek na Google Play](https://play.google.com/store/apps/details?id=cz.fely.weightedaverage)
* Lepší Rozvrh - rychlejší klient pro rozvrh (funguje i offline). [Google Play](https://play.google.com/store/apps/details?id=cz.vitskalicky.lepsirozvrh&utm_source=bakalari-api), [GitHub](https://github.com/vitSkalicky/lepsi-rozvrh/)
* Bakaláři klient - Klient Bakaláři pro Windows: https://github.com/Nkaskaj/BakalariClient
* Online token generator - jednoduchý generátor tokenů pro API 1 i API 3 https://ondrovywebovky.cz/token/

Některé další programy a nástroje pracující s tímto API najdete na https://github.com/bakalari-api.

# Moduly
* [absence](moduly/absence.md)
* [akce](moduly/akce.md)
* [all](moduly/all.md)
* [interfaces](moduly/interfaces.md)
* [komdel](moduly/komdel.md)
* [komenslisty](moduly/komenslisty.md)
* [komsend](moduly/komsend.md)
* [login](moduly/login.md)
* [nastenka](moduly/nastenka.md)
* [odeslane](moduly/odeslane.md)
* [pololetni](moduly/pololetni.md)
* [predmety](moduly/predmety.md)
* [predvidac](moduly/predvidac.md)
* [prijate](moduly/prijate.md)
* [priloha](moduly/priloha.md)
* [rozvrh](moduly/rozvrh.md)
* [ucitelrozvrh](moduly/ucitelrozvrh.md)
* [setok](moduly/setok.md)
* [setread](moduly/setread.md)
* [suplovani](moduly/suplovani.md)
* [ukoly](moduly/ukoly.md)
* [vyuka](moduly/vyuka.md)
* [wlogin](moduly/wlogin.md)
* [znamky](moduly/znamky.md)
* classification
* classificationMarks
* home
* rozvrhakt
* rozvrhnext
* rozvrhperm
* timeline
* tkday
* tkedit
* tksave
* tksaveabsent
* ucitelakce
* ucitelall
* ucitelpredmety
* ucitelrozvrhakt
* ucitelrozvrhnext
* ucitelrozvrhperm
* ucitelsuplovani
