---
title: "3_Komentorivi"
draft: false
---

Komentorivin käyttäminen saattaa kuulostaa henkilöille jotka ovat tottuneet graafisiin käyttöliittymiin jopa antiikkiselta. Mutta todellisuudessa komentoriviä käytetään nykypäivänä todennäköisesti enemmän kuin koskaan. 

Syynä tähän on mm. automaatio. Ohjelmoija tekee koodiin muutoksia ja lähettää ne 


Käyttäjä saattaa yhdellä graafisen käyttöliittymän napinpainalluksella aloittaa monimutkaisen tapahtumasarjan, jossa tietokone ajaa komentorivin avulla useita pienohjelmia saavuttaen lopulta käyttäjän haluaman lopputuloksen. Nämä pienohjelmat voivat olla käyttöjärjestelmän tiedostonhallintaan liittyviä toimintoja, internet palveluita ja toteutettu jollain ihan täysin eri ohjelmointikiellellä kun varsinanen käyttöliittymä. 

Monesta ohjelmasta löytyy myös sisäänrakennettu komentorivi jolla edistyneet käyttäjät voivat muokata ohjelman toiminnallisuutta, automatisoida toistuvia vaiheita ja päästä käsiksi toiminnallisuuksiin jotä ei perus käyttöliittymästä syystä tai toisesta löydy. 
Esimerkkejä: Blender3D, Photoshop, Pelit ja niiden modaustyökalut, 

<br />

## Komentorivillä navigointi

Hae ja avaa käynnästä valikosta joko cmd, Powershell tai cmder. Nämä toimivat melko samalla tavalla joten valinnalla ei ole sikäli hirveästi väliä. 

Komentorivillä navigointi tapahtuu __cd__ komennolla (__Change directory__). Kirjoittamalla komentorivillä __cd c:/__ komentorivi siirtyy tietokoneen __c:/__ juureen. Kirjoittamalla tämän jälkeen __cd Windows__ siirtyy komentorivi __c:/__ asemalta löytyvään Windows kansioon. Takaisinpäin pääsee kirjoittamalla __cd ..__ jolloin komentorivi siirtyy takaisin Windows kansiosta __c:/__ aseman juureen. 

Jokaisella asemalla on oma erillinen "nykyinen asema"(__*Current directory*__) johon voi navigoida kirjoittamalla aseman nimen ja kaksoispisteen esim. __g:__

<table border=2>
    <tr>
        <td>
            <b>Komento</b>
        </td>
        <td>
            <b>Kuvaus</b>
        </td>
    </tr>
    <tr>
        <td>
            cd asema-kirjain:/
        </td>
        <td>
            <b>esimerkki: cd c:/ </b><br />
            Siirtyy tietokoneen c-asemalle.
        </td>
    </tr>
    <tr>
        <td>
            cd kansion nimi
        </td>
        <td>
            <b>esimerkki: cd Windows </b><br />
            siirty nykyisessä kansiossa (C:/) olevaan Windows kansioon.
        </td>
    </tr>
    <tr>
        <td>
            cd ..
        </td>
        <td>
            Siirtyy kansio-hierarkiassa taakseppäin. Esimerkiksi Windows kansiosta takaisin C-aseman juureen. 
        </td>
    </tr>
    <tr>
        <td>
            dir
        </td>
        <td>
            Listaa nykyisen kansion tiedostot ja ali-kansiot. 
        </td>
    </tr>
</table>

<br />

![Komentorivi Powershell](Kuvat/Komentorivi_Powershell.png)

Nykyisen kansion sisällön saa selville kirjoittamalla __Dir__ jolloin komentoriville tulostuu kaikki kansion sisällä olevat alikansiot ja tiedostot. 

<br />

![Komentorivi cmd](Kuvat/Komentorivi_cmd.png)

<br />

### Komentorivi Vinkkejä

<table border=2>
<tr>
    <td>
        Automaattinen täyttö (TAB / &#8633;)
    </td>
    <td>
        <ul>
            <li>
                Kirjoittaessasi kansiopolkua voit painaa __tabia__ ja komentorivi yrittää arvata ja täyttää loppuosan tiedoston tai kansion nimestä. Tämä nopeuttaa navigointia sillä käyttäjän tarvitsee kirjoittaa tiedoston tai kansion nimen alusta vain osa ja komentorivi arvaa loput. 
            </li>
            <li>
                Powershell lisää tiedostojen eteen __./__ joka tarkoittaa lähinnä nykyistä kansiota joten siitä ei tarvitse liiemmin välittää.
            </li>
        </ul>
    </td>
<tr>
    <td>
        Komentohistoria (Nuolet: &#8593; ja &#8595;)
    </td>
    <td>
        <ul>
            <li>
                Nuolinäppäimillä ylös ja alas voi selata komento-historiaa(__Command history__). Tämä helpottaa esimerkiksi python koodin ajamista sillä halutessa ajaa koodia uusiksi ei tarvitse joka kerta kirjoittaa komentosarjaa uusiksi.
            </li>
            <li>
                Cmd komentorivin historia säilyy yleensä siihen asti kunnes cmd-ikkunan sulkee. Muut komentorivi ohjelmat saattavat säilyttää komentohistoriaa huomattavasti pidempään.
            </li>
        </ul>
    </td>
</tr>
<tr>
    <td>
        Välilyönnit tiedostojen ja kansioiden nimissä.
    </td>
    <td>
        <ul>
            <li>
                Mikäli kansion nimessä on väli kuten <i><b>__Program Files__</i></b> voit kirjoittaa kansion nimen lainausmerkkeihin <i><b>cd "Program Files"</i></b>   
            </li>
        </ul>
    </td>
</tr>
</table>

<br />

## Python kooditiedoston ajaminen komentoriviltä

1. Luo kansio Python opas jonnekin helposti löydettävään paikkaan.
    * Suosittelen sijaintia C:/Projektit/PythonKansio 
2. Kopio ja liitä muistoon(__Notepad__) alla oleva koodinpätkä.

Python 3
```python
print("Terve maailma!")
```

3. Tallenna tiedosto Projektit/PythonOpas kansioon nimellä TerveMaailma.py
4. Avaa komentorivi cmd tai Powershell Windows käynnistä valikosta.
5. Navigoi komentorivillä kansioon PythonOpas
6. Suorita komentorivillä seuraava komento

```bash
python TerveMaailma.py
```

![Terve Maailma](Kuvat/TerveMaailma.png)

Komentoriville pitäisi tulostua perinteinen ["Hello World"](https://en.wikipedia.org/wiki/%22Hello,_World!%22_program) suomeksi. HelloWorld esimerkki on yleensä ensiaskel uuden ohjelmointikielen opiskelussa. HelloWorld esimerkit voivat kertoa yllättävän paljon ohjelmointikielestä ja esimerkin suorittaminen on yleensä hyvä testi jonka perusteella voi päätellä, että kaikki on ainakin tähän mennessä kunnossa.

Periaattessa tämä on kaikki mitä tarvitaan python koodin kirjoittamiseen ja ajamiseen, mutta seuraavassa osiossa

<br />
---
 &#8592; [2. Python asennus](2_PythonAsennus.md) | [4. Kehitysympäristö](4_Kehitysympäristö.md) &#8594; 