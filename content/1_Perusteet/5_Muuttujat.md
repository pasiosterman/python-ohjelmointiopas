---
title: "5_Muuttujat"
draft: false
tags: [muuttujat, merkkijono, kokonaisluku]
---
 
Ohjelmoinnissa muuttujat koostuvat tunnisteesta (__engl. identifier__) ja muuttujan sisältämästä arvosta (__eng. value__). Pythonissa uuden muuttujan voi esitellä esimerkiksi seuraavilla tavoilla.

```python
nimi = "Matti Meikäläinen"
syntymavuosi = 1994
paino = 80.5
elossa = True
```

Yllä olevassa esimerkissä esitellään __4 muuttujaa__ joihin sijoitetaan yhtäsuuruusmerkki(=) sijoitusoperaattorilla (__engl. Assignment Operator__) haluttu arvo. 

**Alla havainnollistava taulukko neljästä esitellystä muuttujasta.** 

|  Tunniste    | Arvo              | Tyyppi        |
|--------------|-------------------|---------------|
| nimi         | Matti Meikäläinen | Merkkijono    |
| syntymavuosi | 1994              | Kokonaisluku  |
| paino        | 80.5              | Desimaaliluku |
| elossa       | True              | Totuusarvo    |

Kun muuttuja on esitelty on tähän mahdollista viitata muualta koodista jos vaikka haluaa käyttää sitä laskutoimituksessa tai sijoittaa muuttujaan uuden arvon. 
Mikäli haluamme nostaa paino muuttujan arvoa 1.5kg on tämä mahdollista tehdä seuraavasti. 

```python
paino = 80.5
paino = paino + 1.5
```

|  Tunniste    | Arvo              | Tyyppi        |
|--------------|-------------------|---------------|
| paino        | 82.0              | Desimaaliluku |

Yllä olevassa koodinpätkässä viitataan toteutetaan laskutoimitus jossa viitataan paino nimisen muuttujan arvoon. Kun laskutoimitus on suoritettu sijoitetaan lopputulos samaan paino muuttujaan sijoitusoperaattorilla(**=**) jolloin arvo päivittyy. 

Halutessa voimme säilyttää vanhan painon **sijoittamalla lopputuloksen uuteen muuttujaan**.

**Esim:**
```python
paino = 80.5
uusipaino = paino + 1.5
```

|  Tunniste    | Arvo              | Tyyppi        |
|--------------|-------------------|---------------|
| paino        | 80.5              | Desimaaliluku |
| uusipaino    | 82.0              | Desimaaliluku |

**Esim:**
```python
paino = 80.5
uusipaino = paino + 1.5
muutos = uusipaino - paino
```

|  Tunniste    | Arvo              | Tyyppi        |
|--------------|-------------------|---------------|
| paino        | 80.5              | Desimaaliluku |
| uusipaino    | 82.0              | Desimaaliluku |
| muutos       | 1.5               | Desimaaliluku |

# Kommentit

Koodiin kommenttien lisäys onnistuu \# merkillä. Python tulkki ohittaa kommenttirivit ohjelmakoodia kääntäessään joten niitä voi käyttää muistiinpanojen tekoon tai koodin toiminnallisuuden dokumentoimiseen. Muistiinpanojen lisääminen koodiin kommenttien on suotavaa erityisesti ohjelmoinnin opiskelun alkuvaiheessa jotta voi tarvittaessa luntata mitä jokin asia tarkoittikaan. 

```python
# Sijoitetaan merkkijono Matti Meikäläinen muuttujaan nimi.
nimi = "Matti Meikäläinen"

# tulostetaan nimi komentoriville print funktiolla.
print(nimi)
# tulostaa: Matti Meikäläinen
```

## Vinkkejä

1. VSCodessa **Ctrl + k + c** kommentoi nykyisen tai valitut rivit ja **Ctrl+ k + u** taas poistaa kommentin. Kyseessä on pikanäppäin sekvenssin eli **älä yritä painaa kaikkia näppäimiä samaan aikaan pohjassa** vaan pidä ctrl pohjassa ja näpäytä ensiksi k ja sitten u. 

