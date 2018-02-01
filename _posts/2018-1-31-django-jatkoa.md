# Teknologiademo 2 (Django ja MTV) #

Jatkoa edellisestä teknologiademosta. Ennen tätä demoa tulisi jokaisella olla Python asennettuna ja Django-kehitysympäristö kunnossa. Mikäli ei ole, kysykää apua [Slackissa](www.ohsiha.slack.com). Todennäköisesti ette ole ongelmanne kanssa yksin, vaan joku muu on kamppailut ratkaisun kanssa.

__Huom. esimerkeissä käytetty py-komentoa, jota käytetään Pythonin kutsumiseen. Tämä voi erota riippuen versiosta tai käyttöjärjestelmästä. Macissä komento on python3.__

## Ensimmäisen Django-projektin aloittaminen

Projektihakemiston lisääminen Atomissa tapahtuu _File -> Add Project Folder..._, jonka jälkeen kaikki Djangon tiedostot, jotka luotiin automaattisesti ensimmäisen _startproject_-komennolla, näkyvät Atomin puunäkymässä. Seuraavat tiedostot pitäisi näkyä

- _ _ init _ _ .py
  - Kertoo Pythonille, että kyseessä on Python-paketti
- settings.py
  - Sisältää projektikohtaiset asetukset, joita tullaan muuttamaan mieleiseksi
- urls.py
  - Sisältää kaikki URL-tunnisteet (eroaa [SPA](https://en.wikipedia.org/wiki/Single-page_application)-toteutuksissa), joita Django voi käsitellä
- wsgi.py
  - [Web Service Gateway Interface](https://en.wikipedia.org/wiki/Web_Server_Gateway_Interface), liittyy projektin siirtämiseen internettiin, ei tällä hetkellä oleellinen
- db.sqlite3
  - Django ehdottaa vakiona SQLiten käyttämistä tietokantateknologiana, myös muut kuten PostgreSQL toimii hyvin Djangon kanssa
- manage.py
  - Tarvitaan mm. projektin ajamiseen web-toteutukseksi komennolla _py manage.py runserver_

### Applikaation lisääminen ###

Djangon applikaatio tarkoittaa yhden toiminnallisuuden lisäämistä koko web-toteutukseen (Huom. Django application != web application). Django-applikaation lisääminen onnistuu projektihakemiston sisällä komennolla

    py manage.py startapp applikaation_nimi

 Tuloksena syntyy uusi hakemisto, jonka sisällä on mm. seuraavat tiedostot _models.py_ ja _views.py_, joihin palataan myöhemmin.

Django-applikaation linkittäminen projektiin tapahtuu settings.py -tiedostossa, missä ALLOWED_HOSTS -kohtaan pitää lisätä kyseinen applikaatio.

Mikäli komentorivi ilmoittaa seuraavan tekstin _You have 14 unapplied migration(s). Your project may not work properly until you apply the migrations for app(s):_, pääsee siitä eroon komentorivin komennolla

    py manage.py migrate

### MVC Djangossa ###

MVC tulee sanoista Model, View, Controller. MVC on ajatusmalli, jonka taakse käytännössä kaikki web-teknologia pohjautuu. MVC:n tarkoituksena on luoda rakenne web-sovellusten kehittämiseen, jossa voidaan käyttää valmiita rakenteita useasti, eikä web-sovelluksia tarvitse "kovakoodata" (engl. termi _DRY, Don't repeat yourself_). Lyhykäisyydessään

- Model mallintaa, miten tietokanta kommunikoi palvelimen kanssa. Esimerkiksi tietokanta pitää kirjaa, mistä tietokantataulusta löytyy adminit
- View näyttää halutun sisällön tallennettujen "kehyksien" mukaisesti (HTML/CSS!)
- Controller pitää huolen siitä, mitä käyttäjälle näytetään sekä esimerkiksi antaa valtuuksia admineille muuttaa web-sovelluksen sisältöä

MVC:n ajatusmalli perustuu siihen, että web-sovellukset kulku menee lähes aina niin, että käyttäjä kertoo palvelimelle mitä haluaa, palvelin hakee tietokannasta tarvittavat tiedot ja näyttää ne käyttäjälle sopivassa muodossa.

Django käyttää samaa ajatusmallia, mutta käyttää termeinään MTV, Model, Template, View. Lisätietoa runsaasti netissä ja esimerkiksi [täällä](https://djangobook.com/model-view-controller-design-pattern/). Hyviä Youtube-videoita mm. [täällä](https://www.youtube.com/watch?v=1IsL6g2ixak) ja [täällä](https://www.youtube.com/watch?v=pCvZtjoRq1I).

### Demo Djangon MTV:stä ###

MTV-mallin rakentaminen tapahtuu Djangossa päinvastaisessa järjestyksessä; ensin luodaan templatet, joita näytetään käyttäjälle, sitten luodaan viewt, joissa tapahtuu web-sovelluksen logiikka, ja lopuksi modelit, joihin kytketään tietokannat. Tässä nopeassa demossa ei vielä tietokantaa kytketä Djangoon.

Templatet lisätään _settings.py_-tiedostossa. Kohdassa TEMPLATES tulee olla kirjoitettu seuraavasti:

    'DIRS': [os.path.join(BASE_DIR, "templates"),],

Tällöin Django hakee _projektin_nimi/templates/_-hakemistosta kaikki templatet.

Seuraavaksi luodaan templates-hakemisto, johon lisätään .html-tiedosto. Sisällön tuominen Djangosta .html-tiedostoon tapahtuu lisäämällä kenttä _{{ kentän_nimi }}_, jolloin Djangon views.py tietää, mihin sen tuoma sisältö kiinnitetään. Views.py-tiedostossa sisällön luominen tapahtuu esimerkiksi seuraavasti:

    from django.shortcuts import render
    from django.http import HttpResponse

    def index(request):
      eka_dict = {'sisalto': "Tämä on tekstiä views.py:stä!"}
      return render(request, 'testi_app/index.html', context=eka_dict)

Näin olet tehnyt ensimmäisen dynaamisen html-sivun!


##### Lopuksi: Ylläolevat, ja paljon enemmän löytyy vieläkin Djangon omasta [dokumentaatiosta](https://docs.djangoproject.com/en/2.0/). Lisäksi muita erityisen hyviä tutoriaaleja erityisesti vasta-alkajille ovat [Django Girls Tutorial](https://tutorial.djangogirls.org/en/) ja [The Django Book](https://djangobook.com/tutorials/). #####
