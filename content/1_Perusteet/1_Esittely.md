---
title: "1_Esittely"
draft: false
---

## Alkusanat
Tämä on kevyt ohjelmointiopas __Python__ ohjelmointikielellä. Päädyin kirjoittamaan oppaan suomenkielellä koska englanninkielisiä oppaita löytyy jo pilmin pimein. Uskon myös, että äidinkielellä asioiden opiskelu on monelle helpompaa. Pyrin kuitenkin tuomaan esille suluissa myös joidenkin asioiden englanninkielisiä termejä, jotta niistä on helpompi hakea lisätietoja. 

Oppaassa pyrin käymään asiat yleisluontoisesti läpi takertumatta liikaa nippelitietoihin tai kielen erityisominaisuuksiin. Nämä ovat mielestäni sellaisia asioita joihin kannattaa perehtyä vasta kun perusteet ovat hallussa tai niitä oikeasti tarvitsee. Pyrin myös kirjottamaan koodin tavalla joka vastaa lähemmin muita ohjelmointikieliä mikä toivottavasti auttaa opetellessa myös muita ohjelmointikieliä.  

## Ohjelmoinnin opiskelu

Ohjelmointi tai ohjelmistokehitys on aihealueena todella laaja. Monella voi tulla seinä vastaan jo siinä vaiheessa kun yrittää päättellä mistä kannattaisi aloittaa sillä kieliä, työkaluja, termejä ja aihealueita on niin valtavasti. Aloittaessa tuntee taas itsensä helposti tyhmäksi joka saattaa olla hyvinkin turhauttavaa sillä sisäistettävää on todella paljon ja monet asiat on helppo ymmärtää väärin.

Näistä ei kannata kuitenkaan lannistua sillä ohjelmointi vaatii paljon omatoimista harjottelua ja kokeilua jotta perusteet saa sisäistettyä. Sinnikkyys palkitaan ahaa elämyksillä ja ohjelmointiin liittyvä turhautuminen vähenee usein merkittävästi. Kun yksi ohjelmointikieli on hallussa on toisen oppiminen merkittävästi helpompaa. 

Ohjelmointia opiskellessa on myös helppo yrittää haukata liian isoa palaa kerralla, erityisesti jos on jokin asia jo mielessä jota haluaisi lähteä kehittämään kuten vaikka peli, verkkopalvelu tai tietokantasovellus. Kannattaa kuitenkin välttää kiusausta ja keskittyä perusteisiin ja säästä loppupeleissä aikaa välttämällä monta sudenkuoppaa ja potentuaalista turhautumista joka yleensä liittyy siihen kun yrittää sisäistää montaa asiaa keralla. 

# Python 

## Miksi Python

Python on korkean tason ohjelmointikieli(__*high-level language*__) joka toimii melkeinpä missä tahansa käyttöjärjestelmässä. Kielen kanssa on helppo päästä alkuun sillä se vaatii lähinnä python asennuksen ja koodia voi kirjoittaa käytännössä milla tahansa tekstieditorilla. Kieli on myös alusta alkaen suunniteltu yleisluontoiseksi ohjelmointikieleksi joten se soveltuu monipuolisesti eri tarkoituksiin. 

Python syntaksia pidetään yleisesti melko helposti lähestyttävänä ja kieli onnistuu piilottamaan konepeltinsä alle mittavan määrän monimutkaisuutta josta aloittelian tai peruskäyttäjän ei kannata juuri stressata. Konepellin alle on halutessaan mahdollista kurkistaa, sillä sen [lähdekoodi](https://github.com/python) on vapaasti saatavilla. 

Oppassa tulen käyttämään __Pythonin versiota 3.8.6__ mutta asiat jota opas käsittelee tuskin tulevat radikaalisti muuttumaan joten voit ladata uudemman version. Pyrin myös ottamaan __Python 2__ poikkeavuuksia esiin jos vaikka siitä olisi apua niille epäonnisille opiskelijoille jotka joutuvat __ViLLE oppimisympäristön__ kanssa painimaan (*osannottoni*).

Tässä kohtaa voisin myös jaaritella pitkästi siitä mitä ohjelmointi on ja miten ohjelmointikielet kuten python toimivat. Esimerkkinä voisin sanoa, että Python on dynaamisesti tyypitetty(__Dynamic typing__), lennossa tulkattava(__Interpreted language__) korkean tason ohjelmointikieli(__*High-level language*__) mutta tämä ei nyt kovin hirveästi kerro henkilölle joka ei ole ohjelmointia missään muodossa harrastanut.

## Koodiesimerkkien syntaksi

Pyrin kirjoittamaan koodiesimerkit tavalla joka on mahdollisimman yhtenäinen muiden ohjelmointikielien kanssa (esim.  Javascript/TypeScript, C#, Java ja C/C++). Koodiesimerkit eivät siis välttämättä seuraa ns. "Pythonic" filosofiaa.

Muita ohjelmointikieliä opiskelleet huomaavat melko nopeasti, että python sisältää paljon taustalla tapahtuvaa ns. __taikuutta__. Taikuudella tarkoitan ohjelmointikielen tapaa piilottaa monimutkaisuutta käyttäjältä tekemällä oletuksia ja asioita automaattisesti käyttäjän tiedostamatta. Pidemmän päälle tämä on hyödyllistä sillä koodia joutuu kirjoittamaan merkittävästi vähemmän ja on täten helpompi keskittyä olennaiseen, mutta vastapainona äärimmilleen tiivistetty koodi jättää aloittelijoiden silmissä paljon kertomatta. 

Moni joutuu elämänsä aikana opettelemaan vähintään kourallisen ohjelmointikieliä. Koska yhden ohjelmointikielen osaaminen helpottaa merkittävästi toisten ohjelmointikielten opiskelua niin haluan hyödyntää Pythonin taipuisaa syntaksia helpottaakseni tätä prosessia. 