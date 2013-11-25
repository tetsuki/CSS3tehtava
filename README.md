CSS3 Media Query
================
RYHMÄ: Pekka Virtanen, Eeva Haataja

URL:users.metropolia.fi/~XXXXXX

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

LG L5 E610
==========

Raportti sivustolla käynnistä.
Tukeeko puhelin Media Querya?
Käyttökokemus?

Samsung Galaxy S3
=================

Raportti sivustolla käynnistä.
Tukeeko puhelin Media Querya?
Käyttökokemus?
