# PUMA
Prospecting the Urban Mines of Amsterdam

Ontwikkeld in het kader van het project Prospecting the Urban Mines of Amsterdam [PUMA](http://www.ams-institute.org/solution/puma/) door Leiden University, Institute of Environmental Sciences; Delft University of Technology, Faculty of Architecture and the Built Environment; Metabolic Amsterdam & Waag Society.

### Kaart

De live versie is beschikbaar op: [code.waag.org/puma](http://code.waag.org/puma) en is gebaseerd op de [gebouwenkaart](code.waag.org/puma).


### Berekening

Voor de inschatting van het gewicht aan staal en koper wordt gebruik gemaakt van het model zoals beschreven in
'[PUMA – from building to urban mine (2016)](http://amsdatahub.waag.org/browser#search=kou&type=paper&item=39286)'
Van Koutamanis et al.

Dit stappenplan resulteert per adres (vbo) in een ordinale score A:

* A(s) = score staal
* A(k) = score koper

Per adres (vbo) wordt hier een minimum en maximumwaarde in kilogrammen aan toegekend:

* Pa(s-) = Puma minimum kilo staal per adres
* Pa(s+) = Puma maximum kilo staal per adres
* Pa(k-) = Puma minimum kilo koper per adres
* Pa(k+) = Puma maximum kilo koper per adres

Deze waarden per adres (vbo) worden voor de kaart opgeteld per gebouw (pand) en gedeeld door de voetafdruk (oppervlakte) van het gebouw (pand), wat leidt tot:

* Pg(s-) = Puma minimum kilo staal/pand
* Pg(s+) = Puma maximum kilo staal/pand
* Pg(k-) = Puma minimum kilo koper/pand
* Pg(k+) = Puma maximum kilo koper/pand


### Data

De gebruikte data komen uit:

* [BAG](http://amsdatahub.waag.org/browser#search=bag&item=39915)
* [AHN](http://amsdatahub.waag.org/browser#search=ahn&item=39371)

Er zijn drie bestanden die de berekening en resultaat voor Amsterdam geven:

Scores én kilogrammen per adres voor Amsterdam:

* [puma adressen ams.csv](/data/puma_adressen_ams.csv)

Oppervlakte (voetafdruk) en kilogrammen per pand (gevisualisseerde data):

* [puma panden ams.csv](/data/puma_panden_ams.csv)

Totaal kilogrammen per stadsdeel (alleen voor Amsterdam):

* [puma buurt ams.txt](/data/puma_buurt_ams.txt)