2. Kommenteilla kommentoidaan usein koodirivejä pois jota ei haluta suorittaa. Yksi syy voi olla toimimattoman koodiosuuden kommentointi pois käytöstä väliaikaisesti tai mikäli haluaa kirjoittaa jonkun vanhan osuuden uudestaan paremmin voi vanhan osuuden kommentoida referenssiksi uudelle tai siltä varalta jos uusi versio ei toimikkaan niin kuin haluaisi.

&nbsp;&nbsp;

***

# Tietotyypit

Tietotyyppi on muuttujan arvon ominaisuus joka kertoo tietokoneelle minkälaisesta tiedosta on kyse ja miten sitä voi käsitellä. Pythonin sisäänrakennettuihin perustietotyyppeihin kuuluu mm. kokonaisluku, liukuluku, merkkijono ja totuusarvo. 

Luo uusi tiedosto ja anna sen nimeksi vaikka muuttujat.py jotta pääset itse kokeilemaan ja muokkaamaan seuraavia koodiesimerkkejä käytännössä. 

## Kokonaisluku (**engl. integer, int**)

Kokonaisluvuilla kuvataan yleensä lukumääriä, järjestysnumeroa tai taulukon soluja. 
Otetaan esimerkiksi tilanne jossa pelaajan kokonaispisteet kerrotaan kertoimella. 

```python
# kokonaispisteet muuttujaan sijoitetaan arvo 100
kokonaispisteet = 100

# kerroin muuttujaan sijoitetaan arvo 5
kerroin = 5

# kerrotaan kokonaispisteet arvo kerroin muuttujan arvolla.
# sijoitetaan lopputulos kokonaispisteet muuttujaan.
kokonaispisteet = kokonaispisteet * kerroin

# tulostetaan kokonaispisteet muuttujan arvo komentoriville.
print(kokonaispisteet)
# tulostaa: 500
```

***

## Desimaaliluku eli liukuluku (**engl. floating-point, float**)

Koska äärettömän tarkkuuden esittämiseen tarvitaan ääretön määrä muistia tyydytään desimaalilukujen kanssa yleensä 32 tai 64 bittisiin desimaalilukuihin, näitä kutsutaan **liukuluvuiksi**. Liukuluvuissa desimaaliarvon tarkkuus heikkenee kokonaisosan merkkimäärän kasvaessa mikä voi johtaa pyöristysvirheisiin. Sijoittaess muuttujaan lukumäärän desimaalierottimella (**.**) määritellään muutujan arvo automaattisesti tyypiksi liukulu.

```python
# sijoitetaan muuttujaan luku liukuluku 1.0
luku = 1.0

# sijoitetaan muuttujaan pii liukuluku 3.14159265359
pii = 3.14159265359

# jaetaan luku muuttujan arvo pii muuttujan arvolla
# sijoitetaan lopputulos tulos muuttujaan. 
tulos = luku / pii
print(tulos)
# tulostaa: 0.3183098861837697
```

Jakolaskujen lopputulos annetaan myös liukulukuna vaikka laskussa käyttäisikin kokonaislukuja ja lopputulos olisi kokonaisluku.

```python
# sijoitetaan luku1 muuttujaan kokonaisluku 3
luku1 = 3

# sijoitetaan luku2 muuttujaan kokonaisluku 1
luku2 = 1

# jaetaan luku1 arvo luku2 arvolla
# sijoitetaan lopputulos tulos muuttujaan
tulos = luku1 / luku2
print(tulos)
# tulostaa 3.0
```

***

# Totuusarvo (**engl. Boolean, Bool**)

Totuusarvo kuvaa onko jokin asia tosi vai epätosi. Esimerkkeinä voi mainita vaikka jonkin ohjelman asetus jonka voi laittaa päälle tai pois, onko pelaajalla tarpeeksi rahaa pelissä ostaakseen parannusesineen, onko peli käynnissä tai vaikka onko käyttäjä kirjautunut sisään. Totuusarvoja käytetään erityisesti ehtolausekkeissa joita tulemme käymään myöhemmin. 

