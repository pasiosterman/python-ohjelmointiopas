---
title: "1_Esittely"
draft: false
---

# Alkusanat

Tämän oppaan kirjoittamisen tarkoituksena on tarjota kevyt opas ohjelmointiin **Python** ohjelmointikielellä. Tavoitteena on välttää turhaa jaarittelua, keskittyä oleennaiseen ja käsitellä aiheet kompaktisti takertumatta nippelitietoihin ja täten välttyä [informaatioähkyltä](https://fi.wikipedia.org/wiki/Informaatio%C3%A4hky). 

Kirjoitan oppaan suomeksi sillä uskon että ohjelmoinnin perusteet on helpompi sisäistää omalla äidinkielellän. Tulen käyttämään suomea myös koodiesimerkeissä **korostaakseni asioita koodista** jotka voi itse nimetä haluamallaan tavalla. Suosittelen silti käyttämään ohjelmoinnissa pääsääntöisesti englantia jotta koodi on helpommin ymmärrettävää myös heille jotka eivät välttämättä ymmärrä suomea. Tulen ottamaan esille myös englanninkieliset termit joka toivottavasti helpottaa ongelmanratkonnassa ja hakukoneita hyödyntäessä. 

Opas nojaa vahvasti kompakteihin, kommentoituihin koodiesimerkkeihin jotka käsittelevät yhtä asiaa kerrallaan. 

# Ohjelmoinnin opiskelun haasteet

Ohjelmistokehitys on aihealueena todella laaja käsite, sisäistettävää on paljon ja asiat on helppo ymmärtää vääriin. Tämä johtaa helposti turhautumiseen jonka vuoksi osa luovuttaa jo alkumetreillä. Ohjelmoinnin perusteiden sisäistäminen ei kuitenkaan ole mikään ylitsepääsemätön este vaan vaati lähinnä sinnikkyyttä, kokeilua ja tietysti aikaa. Kun perusteet saa viimein haltuun ja asiat loksahtavat paikoilleen alkaa ohjelmointi yleensä tuntua paljon mielekkäämmältä näpertämiseltä. 

Tämän tason saavuttaminen kannattaa pyrkiä tekemään itselleen mahdollisimman helpoksi.

## Miksi Python

Python on erinomainen kieli ohjelmoinnin perusteiden opetteluun sillä sen kielioppisäännöt eli syntaksi onnistuu piilottamaan taakseen runsaasti monimutkaisuutta millä aloittelijan ei alkuvaiheessa kannata vaivata päätään. Syntaksissa yhdistyy skriptikielistä tuttu kompaktisuus sekä yleiskäyttöisten ohjelmointikielien selkeys. 

Ehkä suurin etu tulee silti mahdollisuudesta ajaa koodia skriptikielen tavoin tiedostosta rivi kerrallaan keskittyen puhtaasti siihen mikä on oppimisen kannalta sillä hetkellä oleellista. Alla havainnollistava esimerkki yksinkertaisesta "Terve maailma!" tekstin tulostamisesta **Python** ja **C#** ohjelmointikielillä. 


**Python**
```python
print("Terve maailma!")
```

**C#**
```csharp
class Sovellus 
{         
   static void Main()
   {
      System.Console.WriteLine("Terve maailma!");
   }
}
```

Kuten esimerkistä voi nähdä Pythonissa "Terve maailma!" tulostamiseen vaaditaan ainoastaan funktio joka tulostaa sille annetun "Terve Maailma!" tekstin. C#:lla taas sekoitetaan aloittelevan ohjelmoijan päätä heti alkuun monilla asioilla jotka käsitellään yleensä paljon myöhemmin ohjelmointia opetellessa. 

Näitä kieliä opiskelessa onkin yleistä kehottaa aloittelevaa ohjelmoijaa kehotetaan jättämään huomiotta valtaosa koodista melko pitkäksikin aikaa kunnes ne viimein käsitellään.

<!-- ## Python versio


## Visual Studio Code

Koodin muokkaamiseen ja ajamiseen tulen käyttämään [Visual Studio Code](https://code.visualstudio.com/) ohjelmistoa.  -->