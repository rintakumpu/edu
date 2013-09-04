# Tilastotieteen peruskurssi a #

**Henri Pesonen (vastaanotto Ma 14&ndash;15; Pub 455)**
**Luento 2: 4.9.2013**

## Havaittavien tapahtumien joukko (joukko-oppi jatkuu) ##

Havaittavien tapahtumien joukko F on &sigma;-algebra, eli F on otosavaruuden &Omega; kaikkien mahdollisten osajoukkojen osajoukko, joka toteuttaa ominaisuudet (_Kolmogorovin aksioomat_):

1. &Phi; sisältää ainakin yhden alkion == Havaitsemme satunnaisilmiöss varmasti jotain (matem. eksaktisti ilmaistuna)
2. jos A &isin; &sigma; niin myös Ac &isin; &sigma; ==  Jos tapahtuma on mahdollista on havaita, on oltava mahdollista havaita, ettei tapahtumaa tapahdu
3. jos A1, A2, A3 ... &isin; F, niin A1 &cup; A2 &cup; A3 &cup; ... &isin; F == Jos useamman tapahtuman esiintyminen on havaittavissa, niin voimme havaita jos yksi näistä esiintyy

**Esim:**

&Omega; = {Tupu, Hupu, Lupu}
F = {0, {Tupu}, {Hupu}, {Lupu}, {Tupu, Hupu}, {Tupu, Lupu}, {Hupu, Lupu}, {Tupu, Hupu, Lupu}} // Kolmogorovin aksioomat pätevät

## Klassinen todennäköisyys ##

Uhkapelien tarpeisiin 1600-luvulla (tai sinnepäin). Suotuisten tapahtumien lukumäärän suhde kaikkien mahdollisten tapahtumien lukumäärään. Vaaditaan, että vaihtoehtoiset tapaukset ovat **yhtä mahdollisia**, mihin vaaditaan äärellinen määrä mahdollisia tapahtumia. (Esim. nopanheitto; jokainen sivu yhtä mahdollinen, yhden sivun todennäköisyys 1/6) &ndash; todennäköisyys != mahdollisuus.

## Frekventistinen todennäköisyys ##

Satunnaiskoetta toistettaessa tapahtuman esiintymisfrekvenssi stabiloituu (konvergoituu) kohti tiettyä arvoa, kun kokeiden määrä kasvaa. **Todennäköisyys** on
esiintymisfrekvenssin raja-arvo toistojen määrän kasvaessa rajatta (esim. kolikonheitossa 0.5). _Ongelma:_ Satunnaisilmiö/koe oltava ainakin teoriassa toistettava.

## Bayesilainen todennäköisyys ##

Subjektiivisen tulkinnan mukaan todennäköisyys **uskomuksemme** tai **epävarmuutemme** mitta tapahtumista. Voimme puhua ainutkertaisten tapahtumien todennäköisyyksistä (esim. 3. maailmansota ennen vuotta 2025). Ongelmana subjektiivisuus.

## Todennäköisyysmitta ja -avaruus##

Todennäköisyysmitta df. Funktio P: F &rarr; R, jos toteuttaa seuraavat aksioomat:

1. P(&Omega;) = 1, &omega;i kuuluu varmasti otosavaruuteen, otosavaruus on varma tapahtuma
2. 0 <= P(A) <= 1 [0,1], &forall;A &isin; F &ndash; **Käytä tätä tietoa laskujen tarkastamiseen** (tentissä miinuspisteitä, jos ei mainintaa mahdottomasta tuloksesta ts. siitä, että on laskenut väärin)
3. A1, A2, ... &isin; F **ja** Ai &cap; Aj = &empty;, i != j &rarr; P(U&infin;/i=1Ai)  = &sum;&infin;/i=1 P(Ai); aksiooman 3. tulos pätee myös äärelliselle määrälle tapahtumia

Todennäköisyysavaryys df. (&Omega;, F, P)
