---
title: "5_Muuttujat"
draft: false
---
 
Ohjelmoinnissa muuttujat koostuvat tunnisteesta (__engl. identifier__) ja muuttujan sisältämästä arvosta (__eng. value__). Pythonissa uuden muuttujan voi esitellä esimerkiksi seuraavilla tavoilla.

```python
nimi = "Matti Meikäläinen"
syntymavuosi = 1994
paino = 80.5
elossa = True
```

Ylläolevassa esimerkissä esitellään __4 muuttujaa__ joihin sijoitetaan yhtäsuuruusmerkki(=) sijoitusoperaattorilla (__engl. Assignment Operator__) haluttu arvo. Alla havainnollistava taulukko neljästä esitellystä muuttujasta. 

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

Ylläolevassa koodinpätkässä viitataan toteutetaan laskutoimitus jossa viitataan paino nimisen muuttujan arvoon. Kun laskutoimitus on suoritettu sijoitetaan lopputulos samaan paino muuttujaan sijoitusoperaattorilla(**=**) jolloin arvo päivittyy. 

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
| muutos       | 1.5               | Erotus        |

# Kommentit

Koodiin kommenttien lisäys onnistuu \# merkillä. Python tulkki ohittaa kommenttirivit ohjelmakoodia kääntäessään joten niitä voi käyttää muistiinpanojen tekoon tai koodin toiminnallisuuden dokumentoimiseen. Muistiinpanojen lisääminen koodiin kommenttien on suotavaa erityisesti ohjelmoinnin opiskelun alkuvaiheessa jotta voi tarvittaessa luntata mitä jokin asia tarkoittikaan. 

```python
# Sijoitetaan merkkijono Matti Meikäläinen muuttujaan nimi.
nimi = "Matti Meikäläinen"
# tulostetaan nimi komentoriville print funktiolla.
print(nimi)
```

# Tietotyypit

Tietotyyppi on muuttujan arvon ominaisuus joka kertoo tietokoneelle minkälaisesta tiedosta on kyse ja miten sitä voi käsitellä. Pythonin sisäänrakennettuihin perustietotyyppeihin kuuluu mm. kokonaisluku, liukuluku, merkkijono ja totuusarvo. 

Luo uusi tiedosto ja anna sen nimeksi vaikka muuttujat.py jotta pääset itse kokeilemaan ja muokkaamaan seuraavia koodiesimerkkejä käytännössä. 

## kokonaisluku (engl. integer, int)

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
```

## Desimaaliluku eli liukuluku (engl. floating-point, float)

Koska äärettömän tarkkuuden esittämiseen tarvitaan ääretön määrä muistia tyydytään desimaalilukujen kanssa yleensä 32 tai 64 bittisiin desimaalilukuihin. Näitä kutsutaan liukuluvuiksi. Liukuluvuissa desimaaliarvon tarkkuus heikkenee kokonaisosan merkkimäärän kasvaessa mikä voi johtaa pyöristysvirheisiin.  

```python
a = 1.0
pi = 3.14159265359
tulos = a / b
print(tulos)
```