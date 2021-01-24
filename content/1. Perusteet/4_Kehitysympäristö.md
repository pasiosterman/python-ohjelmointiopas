---
title: "4. Python kehitysympäristö"
draft: false
---

Kehitysympäristöllä tarkoitetaan kokonaisuutta joka pitää sisällään kaikki joko kielen, alustan tai ohjelmistokehyksen kannalta oleelliset työkalut. Yksinkertaisimmillaan tähän kokonaisuuteen kuuluu tekstinkäsittelyohjelma jolla koodia kirjoitetaan, tulkki tai kääntäjä jolla ohjelmakoodia muutetaan tietokoneen ymmärtämään muotoon. 

Monimutkaisempi esimerkki voisi olla vaikka mobiilisovellusten-kehitysmypäristö johon kuuluukin läjä työkaluja lisää. Näillä työkaluilla voi mm. testata koodia laitteella/emulaattorilla, pakata sovelluksen laittelle tarkoitetuksi asennustiedostoksi. 

<br/>

## Visual Studio Code

Koska koodin kirjoittaminen muistiolla on nykypäivänä tietynlaista masokismia on parempi, että lataamme siihen paremmin soveltuvan työkalun. Pythonille kirjoitushetkellä suositut valinnat ovat __Visual Studio Code__ *(lyh. VSCode tai Code)* ja __PyCharm__. Tässä oppassa tulemme käyttämään Visual Studio Codea sillä editori on melko suosittu myös muita ohjelmointikieliä kirjoittaessa (esim. javascript, typescript, java, rust, go).

Lataa ja asenna Visual Studio code koneellesi. Asennustiedoston voi käydä latailemassa Visual Studio Coden sivuilta joihin löytyy linkki alta.
* [Visual Studio Code - lataussivusto](https://code.visualstudio.com/)

Käytän itse versiota oppaassa versiota __1.52.1__

Kun asennus on valmis avaa Visual Studio Code. Avaa laajennusvalikko (engl. Extensions) ja hae Python ja Pylance laajennuksia. Asenna laajennukset visual studio codeen asennuspainikkeella (engl. Install)

- Laajennusvalikon saa auki myös näppäinyhdistelmällä __CTRL+SHIFT+X__
- Laajennuksista saa lisätietoja niitä klikkaamalla.

![Python laajennus](Kuvat/Python_PyLance_Asennus.png)
*(Perusasetuksilla valikko on vasemmalla, olen siirtänyt sen omassa asennuksessa oikealle)*

1. __Python laajennus__
    * Laajennus tuo editoriin toiminnallisuudet mm. ajaa, analysoida, formatoida koodia sekä tuo koodin ulkoasuun vähän väriä, mikä helpottaa koodin lukemista.
2. __Pylance laajennus__
    * Parantaa python kielen tekstin automaattista täydennystä joka nopeuttaa koodin kirjoittamista. Automaattisella täydennyksellä editori tarjoaa ehdotuksia koodia kirjoittaessa joista voi halutessaan valita täydennyksen __nuolinäppäimillä + tabilla__ haluamansa tai ihan __hiirellä klikkaamalla__. 

<br/>

## Projektikansion avaaminen VSCodessa

Avaa viime [osiossa](3_Komentorivi.md) luotu __PythonOpas__ kansio Visual Studio Codessa. Tämä onnistuu valitsemalla ylävalikosta 
> File > Open Folder

Nyt pitäisi avautua perinteinen kansion valintanäkymä josta voit navigoida PythonOpas kansioon. Mikäli laitoit kansion suosittelemaani paikkaan sen pitäisi löytyä seuraavasta polusta:
> C:\Projektit\PythonOpas

PythonOpas kansion pitäisi avautua sisältöineen Visual Studio Codeen. 

<br />

## Python koodin ajaminen VSCodella

Visual Studio Code sisältää sisäänrakennetun komentorivin jonka saa esiin näppäinyhdistelmällä __Ctrl + ö__. Vaihtoehtoisesti komentorivin saa esiin myös ylävalikosta.
> View > Terminal

Komentorivin pitäisi avautua suoraan VSCodessa auki olevaan projektikansioon. Voit suorittaa viime [osiossa](3_Komentorivi.md) luodun __TerveMaailma.py__ kooditiedoston kirjoittamalla komennon python tiedostonimi eli: 

```bash
python TerveMaailma.py
```

![VSCode komentorivi](Kuvat/VSCode_Komentorivi.png)

Toinen vaihtoehto olisi avata tiedosto ja painaa yläkulmasta löytyvää play nappulaa jolloin VSCode ajaa sillä hetkellä auki olevan python kooditiedoston komentorivillä.  

![VSCode komentorivi](Kuvat/VSCode_PlayNappula.png)