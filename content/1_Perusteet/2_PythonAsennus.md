---
title: "2_Pythonin_asennus"
draft: false
---

Tietokone ei ymmärrä Python koodia sellaisenaan joten tarvitsemme tulkin (__Python interpreter__) jonka avulla koodin suorittaminen onnistuu. Tämä kuuluu python asennustiedostoon jonka voi ladata Pythonin sivuilta. Pythonin voi löytää myös Windows kauppapaikalta ja Linuxilla paketinhallintajärjestelmästä.

* [Linkki Pythonin sivuille](https://www.python.org/)

Asennuksen yhteydessä rastita kohta __Add Python \*versio\* to Path__. 
![Python asennus](Kuvat/python_asennus.png)

Mikäli tämä unohtuu voit muokata asennusta ajamalla asennustiedoston uudestaan ja valitsemalla modify. Modify osiossa paina next ja valitse advanced options kohdasta __Add Python to environment variables__ ja install.

![Python asennuksen muokkaus](/Kuvat/python_muokkaus.png)

Asennettuasi Pythonin voit testata sen toimivuutta komentorivin avulla(__*Command Line Interface, CLI, Terminal*__). Komentorivin saa auki windowsilla hakemalla cmd nimistä sovellusta kun taas Linuxilla ja Macillä komentorivi kulkee nimellä terminal. 

Kokeile ajaa seuraava komentoja komentoriviltä varmistaaksesi, että python toimii. Komentoriville pitäisi tulostua asentamasi pythonin versionumero. 

```bash
python --version
```

![Python versio komentorivillä](/Kuvat/python_versio_cmd.png)

Mikäli komentorivi ei tunnista Pythonia komennoksi täytyy Python käydä lisäämässä PATH nimiseen ympäristömuuttuujaan. Alla olevasta linkistä löytyy ohjeet miten Python lisätään Path ympäristömuuttujaan.
* [Windows Ympäristömuuttujan lisäys](/Muut/PathMuuttujanMuokkaus.md)