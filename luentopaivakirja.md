---
layout: default
title: Luentopäiväkirja / OHSIHA 2019
year: 2019
---

Tämä on Ohjelmallisen sisällönhallinnan kevään 2019 toteutuskerran luentopäiväkirja.
Toteutus noudattelee [vuoden 2018 toteutuskertaa](https://ohsiha.github.io/2018/luentopaivakirja).
Alan dynaamisuudesta johtuen sisältöjä ja toteutustapaa kuitenkin kehitetään jatkuvasti.

Luennot tallennetaan [Echo360](https://echo360.org.uk/section/89ccd5ff-39ab-417f-a411-77591e21f565/public)-järjestelmällä.

# Luentopäiväkirja

<div id="accordion">
  <h3>Tulossa</h3>
  <!-- Oh yes, using Markdown inside HTML in Github-based Jekyll!-->
  <div markdown="1">

* Viikko 3.7: Mukautuvat järjestelmät - kohti JODAa
* Viikko 3.6: Datalla ohjattu kehitystyö

*Tarkempi suunnitelma tämän dokumentin kommenteissa*

</div>
</div>

<!-- Tulossa: (Päivittämättä)

Ohjelmallisen sisällönhallinnan kevään toteutuskerta on päättynyt.
[Johdanto datatieteeseen](http://jodatut.github.io/2018) jatkaa siitä mihin Ohjelmallinen sisällönhallinta jäi.

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
[$_SERVER](http://matriisi.ee.tut.fi/hmopetus/hm-ohj/2007/demo/jakelukonteksti/http-request-details.php),
[request.META.HTTP_REFERER](https://still-dawn-72781.herokuapp.com/headers),
[HTTP_REFERER missing](http://stackoverflow.com/questions/12369615/serverhttp-referer-missing),
[yksinkertainen sijainti](https://www.w3schools.com/html/html5_geolocation.asp),
[HTML5 ja uudet mahdollisuudet](http://blog.teamtreehouse.com/exploring-javascript-device-apis).

Koodiklinikalla Tuomas Kaittolan [React-demo](https://github.com/tuokai/ohsiha-demo).
-->

## Luentoviikko 3.5 (viikko 6): Koostepalvelut ja visuaalinen analytiikka
Ei ennakkotehtävää

<!--[Esitys](luento/0305/esitys.html) hypertekstinä

Kohti hajautettua Web-hypermediaa,
yhdistetty (julkinen) data,
käsitteistä (mashup, survos, muusaus, fuusaus),
eräs koostepalvelu ja sen toteutus.

-->

Aiheena: johdanto koostepalveluihin, koostamisen tasot,informaation visualisointi


Koodiklinikalla perehdytään Djangoon. 
<!--
Pandas (ks.
[Datan käsittely Pythonilla](http://matriisi.ee.tut.fi/~huhtis/esitys/2014/03-edutech-python-data/#/)
tai
[Dashboard-demo](https://github.com/jukkahuhtamaki/dashboard-demo)),
Highcharts ja
D3.js.
->

## Luentoviikko 3.4 (viikko 5): API-talous

Esitehtävä: Lue taustaksi API-talous 101 -kirjan [ensimmäinen luku](https://www.apitalous101.fi/luku-varoitus).

Aiheena: Alustatalous, API-talous, arvonluonti API-taloudessa

*Esitys [hypertekstinä](http://ohsiha.github.io/2019/luento/K4/esitys.html).*

Koodiklinikalla Jukka Huhtamäki demoamassa API-taloutta käytännössä.
Esimerkit:
[visittampere-API](https://github.com/ohsiha/2019-01-visittampere-API) ja
[twitter-collector](https://github.com/ohsiha/2019-01-twitter-collector)

## Luentoviikko 3.3 (viikko 4): Resurssikeskeinen arkkitehtuuri
Ei ennakkotehtävää.

Aiheena: kolmikerrosmalli,
HTTP GET ja POST,
istunnot(tomuus) AJAX,
REST, HTTP ja REST,
[RESTful-periaate](http://www.vinaysahni.com/best-practices-for-a-pragmatic-restful-api), SPA ja REST.

*Esitys [hypertekstinä](http://ohsiha.github.io/2019/luento/K3/esitys.html).*


Koodikliniikalla asennetaan Django-ympäristö ja tutustutaan Djangoon, mikäli ehditään. Kannattaa ottaa oma kone mukaan.
Lähdemme koodikliniikalla liikkeelle oletuksesta, että kaikilta löytyy koneeltaan selain ja editori. Mallisuorituksessa käytetään [Visual Studio Codea](https://code.visualstudio.com/)), mutta harjoitustyön on mahdollista suorittaa myös muilla editoreilla. Lisäksi windowsin käyttäjien kannattaa ladata [python](https://www.python.org/downloads/). Sen asentamisen käymme läpi koodikliniikalla.

Kurssin Slack-alusta on nyt julkaistu. Kutsulinkki on lähetetty sähköpostitse kaikille kurssin osallistujille.

## Luentoviikko 3.2 (viikko 3): Resurssista representaatioksi

Ennakkotehtävä: perehdy [Web-sovellusten arkkitehtuurivaihtoehtoihin](https://blog.octo.com/en/new-web-application-architectures-and-impacts-for-enterprises-1/).

Aiheena: Web-toteutusten perusteet.
URI-tunniste, resurssi, representaatio
HTML, CSS ja Javascript: sisältö, esitystapa, toiminnallisuus.

*"Esitys" [hypertekstinä](http://ohsiha.github.io/2019/luento/K2/esitys.html).*

Lisämateriaalia: Taustaa tarkemmin: Learn [HTML &amp; CSS](https://www.codecademy.com/learn/web), [Javascript](https://www.codecademy.com/learn/javascript).
Edistyneille: [Bootstrap](http://getbootstrap.com/).

Koodikliniikalla tutustutaan HTML + CSS. Kannattaa ottaa oma kone mukaan. Koodikliniikan esimerkit: [html](http://ohsiha.github.io/2019/koodikliniikka/html+css+js/index.html) [css](http://ohsiha.github.io/2019/koodikliniikka/html+css+js/index.css)


## Luentoviikko 3.1 (viikko 2): Käytännöt ja katsaus ohjelmallisen sisällönhallinnan nykytilaan

*Toteutuskerran avausluento järjestettiin tiistaina 8. tammikuuta 2019 kello 10.15 salissa SJ204*.

*Esitys [hypertekstinä](http://ohsiha.github.io/2019/luento/K1/esitys.html).*

Aiheet: Opintojakson ja kevään toteutuskerran esittely ja suorittamisen käytännöt.
Perjantaina koodiklinikalla tutustuttiin harjoitustyöhön. Huom! Aloitamme perjantaina klo 9.00.
[ohjelmallisen sisällönhallinnan tila vuonna 2018](http://ohsiha.github.io/2018/01/10/ohsiha-vuonna-2018).
