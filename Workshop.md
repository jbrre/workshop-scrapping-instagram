# Workshop Scraping Instagram
## Installation
Pour ce Workshop, vous aurez tout d'abord besoin de Python3 et son gestionnaire de paquets, pip3.

    man google

Une fois tout ceci installé, devrez ensuite installer Instaloader depuis pip3.

    pip3 install instaloader

## Connection à Instagram
Pour réaliser la plupart des exercices dans ce workshop, vous aurez besoin de vous connecter à Instagram depuis Instaloader.
**Attention**
A titre personnel, bien que n'ayant jamais été  n'ayant jamais été tempban d'Instagram, j'ai toutefois déjà reçu des demandes une fois revenu sur l'application mobile afin de certifier que je suis bien 100% humain après de gros scrappings. Afin d'éviter que la co d'Epitech soit flag comme un serveur proxy de scrapping, je vous conseille très fortement de réaliser les étapes suivantes sur votre partage de connexion et de ne pas trop scrapper, ou tout du moins d'espacer vos requêtes.

    instaloader --login username
Une fois ceci rentré, l'application vous demandra votre mot de passe et stockera votre token de connexion dans `~/.config/instaloader/session-YOUR-USERNAME`.

## Exercices
[Documentation de l'application ici](https://instaloader.github.io/)
### Exercice 1 : Nombre de likes
Un petit filou a caché son nombre de likes. Je le soupçonne d'acheter des abonnés. Pourriez-vous me dire combien il a eu de likes sur sa dernière photo ?
https://www.instagram.com/jbrre31/

### Exercice 2 : Télécharger des photos
J'aurais besoin de l'intégralité des photos du BDS. Pourriez-vous me les télécharger ?
https://www.instagram.com/bds_epitech_tls/

### Exercice 3 : Echantillon
Il me faudrait un échantillon des likes sur la dernière photo de CR7, mais il en a beaucoup trop ! Pourriez-vous en prendre disons une centaine ?
⚠️ `islice`
https://www.instagram.com/cristiano/

### Exercice 4 : Un code un peu plus complet
Vu que vous semblez maîtriser un peu mieux ce logiciel, j'aurais de vous besoin de savoir si les followers du BDE suivent également l'Instagram du BDS. Faites-moi donc un script qui, pour un nombre donné d'abonnés du BDE, dit s'ils suivent le BDS, ne le suivent pas, ou si vous n'avez pas accès à leur données.
![rendu attendu](https://i.imgur.com/FXIhTnI.png)
https://www.instagram.com/bde_epitech_toulouse/

### Exercice 5 : Un code beaucoup plus complet
Il est temps de passer à de vraies situations de scrapping ! Une agence de marketing cherche une influenceuse pour promouvoir des produits beauté, et cherche un profil suivi majoritairement par des femmes. Faites un script qui permet de récupérer les noms d'utilisateur et nom affiché (full_name) des followers d'un compte ou des likes d'une photo, et comparez-là à une namelist afin d'obtenir un pourcentage.
⚠️*les namelists étant en Anglais, je vous conseille vivement de choisir un profil suivi majoritairement par des Anglophones pour ce test*
![rendu attendu](https://i.imgur.com/fL0Hdt7.png)

### Exercice 6 : Aller plus loin
Si vous êtes arrivés jusque là, pourquoi ne pas aller plus loin ?
Essayez donc de faire l'exercice ci-dessus avec une namelist Française, ou de coder un parser qui prend en compte les prénoms partiels (qui sont souvent mis en nom d'utilisateur ou en nom affiché, exemple "Chlo" au lieu de "Chloé").
Ou alors, pourquoi ne pas coder un script permettant d'afficher les relations entre les followers sous forme d'un graphe ?
[Article sympa sur les relations entre utilisateurs sur les RS](https://www.slate.fr/life/71625/cartographie-des-reseaux-sur-facebook)
Les possibilités sont infinies, vous avez énormément de moyens de vous amuser.
