---
title: "Termejä"
draft: false
---

Ohjelmistokehityksessä käytetään paljon termejä joiden avulla pyritään yleensä helpottamaan kommunikointia asiantuntijoiden välillä. Näiden termien tunteminen ja ymmärtäminen auttaakin merkittävästi ongelmien ratkonnassa. 

## Tulkki (Intrepeter) ja Kääntäjä (Compiler) 

Ennen kuin ohjelmakoodia voidaan suorittaa se pitää ensiksi kääntää muotoon jota tietokone ymmärtää. Tämä tehdään yleensä joko kerralla tai osissa rivi riviltä. Käyttäessä kääntäjää ohjelmakoodi ajetaan vasta kun koko ohjelmakoodi on käännetty, käyttäessä tulkkia ohjelmaa taas käännetään ja ajetaan rivi kerrallaan joka parhaimmassa tapauksessa mahdollistaa jopa ohjelmakoodin muokkaamisen ohjelman ollessa käynnissä. 

Python luokitellaan tulkattuihin kieliin joihin kuuluu mm. Javascript, Lua, Perl. Käänettyiksi kieliksi luokitellaan taas kielet kuten C, C++, C#, Java, Visual Basic, Go, Objective-c ja Rust. 

## Kehitysympäristö

Kehitysympäristöllä tarkoitetaan kokonaisuutta joka pitää sisällään kaikki joko kielen tai alustan kannalta oleelliset työkalut. Yksinkertaisimmillaan tähän kokonaisuuteen kuuluu tekstinkäsittelyohjelma jolla koodia kirjoitetaan sekä tulkki tai kääntäjä jolla ohjelmakoodia voidaan kääntää. 

Yksinkertaisimmillaan kyse on kokonaisuudesta johon kuuluu tekstinkäsittely ohjelma jolla ohjelmakoodia kirjoitetaan sekä kääntäjä jolla kirjoitettua ohjelmakoodia voi tulkata ja ajaa. Usein tähän ympäristöön kuuluu myös ohjelmistokehykset, pelimoottorit, kirjastot yms. jolla helpotetaan työpöytäsovellusten pelien, verkkosivujen ja palveluiden tekemistä.  

## Ohjelmakirjasto (Library)

Ohjelmoinnista keskustellesta voi usein kuulla sanonnan "pyörää ei tarvitse keksiä uudelleen" joka tarkoittaa yleensä sitä että on parempi uudelleen käyttää vanhaa valmista koodia kuin tehdä kaikki aina alusta uudelleen. Yksi tapa uudelleenkäyttää koodia on pakata se ohjelmakirjastoksi joka soveltuu käytettäväksi myös muissa projekteissa. Yleensä tälläisen kirjaston sisältö rajataan jonkin yhden tietyn ongelman ratkaisemiseen kuten vaikka tiedostoihin kirjoittamiseen, graafiikan piirtämiseen, äänten toistamiseen tai tietokannan käsittelyyn. 

Ohjelmointikieliin on yleensä sisäänrakennettu kirjasto jos toinenkin helpottamaan ohjelmistokehitystä ja tulemme hyödyntämään niitä myös tässä oppaassa. 

## Ohjelmistokehys (Framework)

Ohjelmistokehys on yleensä kokoelma ohjelmakirjastoja ja työkaluja joita käytetään jonkin tietyntyyppisten ohjelmien kehitykseen. Esimerkiksi pelikehityksessä ohjelmistokehys sisältää yleensä kirjastot jolla voi lukea käyttäjän painalluksia, piirtää grafiikkaa ruudulle, toistaa ääniä sekä varsiainsen kehyskirjaston joka yhdistää nämä kolme kirjastoa tarjoten kehittäjälle valmiin pohjan kehittää monenlaisia erillaisia pelejä. 

Tämä pohja asettaa yleensä jonkin verran vaatimuksia koodiarkkitehtuurille, mutta usein kehykset toimivat lähinnä valmiina esimerkkiratkaisuna ja ovat laajalti muokattavissa. Yhdessä sovelluksessa voi olla myös useampi ohjelmistokehys, esimerkiksi pelikehys voisi mahdollisesti käyttää integraatiokehystä mahdollistamaan sisällön jakamisen vaikka sosiaaliseen mediaan tai mahdollistamaan mikromaksut eri alustoilla.

## Pelimoottori (Game Engine)

Pelimoottorit muistuttavat idealtaan melko paljon pelinkehitykseen tarkoitettuja ohjelmistokehyksiä, mutta ne ovat yleensä vieläkin kattavampia kokonaisuuksia jotka sisältävät valtavan määrän työkaluja pelien sisällön luomiseen. Nämä työkalut nopeuttavat kehitystä merkittävästi, mutta asettavat tiettyjä rajoituksia, ehtoja ja raameja siihen miten pelejä tulee pelimoottorilla kehittää. Esimerkiksi pelimoottorin sisuksissa olevia kirjastoja ei yleensä ihan niin vain muokata sillä lähdekoodi voi olla suljettua tai pienet muutokset voivat heijastua muualle pelimoottorin toiminnallisuuksiin ja vaatia laajamittaisempia muutoksia sekä ennalta arvaamattomia ongelmia. 