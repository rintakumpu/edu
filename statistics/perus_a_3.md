# Tilastotieteen peruskurssi a #

**Henri Pesonen (vastaanotto Ma 14&ndash;15; Pub 455)**
**Luento 3: 10.9.2013**

Luentomonisteen errata Moodlessa.

**Tentit**

1. Tentit 23.10. 13&ndash;16
2. 25.11. 9&ndash;12
3. Tammikuussa

## Otanta ##

Poimitaan laatikosta (jossa V, S ja P -värisi kuulia) kuula. Nostetaan yksi kuula, palautetaan kuula laatikkoon. Toistetaan kolme kertaa. Mikä on jono?

Esimerkissä erilaisia tapauksia on 27 kpl. (a)

Toistetaan esimerkki palauttamatta kuulia, mahdollisten tapausten joukko tippuu kuuteen. (b)

Kolmas vaihtoehto: Ei tarkastella kuulien järjestystä. Vaihtoehtoja 10 kpl. (c)

Neljäs: Ei palauteta kuulia, ei tarkastella järjestystä. Vaihtoehtoja 1 kpl. (d)

&rarr; Muodostetaan uusi otosavaruus yhdistetyistä tapahtumista.

Tapahtumien märän selvittämiseksi käytetään **kombinatoriikkaa** (matematiikan osahaara, jossa "lasketaan monellako tavalla asioita voidaan tehdä"), perustuu usein **tulosääntöön**.

**Tulosääntö**

* Otos voidaan valita k. vaiheessa.
* Vaihe i voidaan valita ni tavalla.
* Erilaisia tuloksia on n0 * n1 * ... ni = n^k 

### Järjestetty otanta ###

**Järjestetty otanta ilman palautusta:**

* Olkoon &Omega; = { &omega;1, &hellip;, &omega;n}, 
* K:n (k<=0) alkion järjestetty otos ilman palautusta n * (n-1) * (n-2) &hellip; (n - k +1) tavalla

&rarr; **k-permutaatio (n:stä)**, laskuissa on kätevää käyttää merkintää

    n! := n * (n -1)*(n-1)...2*1

n! on n-kertoma

&rarr; k-pituisia jonoja on = **n! / (n-k)!** kpl

**Stirlingin approksimaatio** n! ~= sqrt(2&pi;n) * (n/e) ^ n; jolla ominaisuus, n:n kasvaessa aproksimaatio paranee (pienillä, &lt;10 n:n arvoilla kertoma helppo laskea).

**Järjestetty otanta palauttaen:**

Esim. vakioveikkauksessa vaihtoehdot 1X2 palautetaan otosavaruuteen, jolloin rivejä **3^13 (k^n)**.

### Järjestämätön otanta ###

Kuinka monella eri tavalla voidaan k alkiota valita N.stä. Järjestyksellä, jossa alkiot poimitaan ei merkitystä (ei poimita jonoa).

&Omega;, jossa n erilaista alkiota, k luonnollinen luku siten, että k&lt;=n. Binomikerroin **(n k) := n! / k!(n-k!)** (luetaan n yli k)

**Todistus:** erilaisia **jonoja** on n! / (n-k)!, k! jonoa sisältää samat alkiot.

**Järjestämätön otanta palauttaen**

&Omega; n erilaista alkioita, k N siten, että k&lt;=n. Joukosta voidaan muodostaa k kokoinen järjestämätön otos palauttaen binomikertoimella:

    ((n+k-1) k)

Todistus on hankala ja jätetään myöhemmille kursseille.

Esimerkki, kahden kuusisivuisen nopan heitto, jolloin eri silmälukukombinaatioita ((6+2-1) 2) = 21.
