﻿---
layout: default
title: Harjoitustyöohje / OHSIHA 2020
year: 2020
---

<p><strong>Status:</strong> Ohjeen päivittäminen vuodelle 2020 on vielä hieman kesken, mutta perusajatus ei tule muuttumaan.</p>

<p><strong>Ilmoita epäjohdonmukaisuuksista
  <a href="https://ohsiha.slack.com/archives/C8Q40NY69">Slackin #general-kanavalla</a> tai suoraan <a href="mailto:jukka.huhtamaki@tuni.fi">Jukalle</a>.
</strong></p>

<p>Harjoitustyö on pakollinen osa Ohjelmallisen sisällönhallinnan
<a href="suorittaminen">suorittamista</a>.
Näin siksi, että sisällön käsittelyn automatisoinnin ja verkkopalveluiden toiminnallisuuksien kehittäminen edellyttää välttämättä käytännön harjoittelua.</p>
<p>Harjoitustyön lopputuloksena syntyy koodiportfolio, joka kokoaa yhteen harjoitustyöhön toteutetut toiminnot ja niiden tiiviin dokumentaation.

</p>
<p>Keväällä 2020 voit käyttää harjoitustyön tekemiseen seuraavia vaihtoehtoisia teknologioita:</p>

<ul>

  <li><a href="https://www.djangoproject.com/" target="_blank">Django</a>,
  <a href="https://palletsprojects.com/p/flask/" target="_blank">Flask</a>, <a href="https://www.pylonsproject.org/" target="_blank">Pylons</a> (<a href="https://turbogears.org/" target="_blank">TurboGears</a>, <a href="https://trypyramid.com/" target="_blank">Pyramid (vanha BFG)</a>) tai muu valitsemasi Python-kehys </li>
<li><a href="https://rubyonrails.org/" target="_blank">Ruby on Rails</a></li>
<li><a href="https://nodejs.org/" target="_blank">Node.js</a> (+ esim. <a href="https://backbonejs.org/" target="_blank">Backbone.js</a>)</li>
<li>PHP (ja halutessasi <a href="https://codeigniter.com/" target="_blank">CodeIgniter</a>, <a href="https://laravel.com/" target="_blank">Lavarel</a> tai muu valitsemasi PHP-sovelluskehys)</li>
<li>.Net</li>
</ul>

<p>
	Mikäli olet aloitteleva Web-kehittäjä, suosittelemme Django-kehystä.
	Jos taas olet suorittanut Web-ohjelmoinnin tai olet muuten jo ehtinyt kerryttämään devausosaamistasi, kannustamme valitsemaan itsellesi uuden teknologian.
</p>
<p>
  Käyttötarkoitukseen soveltuvan toteutusteknologian valinta on keskeinen osa onnistunutta Web-kehitysprojektia.
  Tästä syystä on hyödyllistä tutustua eri teknologioihin - vahvuuksineen ja heikkouksineen.
</p>
<!--<p>
  Halutessasi voit tehdä harjoitustyön myös räätälöitävällä sisällönhallintajärjestelmällä, esimerkiksi tiettyyn käyttötarkoitukseen muokatulla <a href="https://fi.wordpress.org/">WordPressillä</a>.
</p>
--><p>
  Ohjelmallisen sisällönhallinnan harjoitustyössä keskitytään
  järjestelmien toiminnallisuuksiin ja automatisoinnissa
  tarvittaviin prosesseihin.
  Tämä tarkoittaa käytännössä esimerkiksi yhteisöllisten toimintojen
  kehittämistä, sovelluksen keräämän datan esittämistä visualisoiden
  tai muuta (palvelun käyttäjän näkökulmasta) "luovaa" toimintaa.
  Teknisen arkkitehtuurin laadukas toteutus on siis nyt toissijainen tavoite.
</p>

## Minimivaatimukset

