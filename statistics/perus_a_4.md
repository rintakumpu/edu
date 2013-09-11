# Tilastotieteen peruskurssi a #

**Henri Pesonen (vastaanotto Ma 14&ndash;15; Pub 455)**
**Luento 4: 11.9.2013**

## Ehdollinen todennäköisyys ##

Usein tarkastellaan tapahtumaa A tieteän että jokin muu saman satunnaisilmiön tapahtuma B on esiintynyt. Vaikuttaako B:n esiintyminen A: esiintymisen todennäköisyyteen?

Tapahtuman B esiintyminen määrittää uuden otosavaruuden. Tarkastellaan A:n esiintymistä B.n määrittämässä otosavaruudessa.

Määritelmä: Kun tapahtuman B todennäköisyys P(B) &gt; 0 (tapahtuma ei voi olla mahdoton), niin tapahtuman A ehdollinen todennäköisyys ehdolla, että B esiintyy on:

P(A|B) = P(A &cap; B) / P(B) 
&equiv;
P(A &cap; B) = P (A|B)P(B)

Tapahtuman B todennäköisyys ehdolla, että B on tapahtunut:

P(B|B) = 1

Olkoot tapahtumat A ja B toisensa poissulkevat :

P(A|B) = P(A&cup;B) / P(B) = P(&empty;) / P(B) = 0

B:n esiintyminen **poissulkee** A:n esiintymisen mahdollisuuden.

**Huom!** P(A&cup;B) != P(A|B) &equiv;  P(todennäköisyys, että A ja B esiintyvät samanaikaisesti) != P(todennäköisyys, että A esiintyy kun tiedetään, että B esiintyy)

**Kokonaistodennäköisyys**

&Omega; = B1 &cup; B2 &cup; Bk, Bi &cap; Bj = &empty;, &forall;i != j

Tapahtuman A todennäköisyys saadaan laskettua kokonaistodennäköisyyden kaavalla:

**P(A) = P(A|B1)P(B1)+...+P(A|Bk)P(Bk)**

## Bayesin teoreema ##

Olkoon tapahtuman B todennäköisyys P(B) &gt; 0
Bayesin teoreema liittää tapahtumien A ja B, ja ehdollisten tapahtumien A | B ja B | A todennäköisyydet toisiinsa:

P(A|B) = P(B|A)P(A) / P(B)

## Tapahtumien riippumattomuus ##

Jos tapahtuman B esiintymisellä ei ole vaikutusta tapahtuman A esiintymiseen. Tapahtumat ovat riippuvaisia, jos tapahtuman B esiintyminen vaikuttaa tapahtuman A esiintymiseen:

A ja B riippumattomia joss
P(A&cap;B)=P(A)P(B)

**Riippumattomuus != poissulkevuus!** Toisensa poissulkevat tapahtumat ovat aina riippuvaisia toisistaan.

Laajennettuna A1,...,An toisistaan riippumattomia joss

P(A1&cap;...&cap;An)=P(A1) ... P(An)

**Huom!** Ei päde osaongelmalle esim A1,...,A3 -riippumattomuus ei päde parille A1,A2!

**Myös:** A ja B riippumattomia P(B) &gt; 0, joss P(A|B) = P(A).

Riippumattomuuden avulla voidaan määrätä todennäköisyysmitta yhdistetylle satunnaisilmiölle. Yhdistetty satunnaisilmiö on koostettu useasta satunnaisilmiöistä. Erityisen tärkeä on **riippumaton toistokoe**, ts. toistetaan täysin samaa koetta monta kertaa.

**Esim.** heitetään noppaa kolme kertaa peräkkäin. Ei ole syytä olettaa nopanheiton vaikuttavan tuleviin heittoihin. Olkoon Ai=i, heitolla saadaan silmäluku kuusi. Yhdistettynä:

P(A1&cap;A2&cap;A3) = P(A1) * P(A2) * P(A3) = 1 / 216.



