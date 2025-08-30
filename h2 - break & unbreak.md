
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
* Raporttia kuuluu kirjoittaa tehtävää tehdessä tuoreeltaan.
* Raportti kuuluu tehdä siistiksi ja helppolukuiseksi.
* Kerrotaan täsmällisesti mitä on tehty ja millä koneella.
* Ei missään nimessä saa plagioida ja lähteet kuuluu merkitä.

## a) Murtaudu 010-staff-only. Ks. Karvinen 2024: Hack'n Fix
### Tehtävät tehtiin Kalissa vmware virtuaalikoneesssa (valmiiksi luotu vm Kalin nettisivulta)
1. avasin termiknaalin Kalissa ja laitoin sudo apt-get update ja sitten sudo apt-get -y install wget unzip micro
2. wget https://terokarvinen.com/hack-n-fix/teros-challenges.zip ja unzip teros-challenges.zip
3. cd challenges/010-staff-only/
4. python3 staff-only.py
5. ctrl+c to quit ja sitten sudo apt-get -y install python3-flask python3-flask-sqlalchemy
6. uudelleen python3 staff-only.py
7. tuli linkki osoitteeseen http://127.0.0.1:5000/
- Nettisivun avattua menin tarkastelemaan pinkoodin syöttökenttää, huomasin että input type oli asetettu numberiksi. Muistin tunnilta sen, että sen voi vain poistaa ja jättää tyhjäksi, jotta lomakkeeseen voi kirjoittaa mitä vain.
- Pidin vuorokauden taukoa kun en osannut ratkaista admin salasanaa.
- Ymmärrän, että kenttään syötetty teksti menee suoraan sql hakuun, mutta en löydä oikeaa tapaa kirjoittaa hakua mikä toimisi.
- Opin, että -- tekstikentän lopussa saa sql haun lopettamaan lopun lukemisen, mikä auttaa asiassa. En silti tiedä miten yhdistäisin haluamani salasanahaun lomakkeen hakuun.
- Selvitin, että UNION yhdistää kaksi hakua samaan, en silti saanut tehtävää millään tehtyä, joten menin lukemaan ratkaisua.
- Ratkaisu olikin ' UNION SELECT password FROM pins--
  - SUPERADMIN%%rootALL-FLAG{Tero-e45f8764675e4463db969473b6d0fcdd}
## b) Korjaa 010-staff-only haavoittuvuus lähdekoodista. Osoita testillä, että ratkaisusi toimii.

## c) Ratkaise dirfuzt-1 artikkelista Karvinen 2023: Find Hidden Web Directories - Fuzz URLs with ffuf. Tämä auttaa 020-your-eyes-only ratkaisemisessa. 

## d) Murtaudu 020-your-eyes-only. Ks. Karvinen 2024: Hack'n Fix

## e) Korjaa 020-your-eyes-only haavoittuvuus. Osoita testillä, että ratkaisusi toimii.



# Lähteet
* Tiivitettävät:
  - [OWASP: OWASP Top 10](https://owasp.org/Top10/A01_2021-Broken_Access_Control/)
  - [Karvinen 2023](https://terokarvinen.com/2023/fuzz-urls-find-hidden-directories/)
  - [PortSwigger](https://portswigger.net/web-security/access-control)
  - [Karvinen 2006](https://terokarvinen.com/2006/raportin-kirjoittaminen-4/)
* Muut tehtävien linkit: 
  - [Hack'n Fix](https://terokarvinen.com/hack-n-fix/)
  - []()
