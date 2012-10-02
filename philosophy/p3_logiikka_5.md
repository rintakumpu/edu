#Luentokerta IV 2.10.2012. PUB2#

##Semantiikan ja päättelyteorian yhteydestä##

###Terveyslause (soundness; eheys)###

Jokaisen päättelyjärjestelmän mukaisesti suoritetun päättelyn tulee olla **validi**
ts. jos S:stä voidaan johtaa lause &phi; niin S:llä on loogisena seurauksena &phi;

Jos S &#8866; &phi; niin S &#8872; &phi;
Jos &phi; on teoreema, niin &phi; on loogisesti tosi. (jos &#8866; &phi;, niin &#8872; &phi;)

###Riittävyyslause###

Jokainen validi päättely on voitava suorittaa päättelyjärjestelmässä:
Jos S:llä on loogisena seurauksena &phi;, niin S:stä voidaan johtaa &phi;

Jos &phi; on loogisesti tosi lause (&#8872; &phi;) niin &#8866; &phi; (&phi; on teoreema)

###Propositiologiikan täydellisyyslause###

Päättelyjärjestelmä on _täydellinen_ joss se on sekä terve että riittävä,
toisin sanoen joss seuraava ehto teoteutuu:

_S:stä voidaan johtaa &phi; joss S:llä on loogisena seurauksena &phi;_

##Ristiriitaisuus##

Lausejoukko S on _ristiriitainen_ joss S:stä voidaan dedusoida mikä tahansa muotoa
(&phi; &and; &not;&phi;) oleva lause

_Laajennettu täydellisyyslause:_

Lausejoukko S on _ristiriidaton_ joss S:ll malli, jossa joukon lauseet yhtäaikaisesti tosia

###Riippumattomuus###

Lause &phi; on _riippumaton_ lausejoukosta S joss
S &cup; {&phi;} on ristiriidaton ja myös S &cup; {&not;&phi;} on ristiriidaton.

