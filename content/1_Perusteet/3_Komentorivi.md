---
title: "3_Komentorivi"
draft: false
---

Graafisiin käyttöliittymiin tottuneille komentorivi saattaa kuulostaa suorastaan antiikkiselta, mutta todellisuudessa komentoriviä käytetään enemmän kuin koskaan. Suurin syy tähän on **kasvanut tarve automatisoida asioita** erilaisten komentosarjojen avulla. Toisena syynä on **halu jakaa sovellukset pienempiin helpommin hallittaviin osiin** jolloin graafinen käyttöliittymä voi toimia erillisenä kokonaisuutena jonka voi tarvittaessa vaihtaa toiseen. 

Monesta ohjelmasta löytyy myös sisäänrakennettu komentorivi jolla edistyneet käyttäjät voivat muokata ohjelman toiminnallisuutta, automatisoida toistuvia vaiheita ja päästä käsiksi toimintoihin jotä ei perus käyttöliittymästä välttämättä löydy.

**Esimerkkejä:** Blender3D, Photoshop, Pelit ja niiden modaustyökalut, 

&nbsp;&nbsp;

***

## Peruskomentoja

```bash
# siirtyy aseman juureen esim. c:/
cd /

# siirtyy c-asemalle.
cd c:/

# listaa nykyisen kansion tai aseman sisältämät tiedostot ja kansiot.
dir

# luo kansion nimeltä testikansio
mkdir testikansio

# siirtyy kansioon testikansio
cd testikansio

# siirtyy takaisinpäin kansiohierarkiassa
cd ..

# poistaa kansion nimeltä testikansio
rmdir testikansio

# tyhjentää komentorivi syötteet
cls
```

&nbsp;&nbsp;

***

## komentorivi vinkkejä

- **Automaattinen täyttö (TAB / &#8633;)**
  - Kirjoittaessasi kansiopolkua voit painaa **tabia** ja komentorivi yrittää päätellä ja täyttää loppuosan tiedoston tai kansion nimestä.
- **Komentohistoria (Nuolet: &#8593; ja &#8595;)**
  - Nuolinäppäimillä ylös ja alas voi selata komento-historiaa(__Command history__). Tämä helpottaa esimerkiksi python koodin ajamista sillä halutessa ajaa koodia uusiksi ei tarvitse joka kerta kirjoittaa komentosarjaa uusiksi.
  - Cmd komentorivin historia säilyy yleensä siihen asti kunnes cmd-ikkunan sulkee. Muut komentorivi ohjelmat saattavat säilyttää komentohistoriaa huomattavasti pidempään.
- **Välilyönnit tiedostojen ja kansioiden nimissä.**
  -  Mikäli kansion nimessä on väli kuten **Program Files** voit kirjoittaa kansion nimen lainausmerkkeihin **cd "Program Files"**

&nbsp;&nbsp;

***

## Python kooditiedoston ajaminen komentoriviltä

1. Luo kansio nimeltä **python_opas** jonnekin helposti löydettävään paikkaan.
    * Suosittelen sijaintia **c:/projektit/python_opas** 
2. Kopio ja liitä muistoon(**engl. Notepad**) alla oleva koodinpätkä.

```python
print("Terve maailma!")
```

3. Anna tiedostolle nimi **terve_maailma.py** ja tallenna se **python_opas** kansioon.
4. Avaa komentorivi **cmd** tai **Powershell** käynnistä-valikosta.
5. Navigoi komentorivillä kansioon **python_opas**
6. Suorita komentorivillä seuraava komento

```bash
python terve_maailma.py
```

![Terve Maailma](/kuvat/perusteet/terve-maailma-komentorivi.png)

Komentoriville pitäisi tulostua perinteinen ["Hello World"](https://en.wikipedia.org/wiki/%22Hello,_World!%22_program) suomeksi. **Hello World** esimerkki on yleensä ensiaskel uuden ohjelmointikielen opiskelussa. Hello World esimerkit voivat kertoa yllättävän paljon ohjelmointikielestä ja esimerkin suorittaminen on yleensä hyvä testi jonka perusteella voi päätellä, että kaikki on ainakin tähän mennessä kunnossa.

