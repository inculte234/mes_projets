Planning en Association Intermédiaire
=========================

Le fichier Google Sheets "Planning en Association Intermédiaire" permet de renseigner et suivre le planning d'intervention d'agents d'association intermédiaire. Il est pensé pour être un espace unique où les chargé.e.s de mise à disposition renseignent les missions, affectent les salarié.e.s. Un certain nombre d'outils permettent de faciliter ce travail. 

Démarrer l'utilisation
--------------
Le fichier fonctionne avec des onglets où l'on renseigne des informations primaires (en vert foncé), des onglets d'affichage (en jaune), et des onglets d'informations complémentaires (en vert clair)

Il est impératif de renseigner les onglets vert foncé en premier et dans cet ordre : 
- créer le salarié
- créer le client
- créer la mission

Ainsi, si une nouvelle mission nécessite un nouveau salarié, il faut créer le salarié avant la mission. 

**L'onglet "mission" ne peut être renseigné correctement que si l'onglet "client" et l'onglet "salarié" est correctement renseigné au préalable.**

Pour une utilisation optimale, il est recommandé d'utiliser aussi les deux onglets vert clair (formation et métier)

Onglet Salariés
--------------
L'onglet "Salariés" permet de renseigner les agents pouvant intervenir pour des missions. 

- Se rendre sur la **première ligne vide**
- Renseigner un **nom complet** dans la colonne *"Nom"*
- Cocher ses **disponibilités**  
  C’est une étape importante. Il s’agit des disponibilités *« en général »*, définies avec le/la salarié lors de son recrutement.
- Éventuellement, ajouter les **formations suivies**  
  (si l’onglet *"Formation"* a été paramétré au préalable)
- Éventuellement, ajouter les **profils métiers**  
  (si l’onglet *"Métiers"* est utilisé)

Onglet Clients
-------------
L'onglet "Clients" permet de renseigner les clients de l'Association Intermédiaire. 

Pour créer un nouveau client : 
- Se rendre sur la **première ligne vide**
- Renseigner un **nom complet** dans la colonne *"Nom"*
- Indiquer ses éventuelles spécificités (adresse, numéro de téléphone de contact, ou autres)

Onglet Missions
-------------
L'onglet "Missions" permet de créer des missions, de les affecter à des salariés

**Pour créer une nouvelle mission :** 
- Ecrire dans la première ligne vide de l'onglet. Il est recommandé de ne pas tenter d'insérer de nouvelles lignes. 
- Choisir le client. Si le client n'existe pas encore, le renseigner dans l'onglet "Clients"
- Choisir le type de mission (si l'onglet "Métiers" est utilisé)
- Renseigner une Date et heure de début d'intervention. La date doit être au format JJ/MM/YYYY HH:MM:SS. C'est à dire que le 02 décembre 2025 à 9h sera renseigné de la manière suivante  02/12/2025 09:00:00. 
- Renseigner de la même façon une Date et une heure de fin d'intervention
- Renseigner le total du temps de pause sur le temps de la mission. 
- Eventuellement, on peut également renseigner, en colonne R, des commentaires additionnels pour préciser la demande (le client demande une tenue particulière, précise une adresse de rdv particulière, etc)

**Pour affecter la mission à un salarié** 
- Choisir un intervenant. La liste des intervenants qui s'affiche est celle des intervenants disponibles normalement sur ces créneaux (grâce aux informations renseignées dans l'onglet "Salariés")

S'affichent dans les colonnes M N et O des informations importantes pour s'assurer que l'affectation est pertinente : 
- La colonne "Avertissement compétences" indique si le salarié correspond au profil métier (grâce aux informations renseignées dans l'onglet "Salariés")
- La colonne "Avertissement dispo" indique si le salarié est déjà affecté à une mission sur le même créneau horaire. 
- La colonne "Avertissement formation" indique si le salarié a bien suivi la formation demandée par le client (Grâce aux informations renseignées dans l'onglet "Formation" et dans l'onglet "Salariés")

Onglet Métiers
-------------
L'onglet "Métiers" permet de lister les métiers pour lesquels l'Association Intermédiaire peut faire des missions. 
Pour créer un nouveau métier, le renseigner dans la première ligne vide disponible de la colonne A. 

Onglet Formations
--------------
L'onglet "Formations" permet de lister les formations disponibles pour les salarié.e.s de l'Association, et de les associer à des clients.

Pour créer une nouvelle formation : 
- en Colonne A, nommer la formation 
- en Colonne B, l'associer à un client (il faut que le client ait, au préalable, été créé dans l'onglet "Clients")

Vous pouvez ensuite aller dans l'onglet "Salariés" pour ajouter les formations suivies par les salarié.e.s. POur cela : 
- dans la colonne AD, sélectionner les formations suivies par chaque salarié.e

Onglet Planning intervenant
-------------
L'onglet "Planning Intervenant", permet de visualiser le planning individuel d'un salarié.

Pour générer le planning d'un intervenant, il faut simplement modifier les variables en jaune : 
- Sélectionner le nom de l'intervenant
- Sélectionner la date de début du planning que l'on veut générer. Vous pouvez double-cliquer sur la cellule pour afficher un petit calendrier cliquable. 
- Sélectionner la date de fin du planning que l'on veut générer. Vous pouvez double-cliquer sur la cellule pour afficher un petit calendrier cliquable. 

Le planning se génère ensuite dans le reste des cellules. 

Vous pouvez l'exporter au format PDF. Dans le menu en haut, cliquer sur sur "Fichier", puis "Télécharger" et "PDF"

Onglet Planning Client
-------------
L'onglet "Planning Client", permet de visualiser le planning individuel d'un client.

Pour générer le planning d'un client, il faut simplement modifier les variables en jaune : 
- Sélectionner le nom du client
- Sélectionner la date de début du planning que l'on veut générer. Vous pouvez double-cliquer sur la cellule pour afficher un petit calendrier cliquable. 
- Sélectionner la date de fin du planning que l'on veut générer. Vous pouvez double-cliquer sur la cellule pour afficher un petit calendrier cliquable. 

Le planning se génère ensuite dans le reste des cellules. 

Vous pouvez l'exporter au format PDF. Dans le menu en haut, cliquer sur sur "Fichier", puis "Télécharger" et "PDF"

