---
title: "6_Matemaattiset operaattorit"
draft: false
---

Matemaattiset operaattorit mahdollistavat erillaisten laskutoimitusten suorittamisen ohjelmakoodissa. Käytimme näistä muutamaa edellisessä osiossa käsitellessämme muuttujia, kokonaislukuja ja liukulukuja. Matemaattisten operaattorien käyttötarkoitukset eivät kuitenkaan rajoitu pelkästään perinteisiin matematiikasta tuttuihin laskutoimituksiin sillä esimerkiksi lisäysoperaattorilla on mahdollista yhdistää merkkijonoja toisiinsa ja vähennysoperaattoria voi käyttää vaikkapa päivämäärien kanssa.     

**Matemaattiset operaattorit.**

|  Operaattori | Nimi        |
|--------------|-------------|
| +            | lisäys      | 
| -            | vähennys    | 
| *            | kerroin     | 
| /            | jako        | 
| %            | jakojäännös |
| **           | eksponentti |

&nbsp;&nbsp;

***

## Lausekkeet (**engl. statements**)

Laskutoimitukset operaattorien kanssa suoritetaan ohjelmointikielissä lausekkeissa jotka Pythonissa päättyvät tyypillisesti rivivaihtoon. Tämä poikkeaa hieman C-sukuisista kielistä  jossa lausekkeet päätetään puolipisteeseen (**;**). 

```python
luku = 10 # lauseke 1
luku = luku + 20 # lauseke 2
luku = luku * luku # lauseke 3
print(luku) # lauseke 4
```

Lauseen päättäminen puolisteeseen (**;**) on mahdollista myös Pythonissa. Puolipisteen avulla voi kirjoittaa useamman lausekkeen samalle riville. 

```python
# 4 lauseketta samalla rivillä puolipisteellä eroteltuna.
etunimi = "Matti"; sukunimi = "Meikäläinen"; kokonimi = etunimi + " " + sukunimi; print(kokonimi)
```

Hyvänä nyrkkisääntönä luettavuuden kannalta on kuitenkin laittaa lausekkeet omalle rivilleen ohjelmointikielestä riippumatta. 

&nbsp;&nbsp;

***

## Yhteenlasku (**+**) (**engl. Addition operator**)

Yhteenlaskut tapahtuu tutulla plus-merkillä. 

```python
tulos = 5 + 2 + 3
print(tulos)
# tulostaa 10
```

Merkkijonojen lisääminen toisiinsa onnistuu sekä muuttujien ja suoraan lausekkeessa esiteltyjen 

```python
etunimi = "Matti"
sukunimi = "Meikäläinen"
# lisätään kokonimi muuttujaan etunimi + välilyönti + sukunimi
kokonimi = etunimi + " " + sukunimi
print(kokonimi)
```

&nbsp;&nbsp;

***

## Vähennyslasku (**-**) (**engl. Substraction operator**)

```python
tulos = 100 - 25
print(tulos)
# tulostaa 75
```

&nbsp;&nbsp;

***

## Kertolasku (**\***) (**engl. Multiplication operator**)

```python
tulos = 5 * 2
print(tulos)
# tulostaa 10
```

&nbsp;&nbsp;

***

## Jakolasku (**/**) (**engl. Division operator**)

Jakolaskun voi suorittaa pythonissa vinoviivalla. Yhdellä vinoviivalla jakolasku palauttaa tuloksen aina liukulukuna.

```python
tulos = 25 / 5
print(tulos)
# tulostaa 5.0
```

Käyttämällä kahta vinoviivaa(**//**) on kuitenkin mahdollista saada tulos alaspäin pyöristettynä kokonaislukuna.

```python
tulos = 25 // 5
print(tulos)
# tulostaa 5
```

&nbsp;&nbsp;

***

## Jakojäännös (**%**) (**engl. Modulus operator**)

```python
tulos = 5 % 3
print(tulos)
# tulostaa 2
```

&nbsp;&nbsp;

***

## Laskujärjestys

Lausekkeissa kannattaa olla tarkkana laskujärjestyksen kanssa sillä **kertolaskut**, **jakolaskut** sekä **jakojäännös** lasketaan aina ennen **yhteenlaskuja** ja **vähennyslaskuja**.  

```python
tulos =  5 * 10 + 5
print(tulos)
# Tulostaa 55
```

```python
tulos =  5 + 10 * 5
print(tulos)
# Tulostaa myös 55
```

**Laskujärjestys taulukko:**

|  **1.** |  **2.** |  **3.** |  **4.** |  **5.** |
|---------|---------|---------|---------|---------|
|  *      |  /      |  %      |  +      |  -      |

Laskujärjestystä on mahdollista muokata sulkujen avulla. Sulkujen käyttö on suotavaa myös luettavuuden kannalta.   

```python
tulos =  (5 + 10) * 5
print(tulos)
# Tulostaa 75
```





