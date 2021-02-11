---
title: "1_Esittely"
draft: false
---

## Alkusanat

Tämän oppaan kirjoittamisen tarkoituksena on tarjota kevyt opas ohjelmointiin **Python** ohjelmointikielellä. Tavoitteena on välttää turhaa jaarittelua, keskittyä oleennaiseen ja käsitellä aiheet kompaktisti takertumatta nippelitietoihin ja täten välttyä [informaatioähkyltä](https://fi.wikipedia.org/wiki/Informaatio%C3%A4hky). 

Kirjoitan oppaan suomeksi sillä uskon että ohjelmoinnin perusteet on helpompi sisäistää omalla äidinkielellän. Tulen käyttämään suomen kieltä myös koodissa mikä mielestäni toimii erinomaisesti korostamaan asioita jotka käyttäjä voi ohjelmakoodissa nimetä haluamallaan tavalla. Tulen kuitenkin tuomaan englanninkieliset termit aktiivisesti tekstissä esille jotta myös englanninkieliset termit tulevat tutuksi.

Pyrin myös kirjoitamaan koodin syntaksin (**engl. syntax**) tavalla joka vastaa lähemmin muita ohjelmointikieliä jonka toivon helpottavan muiden ohjelmointikielien opiskelua ja ymmärtämistä. 

&nbsp;&nbsp;

## Ohjelmoinnin opiskelu

Ohjelmistokehitys on todella laaja aihealue jonka vuoksi ei ole kovin ilmiselvää edes mistä kannattaisi aloittaa. Erityisesti opiskelun alkuvaiheessa sisäistettävää on paljon ja monet asiat on helppo ymmärtää väärin, tämä johtaa herkästi turhautumiseen ja moni saattaa tuntea itsensä jopa tyhmäksi. Tästä ei kuitenkaan kannata lannistautua sillä kun perusteet saa jollain tasolla haltuun niin myös turhautuminen vähenee merkittävästi.

Ohjelmointia opetellessa ei kannata yrittää haukata liian isoa palaa kerralla vaan keskittyä yhteen asiaan. 

### Esimerkki opintopolku ohjelmoinin opiskeluun


1. Ohjelmoinnin perusteet
2. Olio-ohjelmoinnin perusteet
3. Suuntaus
   - a) Peliohjelmointi (**esim. Pygame, Godot,  Unity3D**)
   - b) Web-ohjelmointi (**esim. Django, Flask**)
   - c) Graafiset käyttöliittymät (**esim. TKinter, kivy, PyQT**)
   - d) Toinen ohjelmointikieli (**esim. Javascript/TypeScript, C#, Java, Rust, Go**)
     - kielen oppiminen merkittävästi nopeampaa kun perusteet on jo hallussa.

Mikäli ohjelmoinnista haluaa tehdä ammatin kannattaa varautua elinikäiseen oppimiseen. Uusien työkalujen, ohjelmien ja palveluiden opettelu on alalla arkipäivää ja vain harva tulee töissään toimeen vain yhdellä ohjelmointikiellellä. 

&nbsp;&nbsp;

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