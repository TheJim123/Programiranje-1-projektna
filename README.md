# Programiranje-1-projektna
## Projektna naloga pri predmetu Programiranje 1
### Najbolj popularni animeji
Za to projektno nalogo bom zajel prvih 3000 najbolj popularnih animejev, rangiranih glede na sledečo formulo:
* S = Povprečna ocena za anime (mediana).
* v = Število glasov/ocen za anime = (št. ljudi, ki je ocenilo anime).
* m = Minimalna količina glasov/ocen, ki je potrebna za izračun vrednosti (trenutni minimum je 50 ocen).
* C = Povprečna ocena preko cele baze podatkov.
* Weighted Rank (WR) = (v / (v + m)) * S + (m / (v + m)) * C

Podatke bom pobral s strani [MyAnimeList](https://myanimelist.net/topanime.php)

Za vsak film bom zajel:
* rang (dodal naknadno, a se zdi smiselno to imeti)
* id 
* naslov in leto izida
* dolžino(št epizod) in tip (film ali serija)
* MyAnimeList oceno
* število glasov/ogledov

Delovne hipoteze:
* Ali je zlata doba animejev že mimo, ali se šele začenja?
* Ali so bolj popularni animirani filmi, ali serije?
* Kako dolžina serije vpliva na njeno popularnost?
* V kakšnem razmerju sta število ogledov in MyAnimeList ocena?

Za pridobitev in obdelavo podatkov sem uporabil kodo, ki jo je profesor Pretnar pripravil za predavanja.

Kako uporabljati repozitorij:
Za prenos spletnih strani, s katerih sem črpal podatke je treba pognati koda.py, ki bo poleg tega vse zbrane podatke tudi uredila v csv datoteko. Pri prenosu html zapisov strani se mi je večkrat zgodilo, da nekaterih strani ni pravilno preneslo, zaradi napake "Too many requests", zato tudi prilagam vse pravilno prenešene htmlje in pa že sestavljen csv. Poleg tega nekatere serije nimajo končnega števila epizod, saj se še niso končale. Pri teh, regularni izraz ni mogel zajeti števila epizod, zato sem sam poiskal trenutno število in ga dodal v html na primerno mesto, da je program lahko lepo izvedel kar je moral. V enem primeru sem moral poiskati tudi leto izida, saj le tega ni bilo na strani.

Projektna naloga se nahaja v datoteki Projekt.ipynb
