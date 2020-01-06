---
layout: default
title: Luentopäiväkirja / OHSIHA 2020
year: 2020
---

Tämä on Ohjelmallisen sisällönhallinnan kevään 2020 toteutuskerran luentopäiväkirja.
Toteutus noudattelee [vuoden 2019 toteutuskertaa](https://ohsiha.github.io/2019/luentopaivakirja).
Alan dynaamisuudesta johtuen sisältöjä ja toteutustapaa kuitenkin kehitetään jatkuvasti.

Hyödynnämme [Echo360-järjestelmään tallennettuja luentoja](https://echo360.org.uk/section/89ccd5ff-39ab-417f-a411-77591e21f565/public) keväältä 2019. Mahdolliset uudet luentotallenteet julkaistaan Tampereen yliopiston Pantoptossa.


# Luentopäiväkirja
<div id="accordion">
  <h3>Tulossa</h3>
  <!-- Oh yes, using Markdown inside HTML in Github-based Jekyll! -->
  <div markdown="1">
* Luentoviikko 7 (viikko 8): Mukautuvat järjestelmät - kohti JODAa
* Luentoviikko 6 (viikko 7): Datalla ohjattu kehitystyö
* Luentoviikko 5 (viikko 6): Koostepalvelut ja visuaalinen analytiikka
* Luentoviikko 4 (viikko 5): API-talous
* Luentoviikko 3 (viikko 4): Resurssikeskeinen arkkitehtuuri
* Luentoviikko 2 (viikko 3): Resurssista representaatioksi

*Tarkempi suunnitelma tämän dokumentin kommenteissa*
</div>
</div>
<!--
-->
<!-- Tulossa: (Päivittämättä)

Ohjelmallisen sisällönhallinnan kevään toteutuskerta on päättynyt.
[Johdanto datatieteeseen](http://jodatut.github.io/2018) jatkaa siitä mihin Ohjelmallinen sisällönhallinta jäi.
-->
<!--
## Luentoviikko 3.7 (viikko 8): Mukautuvat järjestelmät

Ei ennakkotehtävää.

*Esitys [hypertekstinä](http://ohsiha.github.io/2019/luento/K7/esitys.html).*

Kohti mukautuvia ominaisuuksia.
Lähestymistapoja mukautuvuuteen (laiteriippumattomuus,
saavutettavuus, kansainvälistäminen &amp; kotoistaminen, personointi, suosittelijajärjestelmät),
mukautuva hypermedia,
käyttäjän mallintaminen,
hajautetut käyttäjäprofiilit,
suosittelujärjestelmät.

Koodiklinikalla hahmotellaan askelia [kohti oppivia järjestelmiä](https://ohsiha.github.io/2019/02/22/oppivat-jarjestelmat.html). Echon kanssa törmättiin teknisiin ongelmiin kesken tallennuksen, joten tallennetta ei valitettavasti julkaista.

## Luentoviikko 3.6 (viikko 7): Datalla ohjattu kehitystyö
Ei ennakkotehtävää

Aiheena: Lean startup ja datalla ohjattu kehitystyö, käytön seurannan periaatteet ja toteuttaminen, käyttödatan kerääminen.

*Esitys [hypertekstinä](http://ohsiha.github.io/2019/luento/K6/esitys.html).*

Koodiklinikalla puhuttiin visualisoinnista.[Toimiva demo .zip pakettina](https://ohsiha.github.io/2019/koodikliniikka/Dashboard/dashboard.zip)

## Luentoviikko 3.5 (viikko 6): Koostepalvelut ja visuaalinen analytiikka
Ei ennakkotehtävää

Aiheena: johdanto koostepalveluihin, koostamisen tasot,informaation visualisointi

*Esitys [hypertekstinä](http://ohsiha.github.io/2019/luento/K5/esitys.html).*

Koodiklinikalla perehdyttiin Djangoon.

## Luentoviikko 3.4 (viikko 5): API-talous

Esitehtävä: Lue taustaksi API-talous 101 -kirjan [ensimmäinen luku](https://www.apitalous101.fi/luku-varoitus).

Aiheena: Alustatalous, API-talous, arvonluonti API-taloudessa

*Esitys [hypertekstinä](http://ohsiha.github.io/2019/luento/K4/esitys.html).*

Koodiklinikalla Jukka Huhtamäki demosi API-taloutta käytännössä.
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


Koodikliniikalla asennettiin Django-ympäristö. Kannattaa ottaa oma kone mukaan.
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

-->

## Luentoviikko 1 (viikko 2): Käytännöt ja katsaus ohjelmallisen sisällönhallinnan nykytilaan

*Toteutuskerran avausluento toteutetaan verkkoluentona.*

*Esitys [hypertekstinä](http://ohsiha.github.io/2020/luento/K1/esitys.html).*

Aiheet: Opintojakson ja kevään toteutuskerran esittely ja suorittamisen käytännöt.
Perjantaina koodiklinikalla tutustutaan harjoitustyöhön.
<!-- Huom! Aloitamme perjantaina klo 9.00.-->

<!-- [ohjelmallisen sisällönhallinnan tila vuonna 2018](http://ohsiha.github.io/2018/01/10/ohsiha-vuonna-2018). -->
