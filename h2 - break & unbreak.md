
## x) Lue/katso/kuuntele ja tiivistä.
### OWASP: OWASP Top 10: A01 Broken Access Control
* Access controllilla yritetään estää pääsy luvattomilta tahoilta, mutta sen voi rikkoa eri tavoin jos sovelluksen ylläpitäjä ei ole huolehtinut asiasta.
* Access controllin voi ohittaa joissain eri tapauksissa esimerkiksi joillain näistä:
  * API kutsut, url osoitteet, keksit ja tokenit
### Karvinen 2023: Find Hidden Web Directories - Fuzz URLs with ffuf
* Artikkelissa esitellään Fuff työkalu, URL osoitteiden fuzzeri. Työkalu käyttää ladattavien sanakirjojen listalta erilaisia URL osoitteisiin laitettavia sanoja löytämään piilotettuja hakemistoja.
* Fuff mahdollistaa mahdollisten tulosten monipuolisen suodattamisen.
### PortSwigger: Access control vulnerabilities and privilege escalation
* On vertikaalista ja horisontaalista access controllia.
  * vertikaalissa on eri ryhmiä joilla on oikeuksia riippuen heidän asemastaan. Admin on korkeammalla kuin mitä normaali käyttäjä olisi.
  * horisontaalisessa esimerkiksi käyttäjät ovat kaikki samalla rivillä oikeuksien suhteen, mutta eivät voi nähdä toistensa tietoja. Esimerkiksi pankkitilit tai verkkokaupan tilaushistoria.
### Karvinen 2006: Raportin kirjoittaminen
* 

## b) hh
hh

## c) hh

### Mikään ohjelmisto ei ole täysin tietoturvallinen.
Niinkuin Kokkola sanoi, niin mikään ohjelmisto ei tosiaan ole täysin tietoturvallinen. Omasta mielestä näkisin myös lisänä sen, että jos jokin ohjelmisto olisikin täysin tietoturvallinen, niin ajan kuluessa kuitenkin ohjelmiston tietoturvallisuus alkaa laskemaan. Tosin siihen pisteeseen pääseminen, missä jokin olisi täysin tietoturvallinen, on varmaan todella mahdotonta päästä nykyteknologialla.

### Hallinnollinen tietoturva on teknisen tietoturvan onnistumisen edellytys.
Tasapaino on tärkeää, että molemmat hoidetaan oikeissa määrin ja ymmärretysti.

### Automaatiotestaus on ohjelmiston tietoturvan kannalta erittäin tärkeää.
Tulevaisuudessa se voisi olla merkittävämpää jos tekoäly pystyisi tekemään luotettavasti testausta. Tällä hetkellä se ei olisi luotettavaa, niin olen samaa mieltä Kokkolan kanssa että automatisointi pitäisi ensin rakentaa ja silloin se on yhtä hyvää kuin itse koodaaja on ollut.

### Ohjelmistoa suunniteltaessa voidaan tehdä paljonkin käyttäjän auttamiseksi tietoturvalliseen toimintaan, mutta nämä toimenpiteet vaikuttavat usein negatiivisesti käytettävyyteen.
Olen itsekin kokenut asiaa. Esimerkiksi salasanan luomisessa jotkin sivustot estävät salasanan copypasten. Käytän salasanamanageria ja mikään ei ole ikävempää kuin yli 15 merkkiä pitkän salasanan kirjoittaminen manuaalisesti. Tavallaan tässäkin asiassa pitää löytää toiminnallisen ja tietoturvallisen väliltä hyvä keskitie.


### Ohjelmiston tietoturvallisuuden suunnitteluun vaikuttaa paljon se, kuinka arkaluonteisia tietoja ohjelmistolla on tarkoitus käsitellä.
Mitä arkaluotoisempaa niin sitä tietoturvallisempi ohjelmiston täytyy olla, luultavasti ihan lainsäädännön mukaan myös.

### Ohjelmistokehittäjät näkevät omat ohjelmistonsa aina merkittävästi riskialttiimpina kuin muiden tekemät ohjelmistot.
Ei varmasti aina, mutta osaava tyyppi varmasti ymmärtää ja näkee enemmän riskejä kuin aloitteleva koodari.

## d) 
#### 1. Ympäristön kuvaus
  - Y

# Lähteet
* Tiivitettävät:
  - [OWASP: OWASP Top 10](https://owasp.org/Top10/A01_2021-Broken_Access_Control/)
  - [Karvinen 2023](https://terokarvinen.com/2023/fuzz-urls-find-hidden-directories/)
  - [PortSwigger](https://portswigger.net/web-security/access-control)
  - [Karvinen 2006](https://terokarvinen.com/2006/raportin-kirjoittaminen-4/)
* hh: 
  - []()
