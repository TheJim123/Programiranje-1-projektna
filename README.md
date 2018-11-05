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
* naslov in leto izida
* dolžino(št epizod) in tip (film ali serija)
* MyAnimeList oceno
* število glasov/ogledov

Delovne hipoteze:
* Ali je zlata doba animejev že mimo, ali se šele začenja?
* Ali so bolj popularni animirani filmi, ali serije?
* Kako dolžina serije vpliva na njen uspeh?
* V kakšnem razmerju sta število ogledov in MyAnimeList ocena?
