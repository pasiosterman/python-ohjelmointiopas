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

<table border=2>
    <tr>
        <td><b>Tunniste</b></td>
        <td><b>Arvo</b></td>
        <td><b>Tyyppi</b></td>
    </tr>
    <tr>
        <td>nimi</td>
        <td>Matti Meikäläinen</td>
        <td>Merkkijono</td>
    </tr>
    <tr>
        <td>syntymavuosi</td>
        <td>1994</td>
        <td>Kokonaisluku</td>
    </tr>
    <tr>
        <td>paino</td>
        <td>80.5</td>
        <td>Desimaaliluku</td>
    </tr>
    <tr>
        <td>elossa</td>
        <td>True</td>
        <td>Totuusarvo</td>
    </tr>
</table>
<br />
Muuttujan esittelyn jälkeen niiden sisältämään arvoon on mahdollista viitata koodista tunnisteen avulla sekä tietysti muuttuja nimen mukaisesti muuttaa muuttujan arvoa. Otetaan vaikka esimerkki tapauksesta jossa paino nousee 1.5kg on tämä mahdollista esittää seuraavasti. 

```python
paino = 80.5
paino = paino + 1.5
```

<table border=2>
    <tr>
        <td><b>Tunniste</b></td>
        <td><b>Arvo</b></td>
        <td><b>Tyyppi</b></td>
    </tr>
    <tr>
        <td>paino</td>
        <td>82.0</td>
        <td>Desimaaliluku</td>
    </tr>
</table>
<br />

Ylläolevassa koodissa viitataan paino-nimisen muuttujan sisältämään arvoon ja lisätään tähän 1.5kg. Kun lopputulos on saatu sijoitetaan tämä takaisin paino-nimiseen muuttujaan jolloin arvo päivittyy. Halutessa voimme säilyttää vanhan painon sijoittamalla lopputuloksen uuteen muuttujaan.

```python
paino = 80.5
uusipaino = paino + 1.5
```

<table border=2>
    <tr>
        <td><b>Tunniste</b></td>
        <td><b>Arvo</b></td>
        <td><b>Tyyppi</b></td>
    </tr>
    <tr>
        <td>paino</td>
        <td>80.5</td>
        <td>Desimaaliluku</td>
    </tr>
    <tr>
        <td>uusipaino</td>
        <td>82.0</td>
        <td>Desimaaliluku</td>
    </tr>
</table>
<br />

# Tietotyypit

Tietotyyppi on muuttujan arvon ominaisuus joka kertoo tietokoneelle minkälaisesta tiedosta on kyse ja miten sitä voi käsitellä. Pythonin sisäänrakennettuihin perustietotyyppeihin kuuluu mm. kokonaisluku, liukuluku, merkkijono ja totuusarvo. 




Luo uusi tiedosto ja anna sen nimeksi vaikka muuttujat.py jotta pääset itse kokeilemaan ja muokkaamaan seuraavia koodiesimerkkejä käytännössä. 

## kokonaisluku (engl. integer, int)



```python
arvo1 = 10
arvo2 = 20
summa = arvo1 + arvo2
print(summa)
```