Keväällä 2020 harjoitustöissä painotetaan datakeskeisten palvelujen kehittämistä. Ota lähtökohdaksi jokin olemassa oleva data, ota se käyttöön omassa palvelussasi ja rakenna dataa edelleen jalostava toiminnallisuus. Esimerkkejä datan lähteistä ovat avoimen datan kokoelmat
[Tampereella](https://data.tampere.fi/fi/) ja
[Helsingissä](http://www.hri.fi/fi/),
[Spotify](https://developer.spotify.com/web-api/),
[Twitter](https://developer.twitter.com/en/docs/tweets/search/overview/standard.html) - ja
[Tampere3](https://avoindata.tuni.fi/)!
Kattavia datalähdelistauksia löydät muun muassa  ProgrammableWeb- ja
[apinf.io-palveluista](https://apinf.io/).  

Harjoitustyön minimivaatimuksena on toteuttaa verkkopalvelu, joka näyttää dataa käyttäjälle vuorovaikutteisella tavalla. Lisäksi käyttäjällä on mahdollisuus rekisteröityä ja kirjautua palveluun.
Löydät lisätietoa tämänkaltaisista datatuotteista esimerkiksi Tuomas Kaittolan diplomityöstä [Web-teknologioilla toteutetun datatuotteen arkkitehtuuri](https://trepo.tuni.fi/handle/123456789/25359).

Jos kuitenkin haluat toteuttaa Web-palvelun ilman erillistä datalähdettä, minimivaatimukset täyttää palvelu jonka sisältöä on mahdollista lisätä, muokata, poistaa ja listata Web-käyttöliittymän tuella.
Toteuta tällöin seuraavat ominaisuudet:
<ul>
  <li>sisäänkirjautuminen,</li>
  <li>uloskirjautuminen (&quot;Kiitos ja tervetuloa uudestaan&quot;),</li>
  <li>listaus sisällöstä,</li>
  <li>uuden sisältöartikkelin (resurssin) lisääminen ja</li>
  <li>sisältöartikkelin tietojen muokkaaminen.</li>
</ul>

Harjoitustyön pohjana on mahdollista hyödyntää aikaisemmin esimerkiksi harrastusprojektina toteutettua sovellusta siinä tapauksessa, että sitä ei aikaisemmin ole miltään osin käytetty osana mitään opintosuoritusta.
Vanhan työn käyttäminen ei kuitenkin anna erivapauksia pisteiden jakamisen perusteisiin: ominaisuuden on tässäkin tapauksessa vastattava annettua kuvausta.

<!--<p>
  Huomaathan, että harjoitustyön tuloksena ei välttämättä tarvitse syntyä tuotantokelpoista verkkopalvelua; erilaisten ominaisuuksien kehittelyä ja esittelemistä tukeva prototyyppi riittää oikein hyvin.
</p>
-->
Harjoitustyön tekeminen alkaa kehitysympäristön perustamisella ja valinnalla.
Voit joko asentaa itsellesi vaikkapa Django-ympäristön tai perustaa ympäristön valitsemallesi alustalle.
[Heroku](https://www.heroku.com/) on erityisen kiinnostava vaihtoehto ja palvelimen tuunaamisesta kiinnostunut voi ottaa käyttöön vaikkapa <a href="https://aws.amazon.com/" target="_blank">Amazon AWS:n</a> - nyt tavoitteena on kuitenkin edetä suoraviivaisesti kehittämään varsinaista sovellusta.

## Esimerkkejä aiheista

Opiskelija saa valita harjoitustyönsä aiheen vapaasti, luonnollisesti hyvän maun puitteissa. Esimerkkejä aiheista:
<p>
  <strong>Koostepalvelu (mashup)</strong> Olennaisen osan nykyaikasta Web-palvelutarjontaa muodostavat erilaiset koostepalvelut (mashup), jotka koostavat, yhdistelevät, jalostavat ja rikastavat eri lähteistä kerättyä tietoa.
  Keskeisessä roolissa koostepalvelujen toteuttamisessa ovat verkkopalvelujen tarjoamat rajapinnat (Web API), joiden tuella tietoja voidaan ohjelmallisesti siirtää verkkopalvelujen välillä.
  Erilaiset paikkatiedon ja kartan yhdistelmät ovat yleisimmin toteutettuja koostepalveluita, mutta esimerkiksi <a href="https://d3js.org/" target="_blank">D3.js-kirjaston</a> ja avoimen datan yhdistelmällä saa aikaan paljon muutakin.
</p>
<p>
  Toteuta <strong>maailman paras opinto-opas</strong>, joka esittää opinto-oppaan tiedot opiskelijalle hyödyllisellä tavalla.
  Minkälaisia vuorovaikutteisia ominaisuuksia opinto-oppaassa voisi olla? Miten opinto-oppaan tietoja voi visualisoida?
  Onko opinto-oppaasta mahdollista tehdä yhteisöllinen?
</p>
<p>
  <strong>Uuden ajan reittiopas</strong> Esimerkiksi TKL tarjoaa jo käyttäjälle varsin käteviä palveluita bussiaikataulujen selvittämiseen, mutta parannettavaakin on.
  Palvelut eivät aina osaa auttaa käyttäjää lähimmän pysäkin valinnassa: parhaassa tapauksessa käyttäjä voisi etsiä sopivan bussin valitsemalla esim. "Kotiin".
  Aikaisemmin kuljettujen reittien muistaminen ja niiden ehdottaminen auttaisivat myös käyttäjää minimoimaan palvelun kanssa käytetyn ajan.
  Mitä muita toimintoja palvelu voisi toteuttaa?
</p>
<p>
  Edellä mainittuja aiheita voi vapaasti muokata siten, että ne sopivat paremmin tekijän omiin tarpeisiin.
  Erityisen suositeltavaa on keksiä jokin ehdotettuja parempi aihe.
  Inspiraatiota voit kerätä vaikkapa tutustumalla Demolassa tarjolla oleviin
  <a href="https://applications.demola.net/" target="_blank">projektiaiheisiin</a> tai programmableweb.com-sivuston <a href="https://www.programmableweb.com/mashups" target="_blank">koostepalveluesimerkkeihin</a>.
</p>
<p>
  Kurssin harjoitustyö on myös mahdollista suorittaa myös SCIL-projektina. SCIL-projektissa ideoidaan ja kehitetään sovelluksia, jotka hyödyntävät   Tampereen korkeakouluyhteisön avoimen datan palvelua. Katso lisätietoja <a href="http://scil.tampere3.fi/projects/avoin-data/">tehtävänannosta</a>.
</p>.

## Harjoitustyöpisteet ja arvosana

  Harjoitustyöstä voi kerätä pisteitä yhteensä 18 kappaletta.
  Harjoitustyöstä kerättävät pisteet vaikuttavat arvosanaan
  [suorittamisohjeen](https://ohsiha.github.io/2020/suorittaminen) mukaisesti

<p>Neljä vaihetta:</p>
<ol>
<li>
  Kehitysympäristön perustaminen: Django käyntiin omalle koneelle
  tai esimerkiksi Herokun käyttöönotto.
  Katso <a href="https://ohsiha.github.io/2020/01/22/apukysymyksia">apukysymykset dokumentointiin</a>.
  Palautus <strong>perjantaihin 21. helmikuuta kello 17</strong> mennessä. (3 pistettä)
</li>
<li>
  Esimerkkipalvelu valitsemallasi teknologialla:
  Tuki kirjautumiseen ja rekisteröitymiseen tai jokin vaihtoehtoinen tapa käyttäjäkohtaisen tilan ylläpitämiseen sekä esimerkkidatan näyttäminen tai lisää-näytä-päivitä-poista (CRUD) -toiminnot.
  Palautus <strong>perjantaihin 13. maaliskuuta kello 17</strong> mennessä. (3 pistettä)
</li>
<li>
  Datarajapinnan käyttö: Lue dataa oman sovelluksesi käyttöön tarkoituksenmukaisen lähteestä.
  Integroi data elimelliseksi osaksi palvelusi tietosisältöä.
  Voit joko ottaa käyttöön soveltuvan API:n tai vaihtoehtoisesti
  lukea palvelun käyttöön staattisen datan (esimerkiksi <a href="https://data.tampere.fi">data.tampere.fi</a>).
  Palautus <strong>perjantaihin 3. huhtikuuta kello 17</strong> mennessä. (3 pistettä)
</li>
<li>
  Visualisointi: sovelluksen keräämän tai datarajapinnasta luetun datan ei-triviaali visualisointi (siis jotain muuta kuin yksittäinen toimistografiikkaelementti tai joukko kartalle heitettyjä tietoja).
  Käytännössä esimerkiksi suurin osa D3.js-kirjastolla toteuteista visualisoinneista voidaan luokitella ei-triviaaliksi.
  Toteutukseksi käy myös yksinkertaisista, esimerkiksi Highchartsilla toteutetuista visualisoinneista muodostettu kojelauta (dashboard).
  Palautus <strong>perjantaihin 17. huhtikuuta kello 17</strong> mennessä. (3 pistettä)
</li>
</ol>

<p>
  Voit tuplata edelliset pisteet valmistelemalla Koodiklinikalle demon toteutuksestasi.
  Ota yhteyttä Jukkaan jos olet kiinnostunut mahdollisuudesta.
</p>

Edellä kuvatut neljä kokonaisuutta voit toteuttaa omalla koneellasi pyörivässä paikallisessa kehitysympäristössä. Mikäli haluat kerätä **lisää pisteitä seuraavia kokonaisuuksia toteuttamalla**, sinun on ensin julkaistava palvelusi Webiin. Palautus <strong>keskiviikkoon 29. huhtikuuta kello 17</strong> mennessä:

**SPA-toteutus** (3 pistettä):
Palvelusi toimii Single Page Application -periaatteella. Toteutus perustuu esimerkiksi
  [Vue.js](https://vuejs.org/),
  [React](https://reactjs.org/) tai
  [AngularJS](https://angularjs.org/)-kirjastoon.

<p><strong>Käytön analytiikka</strong> (3 pistettä):
Ota käyttöön analytiikkaratkaisu, joka mahdollistaa käyttäjien toiminnan seuraamisen suppiloanalyysiperiaatteen mukaisesti, vrt. <a href="https://mixpanel.com/blog/2009/06/10/introduction-to-analytics-funnel-analysis/">Funnel Analysis</a>.  </p>
<p id="botti">

<strong>Botti</strong> (3 pistettä):
Toteuta botti, joka esimerkiksi tervehtii sivulle saapuvaa käyttäjää ja kysyy miten häntä voisi palvella, tarjoaa palvelusi sisältöä Facebook-chatissa tai välittää hyödyllisiä päivityksiä Slack-kanavalle.
</p>

<p id="reaaliaika">
  <strong>Reaaliaikainen käyttöliittymä</strong> (3 pistettä):
  Näytä järjestelmän tietosisällössä tapahtuvat muutokset käyttäjälle reaaliajassa.
  Esimerksi toteuttamasi kojelauta tai kotonasi tietoa tarjoileva näyttötaulu päivittyvät automaattisesti.
</p>

<strong>Folksonomioihin perustuva taggaaminen</strong> (2 pistettä):
Nimihirviö viittaa tyypilliseen Web 2.0 -palvelujen piirteeseen, joka mahdollistaa käyttäjien vapaasti määrittelemien avainsanojen liittämisen palvelun tietosisältöön.
Merkinnät näkyvät kaikille palvelun käyttäjille ja niitä käytetään esimerkiksi tietosisällön listaamiseen.
Esimerkiksi <a href="https://www.last.fm/" target="_blank">Last.fm</a> soveltaa tageja monipuolisesti.
Pisteiden kerääminen edellyttää myös suosittujen avainsanojen suosittelumekanismin toteuttamista (”Popular tags for this artist”, “recommended tags”).

**AJAX-toteutus** (1 piste):
AJAX-teknologian soveltaminen verkkopalvelun käyttöliittymän toteutuksessa (sekä asynkroninen tiedonsiirto että käyttöliittymän dynaaminen mukauttaminen).
  AJAX-toteutus voi liittyä esimerkiksi käyttöliittymän dynaamiseen päivittämiseen tai käyttäjän syötteen välittämiseen palvelimelle tarkastettavaksi ja virheellisestä syötteestä ilmoittamiseen.
  Myös tagien lisäysmekanismit (ks. <a href="https://en.wikipedia.org/wiki/Tag_%28metadata%29" target="_blank">tag</a><a href="https://en.wikipedia.org/wiki/Tag_%28metadata%29" target="_blank">eja käsittelevä artikkeli</a> Wikipediassa) ovat pääsääntöisesti AJAX-perustaisia.


<strong>HTML5-pohjainen käyttöliittymä</strong> (1 piste):
  Ota verkkopalvelussasi käyttöön vähintään kaksi seuraavista HTML5-kielen esittelemistä tai siihen keskeisesti liittyvistä uusista ominaisuuksista:
  <a href="https://www.whatwg.org/specs/web-apps/current-work/multipage/the-canvas-element.html" target="_blank">Canvas</a>,
  <a href="https://www.w3.org/TR/webstorage/" target="_blank">Web Storage</a>,
  <a href="https://www.w3.org/TR/workers/" target="_blank">Web Workers</a>,
  <a href="https://www.w3.org/TR/websockets/" target="_blank">Web Socket</a> ja
  <a href="https://www.w3.org/wiki/HTML5_form_additions" target="_blank">uudet lomakeominaisuudet</a>.

<strong>Kertakirjautuminen</strong> (1 pistettä):
Yksittäiset palveluntarjoajat tarjoavat usein <a href="https://oauth.net/" target="_blank">OAuth-protokollaan</a> perustuvia keinoja kertakirjautumisen toteuttamiseen,
ks. esimerkiksi <a href="https://developers.facebook.com/" target="_blank">Facebook</a><a href="https://developers.facebook.com/docs/guides/web/#login" target="_blank"> for Websites: Authentication</a>,
<a href="https://code.google.com/apis/accounts/docs/GettingStarted.html" target="_blank">Authentication and Authorization for Google APIs</a> ja
<a href="https://developer.twitter.com/en/docs/basics/authentication/overview/authentication-and-authorization.html" target="_blank">Twitter: </a><a href="https://developer.twitter.com/en/docs/basics/authentication/overview/authentication-and-authorization.html" target="_blank">Authentication &amp; Authorization</a>.
Kerää piste toteuttamalla tuki vähintään yhdelle mainituista kirjautumismenetelmistä.

<strong>Sovelluskehittäjän rajapinta</strong> (3 pistettä):
Mahdollista sovelluksesi keräämän tietosisällön hyödyntäminen ja/tai muokkaaminen muille kehittäjille toteuttamalla sovellukseesi <a href="https://en.wikipedia.org/wiki/Application_programming_interface#Web_APIs">Web API</a> eli sovelluskehittäjärajapinta.

<!--<p><strong>Älypuhelinnäkymä sovellukseen</strong> (3 pistettä): Toteuta yksinkertainen älypuhelinsovellus sovelluksesi keräämien tietojen näyttämiseen/käyttämiseen tai muokkaamiseen.</p>
-->

<p>
  <strong>Koodit ja dokumentaatio GitHubiin</strong> (2 pistettä):
  Käytä GitHub-palvelua koodin versionhallintaan.
  Lisäpiste: jaa koodi avoimella lisenssillä.
  Toinen lisäpiste: kontribuoi olemassa olevaan projektiin.
</p>

<p>
  <strong>WebGL ja 3D</strong> (2 pistettä):
  Toteuta sovellukseesi WebGL-rajapintaa hyödyntävä ominaisuus,
  esimerkiksi
  <a href="https://threejs.org/examples/">Three.js-kirjastoa</a>
  hyödyntävä 3D-toiminnallisuus.
</p>

<p>Erityisen hyödyllisiksi osoittautuvat opiskelijoiden toteuttamat ohjeet palkitaan porkkanapistein. Tarjolla on yhteensä 6 pistettä, jotka lisätään kaikkien muiden kerättyjen pisteiden päälle.</p>

<h2 id="raportointi">Harjoitustyön raportointi</h2>

<p>Harjoitustyöpisteet kerätään julkaisemalla toteutuskerran Slackissä tiivis kuvaus toteuttamastasi toiminnosta. </p>

<p>Yksittäiseen ominaisuuteen liittyvän viestin tulee sisältää seuraavat pääkohdat:</p>
<ol>
<li>tiivis kuvaus toteutuksesta,</li>
<li>muutamia otteita toteutuksesta (ohjelmakoodista, asetustiedostoista, ...),</li>
<li>listaus (siis lista linkkejä) ohjeista tai esimerkiksi verkkolähteistä jotka olivat erityisesti hyödyksi tehtävää tehdessä ja</li>
<li>listaus vähintään kolmesta asiasta, jotka olivat valitulla teknologialla joko erityisen helppoja tai vastaavasti hankaloittivat työtäsi merkittävästi.</li>
</ol>
<p>
  Kun viesti on valmis, julkaise se Slackissä.
  Halutessasi voit kirjoittaa kuvauksen esimerkiksi <a href="https://dillinger.io/">dillinger.io</a>-palvelulla ja liittää sen Slackiin-viestiin PDF-muodossa. Mikäli mahdollista, voit julkaista koko kuvauksen sellaisenaan Slack-kanavalle.
</p>
<p id="teknologiatagi">
Kuvauksen mukainen viesti on toimitettava Slackiin viimeistään perjantaina kello 17 mennessä sillä viikolla, joilloin kyseisestä ominaisuudesta jaetaan pisteet: kirjoita viesti ominaisuuteen liittyvälle kanavalle ja lisää siihen sopivat hashtagit:
  #django,
  #nodejs,
  #react,
  #vue,
  #angularjs,
  #rubyonrails,
  #codeigniter,
  #lavarel,
  #flask,
  #firebase,
  #pylons,
  #turbogears
  ja/tai
  #dotnet.
<!--   ja osoita viesti Ohjelmallinen sisällönhallinta -ryhmälle (Valitse Ryhmät &gt; Näkyvyys &gt; Ohjelmallinen sisällönhallinta 2016).
 --></p>

<h2 id="loppuraportti">Loppuraportti</h2>
<p>
<!--  Harjoitustyön palautus tapahtuu lähettämällä oheisen mallin mukainen tiedote osoitteeseen <a href="mailto:katja.kujala@tuni.fi">katja.kujala@tuni.fi</a>.
  Lähetä viesti otsikolla #OHSIHA: työ valmis <em>perjantaihin 3. toukokuuta kello 17 mennessä</em>.
</p>
<blockquote>
  <p>
    Nimi: James Station<br />
    Opiskelijanumero: 234567<br />
    Sähköposti: <a href="mailto:jstat@trolleywatch.org">jstat@trolleywatch.org</a>
  </p>
  <p>Harjoitustyöni aihe: Verkkopalvelu raitiovaunubongareille</p>
  <p>Harjoitustyö löytyy kokonaisuudessaan oheisesta zip-paketista (ohsiha2018-234567.zip).</p>

<p>Korvaan tenttisuorituksen luentopäiväkirjalla. Osoite luentopäiväkirjaani: <a href="https://blog.fi/jamesstation/ohsiha2020">https://blog.fi/jamesstation/ohsiha2020</a></p>
</blockquote>
<p>
Palautettavan zip-paketin (ohsiha2020-opiskelijanumero.zip) tulee sisältää hakemisto nimeltä ohsiha2018-234567 (korvaa lukusarja 234567 omalla opiskelijanumerollasi), jonka sisältä löytyvät työhösi liittyvät koodi- ja asetustiedostot.
Huomaa, että sovelluksen ei tarvitse toimia sellaisenaan. Riittää, että paketin sisältöön voi perehtyä suoraviivaisesti paketin purkamalla.
</p>
<p>Kurssin alussa annetuista ohjeista poiketen pisteitä ei tarvitse merkitä itse mihinkään.
</p>
-->

Loppuraportti palautetaan <a href="https://moodle.tuni.fi/mod/assign/view.php?id=241945">Moodle-sivuilla olevaan palautusautomaattiin</a>. Loppuraportilla on aikaa palauttaa keskiviikkoon 29. huhtikuuta kello 17 asti.

<!--
<p>
Merkitse lisäksi harjoitustyön eri ominaisuuksien raportoiduista toteutuksista keräämäsi pisteet <a href="https://tuni-my.sharepoint.com/:x:/g/personal/katja_kujala_tuni_fi/EckNaAYrqEdIspI3TjSRWy8BMMZCDmLi9su81-YFV1mP-A?e=79pCf3">laskentataulukkoon.</a><strong>Merkitse pisteet ainoastaan siinä tapauksessa, että olet julkaissut kuvauksen määräaikaan mennessä.</strong>
</p>
<!--
<a href="https://docs.google.com/spreadsheets/d/1z9Xt7bVxSnmarJ2XcVWOfJ9QYkMaJZNu80_SFqq7aUw/edit?usp=sharing">Google-laskentataulukkoon</a> (ei edellytä sisäänkirjautumista).-->
