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
* naslov, leto in sezono izida
* dolžino(št epizod x dolžina epizode), opis in žanre
* "glasovne igralce" in režiserje
* MyAnimeList oceno, starostno oceno
* število glasov
* Studije, Lokalizatorje
* Vir (Ali je adaptacija mladinskega romana, stripa, ali originalna zgodba)

Delovne hipoteze:
* Ali je zlata doba animejev že mimo, ali se šele začenja?
* Ali obstaja kakšen vzorec v spremembi prevladovanja določenega žanra v posameznem desetletju?
* Ali so originalni animeji bolj uspešni kot adaptirani?
* Ali so serije namenjene odraslim gledalcem bolj uspešne od tistih, ki so namenjene mlajšim?
