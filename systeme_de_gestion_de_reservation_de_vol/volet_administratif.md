## Volet Administratif
Les besoins fonctionnels du volet administratif du système de gestion de réservation de vol

### Création, modification et suppression d'aéroports
Identification de l'aéroport: 3 lettres **uniques**, situé dans une ville dans le monde. <br>
Exemples: YUL (Montréal), LAS (Las Vegas), LAX (Los Angeles), BCN (Barcelone), etc.

### Création, modification et suppression de compagnies aériennes
Identification de compagnie aérienne: Par moins de 6 caractères **uniques** à chaque compagnie.

### Création, modification et suppression de vol
Un vol est associé à une **compagnie aérienne**, partant d'un **aéroport d'origine** jusqu'à un **aéroport de destination**, à une **date** et **heure de départ**. <br>
Identification d'un vol est fait par un *ID* qui commence par **2 lettres** suivi d'une **série de chiffres**, unique à chaque compagnie. <br>
Contrainte: l'aéroport de départ et d'arrivé d'un vol doit être différent. 

### Création de sections d'un avion
Exemples de sections: <br>
- Première (F)
- Affaire (A)
- Économique Premium (P)
- Économique (E) <br>
-> Un avion contient 0 ou plus de sections <br>
-> Un avion comporte des sièges organisés en max 100 rangées et 10 colonnes <br>
Identification de siège: Sa section (F, A, P, E), son numéro de rangée(1 à 100) et de colonne (A-J)<br>
Exemples: E56A, A34B <br>
Il y a 4 possibilités au soin d'une section : <br>
- Étroit (S) : trois colonnes avec une aile entre les colonnes 1 et 2 <br>
0|0|0
- Confort (C) : quatre colonnes avec une aile entre les colonnes 2 et 3 <br>
00|00
- Moyen (M) : six colonnes avec une aile entre 3 et 4 <br>
000|000
- Large (L) : dix colonnes avec une aile entre les colonnes 3 et 4, et entre 7 et 8 <br>
000|0000|000 <br>

### Assignation des prix
-> Tous les sièges d'une même section ont le même prix. <br>
F: 100% du plein tarif <br>
A: 75% du plein tarif <br>
P: 60% du plein tarif <br>
E: 50% du plein tarif <br>

### Consultation
Le système affiche tous les vols qui partent et qui arrivent à un aéroport en montrant tous les détails de chaque vol. Le système affiche tous les vols effectués par une compagnie aérienne en montrant tous les détails de chaque vol.
s