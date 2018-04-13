---
layout: default
title: Luentopäiväkirja / OHSIHA 2018
year: 2018
---

Tämä on Ohjelmallisen sisällönhallinnan kevään 2018 toteutuskerran luentopäiväkirja.
Toteutus noudattelee [vuoden 2017 toteutuskertaa](https://ohsiha.github.io/2017/luentopaivakirja).
Alan dynaamisuudesta johtuen sisältöjä ja toteutustapaa kuitenkin kehitetään jatkuvasti.

Osa luennoista tallennetaan [Echo360-järjestelmällä](https://echo360.org.uk/section/8b218f60-14ef-4b65-9d88-1d910ce34f49/public).

# Luentopäiväkirja

<!-- Tulossa:
* Resurssikeskeinen arkkitehtuuri, API-talous, koostepalvelut
* Web-informaatiojärjestelmien (sisällönhallintajärjestelmien) arkkitehtuuri
* Vierailuluento: Datajournalismi/DevOps/Lean Startup/Datalähtöinen ongelmanratkaisu
* Erityiskysymyksiä: tiedolla johdettu kehittäminen
* Erityiskysymyksiä: mukautuvuus & suosittelu
-->

<!-- **Tulossa perjantaina 16. helmikuuta**: Vincitin Tuomas Kaittola esittelee React-ohjelmointia. -->

Ohjelmallisen sisällönhallinnan luennot jäävät tauolle ja painopiste siirtyy harjoitustyön tekemiseen. [Johdanto datatieteeseen](jodatut.github.io/2018) jatkaa siitä mihin Ohjelmallinen sisällönhallinta jää.

## Luentoviikko 3.8 (viikko 8): Mukautuvat järjestelmät

[Esitys](http://ohsiha.github.io/2018/luento/0308/esitys.html) hypertekstinä.

Kohti mukautuvia ominaisuuksia.
Lähestymistapoja mukautuvuuteen (laiteriippumattomuus,
saavutettavuus, kansainvälistäminen &amp; kotoistaminen, personointi, suosittelijajärjestelmät),
mukautuva hypermedia,
mitä mukautetaan?,
käyttäjän mallintaminen,
hajautetut käyttäjäprofiilit,
suosittelujärjestelmät.

Koodiklinikalla hahmotellaan askelia [kohti oppivia järjestelmiä](https://ohsiha.github.io/2018/02/23/oppivat-jarjestelmat.html).

## Luentoviikko 3.6 (viikko 7): Datalla ohjattu kehitystyö

[Esitys](https://www.slideshare.net/jukkahuhtamaki/lean-startup-ja-datalla-ohjattu-kehitysty) Slidesharessa.

Lean startup ja datalla ohjattu kehitystyö.
Käytön seurannan periaatteet ja toteuttaminen (ks.
[lyhyt esitys](https://ohsiha.github.io/2018/luento/0306/esitys.html)).
Käyttödatan kerääminen.
Kontekstin aistiminen.
Esimerkkejä kontekstin tunnistamisesta ja käytön seurannasta:
<!-- <a href="http://matriisi.ee.tut.fi/hmopetus/ohsiha/2014/pruju/09/esitys.php#(9)">luentokalvot</a>,  -->
[$_SERVER](http://matriisi.ee.tut.fi/hmopetus/hm-ohj/2007/demo/jakelukonteksti/http-request-details.php),
[request.META.HTTP_REFERER](https://still-dawn-72781.herokuapp.com/headers),
[HTTP_REFERER missing](http://stackoverflow.com/questions/12369615/serverhttp-referer-missing),
[yksinkertainen sijainti](https://www.w3schools.com/html/html5_geolocation.asp),
<!-- [sijainti ja kartta](http://matriisi.ee.tut.fi/hmopetus/hm-ohj/2013/demo/sijainti/esimerkki.html), -->
[HTML5 ja uudet mahdollisuudet](http://blog.teamtreehouse.com/exploring-javascript-device-apis).

Koodiklinikalla Tuomas Kaittolan [React-demo](https://github.com/tuokai/ohsiha-demo).

## Luentoviikko 3.5 (viikko 6): Koostepalvelut

[Esitys](luento/0305/esitys.html) hypertekstinä.

Kohti hajautettua Web-hypermediaa,
yhdistetty (julkinen) data,
johdanto koostepalveluihin,
käsitteistä (mashup, survos, muusaus, fuusaus),
koostamisen tasot,
informaation visualisointi ja koostepalvelut,
eräs koostepalvelu ja sen toteutus.

Koodiklinikalla Pandas (ks.
[Datan käsittely Pythonilla](http://matriisi.ee.tut.fi/~huhtis/esitys/2014/03-edutech-python-data/#/)
tai
[Dashboard-demo](https://github.com/jukkahuhtamaki/dashboard-demo)),
Highcharts ja
D3.js.

## Luentoviikko 3.4 (viikko 5): Resurssikeskeinen arkkitehtuuri ja API-talous

Lue taustaksi API-talous 101 -kirjan [ensimmäinen luku](https://www.apitalous101.fi/luku-varoitus).

Ensin [Johdanto API-talouteen](https://www.slideshare.net/jukkahuhtamaki/johdanto-apitalouteen) ja sitten [kohti resurssikeskeistä arkkitehtuuria](https://gitpitch.com/ohsiha/2018/master?p=luento/0304#/). API-talous,
kolmikerrosmalli,
HTTP GET ja POST,
istunnot(tomuus) AJAX,
REST, HTTP ja REST,
[RESTful-periaate](http://www.vinaysahni.com/best-practices-for-a-pragmatic-restful-api), SPA ja REST.

Koodiklinikalla jatketaan Django-esittelyä. Toiseen teknologiademoon pääsee [tästä](https://ohsiha.github.io/2018/01/31/django-jatkoa.html).

## Luentoviikko 3.3 (viikko 4): Web-sovelluskehityksen perusteita ja harjoitustyöohje

Ensimmäinen [teknologiademo harjoitustyöhön liittyen](https://ohsiha.github.io/2018/01/19/html-css-django-perusteet.html). HTML/CSS:n perusteet ([MDN Web Docs](https://developer.mozilla.org/fi/) ja [W3 Schools](https://www.w3schools.com/)) sekä Django-kehitysympäristön ja siihen vaadittavien komponenttien pystyttäminen sekä Djangon [dokumentaatioon](https://docs.djangoproject.com/en/2.0/) tutustuminen.

Koodiklinikalla käydään [harjoitustyöohje](https://ohsiha.github.io/2018/harjoitustyo).

## Luentoviikko 3.2 (viikko 3): Resurssista representaatioksi

Ennakkotehtävä: perehdy [Web-sovellusten arkkitehtuurivaihtoehtoihin](https://blog.octo.com/en/new-web-application-architectures-and-impacts-for-enterprises-1/).

Web-toteutusten perusteet.
URI-tunniste, resurssi, representaatio (ks.
[Architecture of the World Wide Web](https://www.w3.org/TR/webarch/#p20)).
[Viileät URI-tunnisteet eivät muutu](https://www.w3.org/Provider/Style/URI).
Demo: twiitti resurssina (ks. [simple_read.py](https://github.com/jukkahuhtamaki/pcm-demo/blob/master/twitter-api/simple_read.py)).
Elegantit URI-tunnisteet (ks. [Use RESTful URLs and actions](http://www.vinaysahni.com/best-practices-for-a-pragmatic-restful-api#restful)).
Demo: jQueryllä resurssi representaatioksi.
HTML, CSS ja Javascript: sisältö, esitystapa, toiminnallisuus.
Taustaa tarkemmin: Learn [HTML &amp; CSS](https://www.codecademy.com/learn/web), [Javascript](https://www.codecademy.com/learn/javascript).
Edistyneille: [Bootstrap](http://getbootstrap.com/).
Koodiklinikalla tunnistetaan [jekyll-now](https://github.com/barryclark/jekyll-now) -kirjastosta esimerkkejä Web-toteutusten perusteista.

## Luentoviikko 3.1 (viikko 2): Käytännöt ja katsaus ohjelmallisen sisällönhallinnan nykytilaan

Toteutuskerran avausluento järjestetään tiistaina 9. tammikuuta 2018 kello 10.15 salissa SJ204.

Esitys [hypertekstinä](http://ohsiha.github.io/2018/luento/01/esitys.html).

Aiheet: Opintojakson ja kevään toteutuskerran esittely ja suorittamisen käytännöt.
Koodiklinikalla tutustutaan  [ohjelmallisen sisällönhallinnan tilaan vuonna 2018](http://ohsiha.github.io/2018/01/10/ohsiha-vuonna-2018).
