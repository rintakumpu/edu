# Tilastotieteen peruskurssi a #

**Henri Pesonen (vastaanotto Ma 14&ndash;15; Pub 455)**
**Luento 1: 3.9.2013**

* **Tilastotieteen peruskurssi a: todennäköisyyslaskenta (2013); 4op**
* Tilastotieteen peruskurssi b: päättelyn perusmenetelmät (2013); 5op
* Tilastotieteen peruskurssi c: tilastollisia malleja (2014); 5op
* Varianssi- ja regressioanalyysi; 5op
* Aikasarjat ja indeksit; 6op

Suositellaan:

* TILM3517 R-kielen alkeet; 2op // TODO: Ilmoittaudu!

* Luennot: 22h; 24.9., 1.10. ja 8.10. luennot salissa Pub 1
* Harjoitukset: 12h; 3 ensimmäistä viikkoa tilastotieteen seminaarihuoneessa (tilastotieteen käytävän päässä; 3 jälkimmäistä viikkoa Pub 409)
* Tentti

Harjoitusajankohdat: // TODO: Ilmoittautuminen 5.9. klo 8!!!

* To 12 &ndash; 14
* To 14 &ndash; 16
* To 16 &ndash; 18
* Pe 8 &ndash; 10
* Pe 10 &ndash; 12

6 harjoituskertaa, 8 harjoitustehtävää per kerta, 40% tehtävistä vaaditaan tenttioikeuteen (so. 20 tehtävää), tehdyullä tehtävillä saa bonuspisteitä 1&ndash;3 (vst. 27 tehtävää&ndash; 41 tehtävää)

Harjoitustehtävät voi palauttaa pätevästä syystä etukäteen (lasketaan tenttioikeuteen, ei bonuspisteisiin)

**Tentit:** Kurssista järjestetään 3 tenttiä, ensimmäinen 23.10. Ilmoittautuminen Nettiopsun kautta. 5 tehtävää, 6 pistettä per tehtävä. Läpipääsyyn vaaditaan 15 pistettä. *2. ja 3. tentin päivät TBA*

**Luentoaikataulu**

1. Housekeeping &amp; peruskäsitteet
2. Laskusääntöjä
3. Otanta
4. Ehdollinen todennäköisyys / tapahtumien riippumattomuus
5. Satunnaismuuttuja ja todennäköisyysjakaume
6. Satunnaismuuttujan funktiot ja tunnuslukuja
7. Satunaismuuttujien yhteisjakauma
8. Ehdollinen todennäköisyysjakauma ja satunnaismuuttujien riippumattomuus
9. TODO: COPY-PASTE from kalvot.

## Tilastotiede ja todennäköisyyslaskenta ##

Tilastotiede on **menetelmätiede**, jossa kuvataan ja selitetään reaalimaailman ilmiöitä havaittavan informaation avulla. Havaittava informaatio sisältää epävarmuutta tai satunnaisuutta.

Todennäköisyyslaskennalla kehitetään matemaattisia malleja satunnaisilmiöille:

1. Jos alkutilan perusteella tiedetään tarkasti lopputulos, ilmiö on **deterministinen** (kausaalinen), eikä ilmiöön liity satunnaisuutta (esim. kemialliset reaktiot).
2. Jos ilmiön alkutilasta huolimatta tapahtuma A voi esiintyä tai olla esiintymättä, niin kyseessä on satunnaisilmiö (ilmiö on **stokastinen**, esim. kolikonheitto, lottoarvonta)

Tehdään päätelmiä objektien joukosta (n) havaitsemalla satunnaisilmiöiden lopputuloksia. Jotta tuloksista voidaan vetää johtopäätöksiä täytyy tietää, mitkä ovat satunnaisilmiön **mahdolliset lopputulokset** == alkeistapaukset! 

Df. **alkeistapaus**, esim. d6-heitto, alkeistapaukset ovat:

&Omega;: { &omega;1 = Silmäluku 1; ..., &omega;6 = Silmäluku 6 }

Otosavaruus eli perusjoukko on kaikkien mahdollisten alkeistapauksien joukko &Omega; 

Otosavaruus voi olla **numeroituva** tai **ylinumeroituva**. Numeroitava, jos jokaiselle alkiolle voidaan määrätä oma luonnollinen luku, esim.
N = {0,1,2,...} t. &Omega; {1,2,3,...,6} &ndash; Ääreelliset joukot numeroituvia (mutta kaikki numeroituvat eivät ääreellisiä?)

Ylinumeroituva, esim. reealiluvut nollan ja yhden välillä, reaktioaika liikenneturvallisuustutkimuksessa, joka on ylinumeroituva. Jos mitataan sekuntin kymmennesosan tarkkuudella (&Omega; = {0.0, ...) numeroituva.

xtunnaisilmiöitä tarkasteltaessa olemme kiinnostuneita esiintyykö tai _realisoituuko_ jokin **tapahtuma**. Tapahtumat ovat otosavaruuden osajoukkoja, jotka koostuvat alkeistapahtumista, ja kuuluvat **havaittavien tapahtumien joukkoon**

Df. tapahtuma: Satunnaiskokeessa tapahtuma on perusjoukon &Omega; osajoukkoa A, joka kuuluu havaittavien tapahtumien joukkoon F.

Tapahtuma A &sub; &omega; esiintyy, jos satunnaislimö lopputulos &omega; kuuluu joukkoon A.

Joukon S **Komplementti** Sc määritellään joukkona, joka ei sisällä joukon S pisteitä.

Erotus A\B := A &cup; Bc.

&Omega; = A &cup; Ac.

Toistensa poissulkevat joukot: A &cap; B == null == &Omega;c jne. jne.

Tapahtumien poissulkevuus Ai &cap; Aj == null; i != j.
