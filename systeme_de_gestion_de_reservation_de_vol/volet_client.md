## Volet Client
Les besoins fonctionnels du volet administratif du système de gestion de réservation de vol

### Vérification des vols disponibles
Le client peut rechercher tous les vols d'un aéroport d'origine à une destination avec des sièges libres, à une date donnée, pour une classe donnée. Le système affiche la liste des vols avec le détail pour chacun : **date** et **heure de départ**, **durée du vol**, **heure d'arrivée**, **compagnie aérienne numéro du vol**, **prix**, **nombre de sièges disponibles pour la section.**

### Réservation de siège
Le client peut réserver un siège disponible dans un vol donné. Il a l'option de **choisir une priorité entre l'aile ou la fenêtre**. Un numéro de réservation est fourni au client. <br>
Contrainte: Un siège réservé n'est plus disponible à un autre passager. <br>
Un siège est **réservé pendant 24 heures**, après quoi il redevient disponible.

### Paiement d'un siège
Le client peut payer pour son siège réservé avec le numéro de réservation. <br> 
Le client entre ses informations personnelles : **noms**, **adresse**, **courriel**, **téléphone**, **date de naissance**, **numéro de passeport**, **date d'expiration de passeport**. <br> 
Le paiement d'un siège est effectué par **carte de crédit**. <br>
Une confirmation de paiement est produite. <br>
Un siège réservé devient assigné à un passager une fois payé. Le siège est donc confirmé.

### Annulation et changement de réservation
Le client peut changer sa réservation pour un autre vol complètement différent. <br>
*Si le siège est confirmé*, le client ne peut changer que la **date et l'heure du vol sans frais**. <br>
Un client peut changer la classe du siège. <br>
Si c'est pour un **upgrade**, ce dernier devra payer la différence. <br>
Si c'est pour un **downgrade**, ce dernier se vera rembourser la différence moins 10% de la différence. (prix tarif plein = 100$, et il faut avoir économique, alors il va se faire rembourser 100 * 0.5 - (100 * 0.5) * 0.1 = 45$).