Otetaan esimerkkinä vaikka tapaus jossa halutaan tieto siitä onko luku1 pienempi tai suurempi kuin luku2. 

```python
# sijoitetaan luku1 muuttujaan kokonaisluku 2
luku1 = 2

# sijoitetaan luku2 muuttujaan kokonaisluku 1
luku2 = 1

# verrataan onko luku1 suurempi kuin luku2
# sijoitetaan lopptulos suurempi nimiseen muuttujaan
suurempi = luku1 > luku2

# verrataan onko luku1 pienempi kuin luku2
# sijoitetaan lopputulos pienempi nimiseen muuttujaan.
pienempi = luku1 < luku2

print(suurempi)
# tulostaa: True
print(pienempi)
# tulostaa: False
```

***

# Merkkijono (**engl. String**)

Merkkijonoja voi ajatella tekstille tarkoitettuna tietotyyppinä. Teknisesti kyseessä on yksiulotteinen taulukko mikä voi sisältää melkeinpä mitä vain kirjaimia, merkkejä ja numeroita.
Ohjelmakoodissa merkkijonon voi alustaa kirjoittamalla tekstiä lainausmerkkien(**""**) sisään. 

**Havainnollistava taulukko merkkijonosta "Terve maailma!":**
| 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 | 12 | 14 | 
|---|---|---|---|---|---|---|---|---|---|----|----|----|----|
| T | e | r | v | e |   | m | a | a | i |  l | m  | a  | !  |

Taulukot tai pythonin tapauksessa listat käsitellään myöhemmässä osiossa.

```python
# sijoitetaan merkkijono Terve muuttujaan "tervehdys"
tervehdys = "Terve"
# lisätään merkkijono tervehdykseen merkkijono " maailma!"
# huom: myös välilyönti on merkki.
tervehdys = tervehdys + " maailma!"
# sijoitetaan muuttujaan merkkijonon seitsemäs merkki
# järjestysnumero on 6 koska taulukko alkaa nollasta.
kirjain = tervehdys[6]

print(tervehdys)
# tulostaa Terve Maailma!
print("merkki: " + kirjain)
# tulostaa merkki: m
```

### Pakomerkki (**engl. Escape character**)

Pakomerkkinä Pythonissa toimii vinoviiva(**/**) ja sen avulla on mahdollista lisätä merkkijonoon mm. rivivaihtoja(**\n**) ja tabulaattori painalluksia(**\t**). Pakomerkit mahdollistavat myös lainausmerkkien käyttämisen merkkijonoissa (**\"**). 

```python
# sijoitetaan merkkijono jossa on lainausmerkkejä sananlasku muuttujaan
sananlasku = "Sananlasku: \"Ei kukaan ole seppä syntyessään\""
# sijoiteaan merkkijono jossa on rivinvaihto monirivi muuttujaan
monirivi = "eka rivi \ntoka rivi"
# sijoitetaan merkkijono jossa on sarkain siirtymä sarkain muuttujaan
sarkain = "\t tabulaattori painallus"

print(sananlasku)
# tulostaa: Sananlasku: "Ei kukaan ole seppä syntyessään"
print(monirivi)
# tulostaa: 
#eka rivi
#toka rivi
print(sarkain)
# Tulostaa
        #Tabulaattori painallus
```

### Monirivinen  merkkijono

Pythonissa pidemmät merkkijonot on mahdollista esitellä kolmella lainausmerkillä (**"""**). Tämä kertoo Python tulkille, että merkkijono jatkuu aina seuraavaan kolmeen lainausmerkkiin asti. 

```python
pitka_teksti = """
Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
Vestibulum tincidunt nibh convallis luctus vulputate. 
In vestibulum, magna nec interdum maximus, arcu felis venenatis
ipsum, a scelerisque diam elit quis orci. 
Proin scelerisque tempus dolor, sit amet auctor dui malesuada
sit amet. Donec facilisis ex lorem, sed eleifend purus imperdiet
nec. Interdum et malesuada fames ac ante ipsum primis in faucibus. 
Maecenas ultrices iaculis arcu sit amet porttitor. 
"""

print(pitka_teksti)
```