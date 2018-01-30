<h1 style="font-size: smaller;">Resurssikeskeinen arkkitehtuuri</h1>

---
## Lomakkeet ja HTTP    
<p>Lomaketoteutukset kommunikoivat Web-palvelimien kanssa HTTP-protokollalla.</p>

---

## Verkkopalvelu ja toimintojen luonne
   <p>Nykyaikainen Web-arkkitehtuuri (<a href="http://www.w3.org/TR/webarch/"><span>http://www.w3.org/TR/webarch/</span></a>) jakaa verkkopalveluiden toiminnot kahteen luokkaan, <dfn>turvallisiin</dfn> ja <dfn>ei-turvallisiin</dfn>.
   </p>

---


## Turvallinen ja ei-turvallinen

   <ul>
      <li><span>Turvallinen toiminto</span> (safe intercation):
         <ul>
            <li>toiminto vastaa luonteeltaan <span>kyselyä/hakua</span></li>
            <li>toiminnon suorittaminen ei muuta sovelluksen tilaa </li>
         </ul>
      </li>
      <li><span>Ei-turvallinen toiminto</span> (unsafe interaction):
         <ul>
            <li>toiminto vastaa luonteeltaan <em>tilausta</em></li>
            <li>toiminnon suorittamisen seurauksena sovelluksen tila muuttuu: käyttäjän lisätään sähköpostilistalle tai rekisteröidään palveluun,
               toiminnon seurauksena syntyy maksutapahtuma ja niin edelleen.
            </li>
            <li>Huom: ei-turvallinen tarkoittaa tässä eri asiaa kuin vaarallinen (dangerous).</li>
         </ul>
      </li>
   </ul>

---

## Toiminnon luonne &amp; välitystavan valinta

   <p>Selain välittää käyttäjän syötteen palvelimelle HTTP-pyyntönä. Lomakesoveltajan valittavana ovat seuraavat HTTP-metodit:
   </p>
   <ul>
      <li><span>get</span>-metodi:
         <ul>
            <li>turvalliset toiminnot: haku/kysely, sovelluksen tila ei muutu </li>
            <li>kaikki pyyntöön liittyvät tiedot koodataan mukaan URI-tunnisteeseen </li>
         </ul>
      </li>
      <li><span>post</span>-metodi:
         <ul>
            <li>ei-turvalliset toiminnot: tilaus, sovelluksen tila muuttuu </li>
            <li>pyyntöön liittyvät tiedot koodataan HTTP-pyynnön otsikkotietoihin </li>
            <li>käyttäminen perusteltua myös arkaluontoisia tietoja (esim. salasana, yhteystiedot tai luottokortin numero) välitettäessä  </li>
         </ul>
      </li>
   </ul>
   <p>Myös Web-selaimessa näkyviä eroja! Mitä?</p>

---

## Kertaus: Pysyvät URI-tunnisteet

   <p>Huomioi myös URI-tunnisteiden <span>pysyvyys</span> (stability) ja <span>ennustettavuus</span> (predictability):</p>
      <ul>
          <li>Resurssia edustava representaatio URI-tunnisteen on tarjolla ajanhetkestä riippumatta </li>
          <li>Resurssin URI-tunnisteen <a href="http://www.w3.org/Provider/Style/URI">tulee pysyä muuttumattomana</a></li>
          <li>URI-tunniste on sama jakelukontekstista (käyttäjä, käyttötilanne ja päätelaite) riippumatta: representaatio
         räätälöidään jakelukontekstiin sopivaksi</li>
      <li><span><span>HTTP-protokollan </span></span><span><span>get</span></span>-metodi mahdollistaa pysyvien URI-tunnusten toteuttamisen:
         kirjanmerkit, linkit ja välimuistin toiminta.</li>
      <li>Esimerkki: <a href="http://aikataulut.tampere.fi/?key=3525&amp;stop=3525">pysäkin numero 3525 aikataulu</a>. Myös ongelmia! Mitä?</li>
   </ul>

---

## Istunnon hallinta

HTTP-protokollan
tilattomuus on jo tuttua, mutta kerrataanpa vielä:
HTTP-protokollassa ei ole sisäänrakennettua keinoa sovelluksen
tilan ylläpitämiseen.

<ul>      <li>
         Sovelluksen
         tilan ylläpitäminen toteutetaan <dfn>istuntojen</dfn> (session)
         tuella:
         <ul>
            <li>
               Sisäänkirjautuminen
            </li>
            <li>
               Sisällön/toimintojen
               näyttäminen käyttöoikeuksien perusteella
            </li>
            <li>
               Sovelluksen
               <span>mukauttaminen</span> käyttäjän mieltymysten
               (preference) perusteella
            </li>
            <li>
               Käyttäjän
               <span>toiminnan seuraaminen</span>, esimerkiksi
               lokitiedon kerääminen

            </li>
            <li>
               <span>Ostoskorin</span> toteuttaminen
            </li>
         </ul>

   ---

   ## Istunnoista

   <ul>
      <li>
         Huomaa, että
         istuntoja voidaan hyödyntää myös ilman käyttäjän tunnistamista.
         Tällöin sovelluksen tilaa ei kuitenkaan voida säilyttää
         <em>istuntojen välillä</em>.

      </li>
      <li>
         Asiakas-palvelin
         -mallissa istunto toteutetaan siten, että asiakkaalle annetaan
         yksikäsitteinen <em>istunnon tunniste</em>, jonka
         asiakas toimittaa takaisin palvelimelle jokaisen pyynnön
         yhteydessä. Istunnon tiedot säilytetään palvelimella ja niihin
         päästään käsiksi istunnon tunnisteen perusteella.

      </li>
   </ul>

---

## Istunnot käytännössä

   <ul>
      <li>
         Istunnon
         tunnisteen välittämiseen on useita tapoja:
         <ul>
            <li>
               <span>Evästeet</span> (Cookie): Eväste on (lyhyt) merkkijono, jonka
               verkkopalvelu välittää asiakkaalle HTTP-vastauksen mukana. Eväste
               tallennetaan käyttäjän koneelle joko istunnon ajaksi tai pysyvästi
               kovalevylle. Asiakas lähettää evästeen palvelulle jokaisen
               palvelupyynnön mukana. Evästeitä nimitetään usein kekseiksi,
               pipareiksi tai jopa taikapipareiksi

            </li>
            <li>
               <span>HTTP GET:</span> Istunnon tunniste sijoitetaan muiden pyynnön
               parametrien tapaan osaksi URI-tunnistetta (<code>example.php?sessionid=xyz123</code>) =&gt;
               ongelmia!
            </li>
            <li>
               <span>HTTP POST:</span> Istunnon tunniste sijoitetaan HTML-lomakkeen
               piilokenttään.
            </li>
         </ul>
      </li>
   </ul>
   <ul>
      <li>
         Evästeen voimassaoloaika voidaan määritellä evästä asetettaessa. Eväste
         voidaan myös aktiivisesti poistaa siinä vaiheessa, kun istunto
         lopetetaan.

      </li>
      <li>
         Istunnot
         ovat erittäin keskeisessä roolissa verkkopalvelun toiminnallisuuden
         toteuttamisessa. Esimerkiksi yleiskäyttöinen ostoskorin
         toiminnallisuus toteutetaan istuntojen avulla.
      </li>
   </ul>

---

## Pohdinta: SPA ja istunnot

---

## Kohti AJAXia

<p>Kolmikerrosmalli esittelee Web-hypermediajärjestelmän teknisen perustan. </p>
<p>AJAX (Asynchronous JavaScript And XML) mahdollistaa entistä vuorovaikutteisempien sovellusten kehittämisen ja esittelee lisää kerroksia arkkitehtuuriin.</p>
<p>
  Ks. havainnollinen [kaaviokuva AJAX-periaatteesta](http://www.webstepbook.com/supplements-2ed/slides/chapter12-ajax-xml-json.shtml#slide7).
</p>


---

Kohti RESTiä</h1>
  <p>Kolmikerrosmalli esittelee Web-hypermediajärjestelmän teknisen perustan. </p>
  <p>REST (Representational State Transfer) -malli (Fielding 2000) laajentaa ja yleistää mallia kohti hajautettua Web-hypermediaa, vrt.
      </p>
  <p><img src="http://www.ibm.com/developerworks/websphere/library/techarticles/0708_colonnese/images/figure1.jpg" alt="Fielding (2000): REST-mallin prosessinäkymä"/></p>
  <p>Kuva: (Fielding, 2000)</p>
</div>

---

## HATEOS

<blockquote><p>Hypermedia As The Engine Of Application State (HATEOAS) is a constraint of the REST application architecture that distinguishes it from other network application architectures.</p>

<p>With HATEOAS, a client interacts with a network application that application servers provide dynamically entirely through hypermedia. A REST client needs no prior knowledge about how to interact with an application or server beyond a generic understanding of hypermedia.</p>

([Wikipedia: HATEOS](https://en.wikipedia.org/w/index.php?title=HATEOAS&oldid=812361783))

---

# Lopuksi
