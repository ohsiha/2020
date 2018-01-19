# Teknologiademo 1 (HTML & CSS, Django) #

## Editorit ja selaimet ##

Web-sovellusten kehitykseen tarvitaan tekstieditori (tai [IDE](https://en.wikipedia.org/wiki/Integrated_development_environment) kuten [Pycharm](https://en.wikipedia.org/wiki/Integrated_development_environment)) sekä selain, jolla voidaan seurata muutoksia.

Päteviä tekstieditoreita ovat
- [Atom](https://atom.io/)
  - Erittäin laaja kirjasto laajennuksia (packages)
  - Toimii Windowsilla, Macilla ja Linuxilla
  - Paras tuki kurssihenkilöstön puolesta
- [Sublime Text](https://www.sublimetext.com/)
  - Erillinen kirjasto laajennuksille (https://packagecontrol.io/)
  - Uusin versio Sublime Text 3
  - Toimii Windowsilla, Macilla ja Linuxilla
- [Notepad++](https://notepad-plus-plus.org/)
  - Kevyin vaihtoehto
  - Vain Windowsille

Selaimeksi suositellaan [Google Chrome](https://www.google.fi/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&uact=8&ved=0ahUKEwjYht7zkOTYAhWKkywKHUqBAOIQFggyMAA&url=https%3A%2F%2Fwww.google.com%2Fchrome%2Fbrowser%2Fdesktop%2Findex.html&usg=AOvVaw0XVP3LCM5kL0uPj3LId6gl)-selainta.

## HTML & CSS ##

- HTML (HyperText Markup Language), internetin kuvauskieli
  - Uusin versio HTML5
- CSS (Cascading Style Sheets), HTML:n avuksi tehty www-dokumenttien tyyliohjeiden laji
  - Uusin versio CSS3

HTML:n ja CSS:n dokumentaatioita:
- HTML: [MDN web docs](https://developer.mozilla.org/en-US/docs/Web/HTML) sekä [W3](https://www.w3schools.com/html/)
- CSS: [MDN web docs](https://developer.mozilla.org/en-US/docs/Web/CSS) sekä [W3](https://www.w3schools.com/css/default.asp)

## Python & Django ##

Django on melko yleinen web-sovelluskehityksessä. Mm. Instagram ja Pinterest on kehitetty Djangolla.

Python on melko uusi ja tulkattava ohjelmointikieli. Pythonin vahvuudet ovat sen monikäyttöisyys muun muassa web-sovelluskehityksessä ja datatieteessä. Python on myös "helppo" ohjelmointikieli, jonka syntaksi on melko yksiselitteinen.

### Djangon asennus ###

Hyvä ohjeistus myös [täältä](https://www.codingforentrepreneurs.com/blog/install-python-django-on-windows/). Harkkatyötä ajatellen: Djangon [dokumentaatio](https://docs.djangoproject.com/en/1.11/) on todella hyödyllinen!

Ladattavat komponentit:
- Python 3.x
- pip
- virtualenv
- Django

Django toimii Pythonin päällä. Ensin ladattava Python: https://www.python.org/downloads/. Kannattaa ladata uusin versio, yhteensopivuudet Djangon kanssa näkee [täältä](https://docs.djangoproject.com/en/1.11/faq/install/#faq-python-version-support).

**HUOM Windows-käyttäjät! Varmistakaa, että checkbox on merkattuna kohdassa "Add Python 3.6.4 to PATH"**

Pythonin version näkee Windowsilla C:\Windows\py.exe, Macilla komentoriviltä "python -V".

[Pip](https://en.wikipedia.org/wiki/Pip_(package_manager)) on paketinhallintajärjestelmä Pythonille. Lataaminen Windowsille onnistuu seuraamalla [tätä](https://github.com/BurntSushi/nfldb/wiki/Python-&-pip-Windows-installation#pip-install) linkkiä (huom. Pythonin 3.6.x versiossa Windowsin komentorivillä Pythonin kutsuminen tapahtuu "python" sijaan "py").

Virtualenvin lataaminen onnistuu komennolla *pip install virtualenv*. Tämä on todella hyödyllinen harkkatyötä ajatellen.

Pip-paketinhallintajärjestelmän avulla onnistuu myös Djangon asentaminen komennolla *pip install django*. Varmistus siitä, että Django on ladattu, onnistuu komennoilla *py*, jonka jälkeen *import django* sekä *print(django.get_version())*.
