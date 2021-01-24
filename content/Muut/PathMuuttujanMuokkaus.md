---
title: "Path-muuttujan muokkaus"
draft: false
---

## Path ympäristömuuttuja

Kirjoittaessasi komennon komentoriville katsoo Windows löytääkö se vastaavaa komentoa sisäisitä komennoista jonka jälkeen se etsii komentoa vastaavaa suoritettavaa tiedostoa ulkoisista komennoista. Ulkoiset komennot ovat käytännössä suoritettavia tiedostoja joiden kansio-polku on lisätty joko järjestelmän tai käyttäjän Path ympäristömuuttujaan.

Haluamme lisätä Pythonin Path-muuttujaan koska muuten esimerkiksi Pythonin suorittamisessa __komentoriviltä__ pitäisi aina kertoa koko polku python.exe tiedostoon:

```
C:\Users\User\AppData\Local\Programs\Python\Python38\Python --version
```

Mutta mikäli lisäämme polun Python.exe:n kansioon Pythonia voi kutsua komentoriviltä paljon lyhyemmin kuten alla olevassa esimerkissä. 

```
Python --version
```

## Python sijainti

Edellä mainittu polku on Python asennuksen sijainti Windows 10 käyttäjärjestelmässä kun Pythonin asentaa oletusasetuksilla. Pythonin sijainnin saa selville vaikka hakemalla Windows kännistävalikosta haulla "Python" jolloin löytyy "__Python.exe__" tai versionumeron sekä bittisyyden kanssa esim.  "__Python 3.8(32-bit)__". 

Oikealla hiirellä klikkaamalla ja omainsuudet(__Properties__) valitsemalla pitäisi löytyä tiedoston sijainti. Vaihtoehtoisesti voi pitää shift-näppäintä pohjassa klikatessa ja valita "Avaa tiedostosijainti" (__Open file location__)

__Sijainit Windowsilla oletusasetuksilla (versiolle 3.8)__
* 64-bit - *C:\Users\User\AppData\Local\Programs\Python\Python38*
* 32-bit - *C:\Users\User\AppData\Local\Programs\Python\Python38-32*

## PATH Ympäristömuuttujan muokkaus

* Käytä Windowsin käynnistä valikon(__Start menu__) hakua ja etsi "Muokkaa järjestelmän ympäristömuuttujia" (__"Edit the system environment variables"__). 

![Windows Haku](/Kuvat/Muokkaa_ympäristömuuttujia_1.png)

<br />

* Paina avautuvasta valikosta Ympäristömuuttujat(__Environment Variables__) nappulaa

![Järjestelmän ominaisuudet valikko](/Kuvat/Muokkaa_ympäristömuuttujia_2.png)

<br />

* Etsi System variables osiosta Path ja paina muokkaa. 

>__Huom:__ Järjestelmämuuttujat(__System variables__) ovat saatavilla kaikille koneen käyttäjille, käyttäjämuuttujat ovat taas saatavilla ainoastaan nykyiselle käyttäjälle. Voit halutessasi tehdä muutoksen myös käyttäjän muuttujiin (__User variables__)


![Ympäristömuuttujat valikko](/Kuvat/Muokkaa_ympäristömuuttujia_3.png)

<br />

* Tämä näkymä on Windows 10:ssä ja Windows 7:ssa hyvin erillainen. 
    * Windows 10. 
        1. Tarkista, ettei Python polkua ole jo listattu.
        2. Lisää polku painamalla new ja liittämällä se muokattavaan kenttään kuvan mukaisesti
        6. Paina OK molempiin ikkunoihin sulkeaksesi ne ja vahvistaaksesi valinnat.
    * Windows 7 
        1. Kopioi ja liitä muuttujan arvo avautuneesta ikkunasta erilliseen tekstieditoriin kuten muistioon(__Notepad__). 
        2. Polut on eroteltu toisistaan puolipisteellä(__;__)
        3. Tarkista ettei Python polkua ole jo lisätty muuttujaan.
        4. Lisää loppuun puolipiste ja polku python.exe kansioon.
        5. Kopioi koko teksti editorista ja liitä se muuttujan arvoon.
        6. Paina OK molempiin ikkunoihin sulkeaksesi ne ja vahvistaaksesi valinnat.
    

![Ympäristömuuttujan muokkaus valikko](/Kuvat/Muokkaa_ympäristömuuttujia_4.png)