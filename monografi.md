Här testar jag att lägga in ett scenario/testfall och anpassa det till hjälptext.

## Skapa ny – Tryckt monografi

Exempel: Under cover, ISBN 9789188107213, Voyager BibID 19775078

### Adminmetadata
* Skapad av/Organisation/Namn (040 ‡a)
- förval: den sigel som skapat posten. Ska inte gå att redigera.
Testdata: BOKR

* Uppgraderad eller importerad av/Organisation/Namn (040 ‡d)
Testdata: S

* Bibliografi/Bibliotek/Sigel (042 ‡9 NB)
Testdata: NB

* Identifikator/Systemnummer/Värde
Testdata: (BOKR)9789188107213 (finns i förhandspost)
(Bokinfos systemnummer som följer med vid postimport, ska inte ändras)

* Katalogiseringsspråk (040 ‡b)
- länkning till entitet
Testdata: svenska (swe)

* Katalogiseringsregler (040 ‡e)
- länkning till entiteter + skapa lokal entitet. RDA finns inte som länkbar entitet.
Förval: länkning till entitet: marc/isbd + lokalt skapad entitet med Kod: rda (eller kan vi skapa en länkbar entitet för rda?)
Testdata: marc/Isbd (länkad entitet)
+ Kod: rda

* Beskrivningsnivå (000/05)
- länkning till entiteter
Testdata:  CIP-post, ändra till nationalbibliografisk/fullständig nivå

### Instans
* Utgivningssätt
- val från lista
Testdata: Monografisk resurs

* Har titel/Titel/Huvudtitel (245 ‡a)
Testdata: Under cover (finns i förhandspost)
Har titel/Titel/Huvudtitel/Övrig titelinformation (245 ‡b)
Testdata: livet som underrättelseagent åt MI5

* Upphovsuppgift
Testdata: Tom Marcus ; översättning: Svante Skoglund

* Identifikator/Typ
Testdata: ISBN
Identifikator/Typ/Värde (020 ‡a)
Testdata: 9789188107213
Identifikator/Bestämning (020 ‡q)
Testdata: inbunden

* Upplageuppgift
Testdata: Första upplagan

* Utgivning
- plats/Benämning (264 -/1 ‡a)
Testdata: [Göteborg]
- agent/Benämning (264 -/1 ‡b)
Testdata: NoNa
- datum (264 -/1 ‡c)
Testdata: 2017
Typ av utgivningsdatum/utgivningsstatus (008/06)
- länkning till entitet
Testdata: s (= ett årtal)

* Tillverkning
- plats/Benämning (264 -/3 ‡a)
Testdata: Falun
- agent/Benämning (264 -/3 ‡b)
Testdata: Scandbook

* Kronologisk täckning (008/11-17)
Testdata: 2017____
(jfr datum …)

* Utgivningsland (008/15-17)
- länkning till entitet
Testdata: Sverige (sw)

* Medietyp (337 ‡b)
- länkning till entitet
Testdata:  n (= unmediated)

* Bärartyp (338 ‡b)
- länkning till entitet
Testdata:  nc (= volume)

* Form för katalogiserat objekt (008/23)
- länkning till entitet
Testdata: - (= ingen av följande)

* Omfång/Benämning
Testdata: 319 sidor

* Mått/Benämning
Testdata: 24 cm

### Verk
* Instans av Verk/Text

* Har titel/Titel/Huvudtitel (240 1-/0 ‡a)
Testdata:  Soldier spy

* Medverkan och funktion/Primär medverkan/Agent/Person (100 1/- ‡a)
- lokal entitet
Medverkan och funktion/Primär medverkan/Agent/Person/Familjenamn
Testdata: Marcus
Medverkan och funktion/Primär medverkan/Agent/Person/Förnamn
Testdata: Tom
-Medverkan och funktion/Medverkan/Agent/Funktion (100 ‡4)
- länkning till entitet
Testdata: relator/author (= författare)

* Medverkan och funktion/Medverkan/Agent/Person (700 1/- ‡a)
- länkad entitet
Testdata: Skoglund, Svante, 1960- (i förhandspost: Skoglund, Svante)
-Medverkan och funktion/Medverkan/Agent/Funktion (700 ‡4)
- länkning till entitet
Testdata: relator/trl (= översättare)

* Klassifikation/DDK-klassifikation/Kod (082 0/4 ‡a)
Testdata: 327.12092
Klassifikation/DDK-klassifikation/Kod/Klassifikationsupplaga (082 ‡2)
Testdata: 23/swe

* Klassifikation/Kod (084 0/4 ‡a)
Testdata: Sei-e
Klassifikation/Termlista/Termlista (084 ‡2)
Testdata: kssb
Klassifikation/Termlista/Termlista/Version (084 ‡2)
Testdata: 8
Klassifikation/Termlista/Termlista/Samma sak som (084 ‡2)
- länkad entitet
Testdata: term/kssb/8

* Ämne/Agent/Person (600 1/- ‡a)
- lokal entitet
Ämne/Agent/Person/Familjenamn
Testdata: Marcus
Ämne/Agent/Person/Förnamn
Testdata: Tom

Ämne/Agent/Jurisdiktion/Är del av/Jurisdiktion/Namn (610 1/4 ‡a)
- lokal entitet
Testdata: Storbritannien
Ämne/Agent/Jurisdiktion/Namn på underordnad enhet (610 ‡b)
Testdata: MI5

- länkning till entitet - sao-term (650 -7- ‡a, ‡2 sao)
Testdata: Säkerhetspolitik
- länkning till entitet - sao-term (650 -7- ‡a, ‡2 sao)
Testdata: Spionage
- länkning till entitet - sao-term (650 -7- ‡a, ‡2 sao)
Testdata: Terrorismbekämpning
- länkning till entiteter - geografiskt ämnesord (651 -/4 ‡a)
Testdata: Storbritannien

* Genre/form
- länkning till entiteter – saogf-termer (655 ‡a, ‡2 saogf)
Testdata: Självbiografier
- länkning till entitet – litterär genre (008/33)
Testdata: 0 ( = marc/NotFictionNotFurtherSpecified = Ej skönlitterärt verk)
- länkning till entitet – biografiskt material (008/34)
Testdata: a (= autobiography = självbiografi)

* Språk (008/35-37) (+ även i 041 ‡a, om relationen Översättning av finns)
- länkning till entiteter
Testdata: svenska (swe)
* Översättning av/Verk/Språk (041 ‡h)
- länkning till entitet
Testdata: engelska (eng)

* Innehållstyp (336 ‡b)
- länkning till entiteter
Testdata: text (txt)
