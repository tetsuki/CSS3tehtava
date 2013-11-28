CSS3 Media Query
================
RYHMÄ: Pekka Virtanen, Eeva Haataja

URL:https://dl.dropboxusercontent.com/u/105512596/css3/toinen/index.html

[HTML-koodi](/index.html)

[CSS-koodi](/tyyli.css)
Responsive Design Basics - Kysymykset
------------------------
Responsiivinen web-design tarkoittaa käyttäjänlaitteisiin sopeutuvaa designia. Käytännössä, käytät sitten tietokonetta, älypuhelinta tai tablettia, web-sivun oleellinen informaatio ja käytettävyys säilyy. Luodaan vain yksi sivu ja sisältö, mutta design säilyy käytetään sitten mitä laitetta hyvänsä.
* Kaikki suhteutetaan laitteeseen prosentteina(%).
* Luodaan mediakyselyt (Media quaries).
* Käytetään eri kuvia eri näyttöformaateille, sekä käytetään korkeus/leveys arvoja niin että ne mukautuu aktiivisesti.

1. Fluid Grid tarkoittaa joustavaa web-sivun asemointia ja sitä että web-sivun elementtejä ei sitouteta tiettyihin pikselimittoihin, vaan elementtien koko sivulla määräytyy näyttökoon mukaan ja täten elementin kokoa voidaan ilmaista esimerkiksi prosenttiluvulla. Fluid grid tarkoittaa myös sitä, että määrittämällä voidaan kontroloida esimerkiksi tilannetta näytön ollessa pieni. Tämä tarkoittaa sitä että haluttuja kenttiä (esim. kuvia) voidaan poistaa näkyvistä kun kenttä ei enää mahdu näytölle tai on ylittänyt tietyn pisteen.
2. Kuvat eri näyttökoilla voidaan näyttää oikeanlaisina asettamalla kuvat skaalautuviksi(flexible images). Tuossa tapauksessa myös kuvan koot voidaan ilmaista prosenttilukuina. Prosenttiluku on suhde näytön alaan nähden.
3. CSS3 Media Query rooli "mukautuvassa" web-designissa on se, että kyselemällä laitteelta esimerkiksi näytönkokoa voidaan kyselyn tuloksena tarvittaessa muuttaa css tiedostoa. Käytännössä työpöytäkäyttäjille voisi olla oma css tiedosto ja taas mobiilikäyttäjille oma. Tuolloin sisältö toimii paremmin käytettävällä laitteella. Mitattavina/kyseltävinä määreinä esimerkiksi näytönkoko, resoluutio, ja suunta(vaaka/pysty). Lähteeni mukaan vanhanaikainen tapa oli käyttää javascript-koodia joka lukee screen-olion ominaisuuksia tätä varten. Nykyään suositellaan CSS3 mediarajoituksia.

ESIM:
@media only screen and (max-width: 640px) {
/* CSS-koodi tilanteisiin, joissa leveys on enintään 640 pikseliä */
}

TAI:
@media handheld { .. tähän väliin kaikki mobiililaitteisiin liittyvät tyylit }
PITÄISIKÖ KIRJOITTAA YLEINEN LYHYT RAPORTTI TYÖSTÄ OK! mut ei ylisuoriteta?
==================================================
- miten määriteltiin eri päätelaitteille sopivaksi?
- Miten määrityksiä tietyille näyttökoille tehdään, miten koodi rakentuu css:ssä kun pohjalla yleisiä määrityksä koko sivua koskevia määrityksiä?
- HTML-tagit
- Mitä pääpointteja tulisi noudattaa mukautuvassa web designissa?
- Jotain tollasta...???
 
 Aluksi oli hieman hankalaa sillä, kaikki tyylit olivat samassa tiedostossa. Mutta sitten kuin Pekka laittoi desktop.css ja mobile.css tiedostot, joihin ohjattiin sitten html-tiedostossa, sivusto alkoi näyttämään jo säädylliseltä. 
        
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <link rel="stylesheet" media="only screen and (max-width: 400px)" href="mobile.css" />
        <link rel="stylesheet" media="only screen and (min-width: 401px)" href="desktop.css"

 





LG L5 E610
==========

Raportti sivustolla käynnistä.
Tukeeko puhelin Media Querya?
Käyttökokemus?

Puhelimeni tukee Media Querya, mutta välillä sen kanssa ilmenee ongelmia. Syy lienee puhelimen vajaavaisuus. Tämän huomaa siitä ilmestyykö navigointipalkki vai ei. Useinmiten näkyy ja tällöin myös käyttökokemus on miellyttävä. Sivustoa on helpompi lukea kun se on asetettu sopivaksi juuri puhelimelle. Mitään mobiileille tarkotettua infoa ei jää huomaamatta ja sivustolla on mukava liikkua vain ylös ja alas. 

Samsung Galaxy S3
=================

Raportti sivustolla käynnistä.
Tukeeko puhelin Media Querya?
Käyttökokemus?

Sivusto aukeaa matkapuhelimellani css-määrityksen mukaan, joka on luotu pienimille näyttöresoluutioille. Sivulla näkyy mobiililaitteella myös navigointipalkki niinkuin pitääkin. Isoimmilla näkymillä navipalkki on poistettu näkyvistä, koska sitä ei noin pienellä sivulla tarvitse. Sivusto latautuu nopeasti kun ei siinä mitään erikoista ole. Sivustoa on helppo käyttää matkapuhelimella, koska siinä selaaminen tapahtuu vain suuntiin ylös ja ales. Uskoakseni Samsung Galaxy S3 tukee media quarya, koska sama sivusto saadaan css perusteella mukautettua sekä työpöydälle että mobiililaitteen ruudulle. Puhelin tunnistaa css:ssässä oleviä näyttökoko määritteitä.

