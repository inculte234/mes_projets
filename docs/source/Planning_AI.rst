.. _planning-ai:

Planning en Association Intermédiaire
=====================================

Le fichier Google Sheets **« Planning en Association Intermédiaire »** permet de renseigner et de suivre le planning d’interventions des agents d’une Association Intermédiaire.

Il est conçu comme un **espace unique** dans lequel les chargé·e·s de mise à disposition peuvent :

- renseigner les missions,
- affecter les salarié·e·s,
- vérifier les compatibilités (disponibilités, compétences, formations).

Un certain nombre d’outils automatisés permettent de **sécuriser et simplifier ces opérations**.

Une version *« vide »* du planning est disponible pour être clonée ici :  
`Accéder au planning vierge <https://docs.google.com/spreadsheets/d/1cqSDBjjlTyBFWRqXx6UsuNnuQA89VfGCgVA6vOYZch0/edit?gid=0#gid=0>`_


Navigation rapide
------------------

- :ref:`Démarrer l’utilisation <demarrer-utilisation>`
- :ref:`Onglet Salariés <onglet-salaries>`
- :ref:`Onglet Clients <onglet-clients>`
- :ref:`Onglet Missions <onglet-missions>`
- :ref:`Onglet Métiers <onglet-metiers>`
- :ref:`Onglet Formations <onglet-formations>`
- :ref:`Onglet Planning Intervenant <onglet-planning-intervenant>`
- :ref:`Onglet Planning Client <onglet-planning-client>`


.. _demarrer-utilisation:

Démarrer l’utilisation
----------------------

Le fichier fonctionne avec trois types d’onglets :

- des **onglets de données primaires** *(en vert foncé)*,
- des **onglets d’affichage** *(en jaune)*,
- des **onglets d’informations complémentaires** *(en vert clair)*.

Il est **impératif de renseigner d’abord les onglets vert foncé, dans l’ordre suivant** :

1. créer le salarié → :ref:`Onglet Salariés <onglet-salaries>`
2. créer le client → :ref:`Onglet Clients <onglet-clients>`
3. créer la mission → :ref:`Onglet Missions <onglet-missions>`

Ainsi, si une nouvelle mission nécessite un nouveau salarié, **le salarié doit être créé avant la mission**. **L’onglet « Missions » ne peut être renseigné correctement que si les onglets « Clients » et « Salariés » sont déjà complétés.**

Pour une utilisation optimale, il est également recommandé d’utiliser les deux onglets vert clair :

- :ref:`Onglet Formations <onglet-formations>`
- :ref:`Onglet Métiers <onglet-metiers>`


.. _onglet-salaries:

Onglet « Salariés »
------------------

L’onglet **Salariés** permet de renseigner les agents pouvant intervenir sur des missions.

Pour créer un nouveau salarié :

- Se rendre sur la **première ligne vide**
- Renseigner un **nom complet** dans la colonne *« Nom »*
- Cocher ses **disponibilités**  
  C’est une étape essentielle. Il s’agit des disponibilités *« en général »*, définies lors du recrutement.
- Ajouter, le cas échéant, les **formations suivies**  
  (voir :ref:`Onglet Formations <onglet-formations>`)
- Ajouter, le cas échéant, les **profils métiers**  
  (voir :ref:`Onglet Métiers <onglet-metiers>`)


.. _onglet-clients:

Onglet « Clients »
------------------

L’onglet **Clients** permet d’enregistrer les clients de l’Association Intermédiaire.

Pour créer un nouveau client :

- Se rendre sur la **première ligne vide**
- Renseigner un **nom complet** dans la colonne *« Nom »*
- Indiquer les informations utiles  
  *(adresse, numéro de téléphone, particularités, etc.)*


.. _onglet-missions:

Onglet « Missions »
-------------------

L’onglet **Missions** permet de créer les missions et d’y affecter des salarié·e·s.

Créer une nouvelle mission :
^^^^^^^^^^^^

- Écrire sur la **première ligne vide** (ne pas insérer de nouvelle ligne)
- Choisir le **client** (voir :ref:`Onglet Clients <onglet-clients>`)
- Choisir le **type de mission** (voir :ref:`Onglet Métiers <onglet-metiers>`)
- Renseigner la **date et l’heure de début** au format :  
  ``JJ/MM/AAAA HH:MM:SS``. Par exemple la date du 2 décembre 2025 à 9h sera notée : ``02/12/2025 09:00:00``
- Renseigner de la même façon la **date et l’heure de fin**
- Renseigner le **temps total de pause**
- Ajouter, en colonne **R**, des **commentaires complémentaires** si nécessaire

Affecter une mission à un salarié :
^^^^^^^^^^^^
- Choisir un **intervenant** dans la liste proposée  
  (disponibilités issues de :ref:`Onglet Salariés <onglet-salaries>`)

Trois colonnes d’alerte permettent de sécuriser l’affectation :

- **Avertissement compétences** (la formule vérifie que le profil métier renseigné pour la mission correspond au profil métier coché pour le salarié)
- **Avertissement disponibilité** (la formule vérie que le salarié n'est pas affecté deux fois sur deux missions sur le même créneau)
- **Avertissement formation**  (la formule vérifie que le salarié a bien suivi la formation demandée par ce client)

Cas particulier : les missions sur plusieurs jours
^^^^^^^^^^^^

Il est possible de créer des **missions qui s’étalent sur plusieurs jours**, à condition qu’elles respectent **des horaires strictement identiques chaque jour** (même heure de début et même heure de fin) et que les **jours travaillés soient continus**.

**Exemple :**

- Début : Lundi 1er décembre 2025 à 09h00  
- Fin : Vendredi 5 décembre 2025 à 17h00  
- Horaires identiques chaque jour : 09h00 → 17h00  

Dans ce cas précis, **la mission peut être renseignée sur une seule ligne**.

En revanche, **si les horaires varient d’un jour à l’autre**, il est alors recommandé de :

- créer **une ligne par jour de mission**.

.. note::

   Afin d’éviter toute erreur de planification ou de calcul, en cas de doute, 
   **il est fortement recommandé de créer autant de missions qu’il y a de jours**


.. _onglet-metiers:

Onglet « Métiers »
-----------------

L’onglet **Métiers** permet de lister les types de missions que peut proposer l’Association Intermédiaire.

Pour créer un nouveau métier :

- Renseigner son **nom dans la première ligne vide de la colonne A**


.. _onglet-formations:

Onglet « Formations »
--------------------

L’onglet **Formations** permet de :

- lister les formations disponibles,
- les associer aux clients,
- puis aux salarié·e·s.

Créer une nouvelle formation :
^^^^^^^^^^^^

- En **colonne A** : nommer la formation
- En **colonne B** : l’associer à un client  
  (voir :ref:`Onglet Clients <onglet-clients>`)

Ensuite, dans l’onglet **Salariés** :

- En **colonne AD**, sélectionner les **formations suivies par chaque salarié·e**
  (voir :ref:`Onglet Salariés <onglet-salaries>`)


.. _onglet-planning-intervenant:

Onglet « Planning Intervenant »
-------------------------------

L’onglet **Planning Intervenant** permet de visualiser le planning individuel d’un salarié.

Pour générer un planning :

- Sélectionner le **nom de l’intervenant**  
  (voir :ref:`Onglet Salariés <onglet-salaries>`)
- Sélectionner la **date de début**
- Sélectionner la **date de fin**

Le planning se génère automatiquement.

**Export en PDF :**

On peut **exporter en PDF :** le planning en allant dans : Menu **Fichier** → **Télécharger** → **PDF**


.. _onglet-planning-client:

Onglet « Planning Client »
--------------------------

L’onglet **Planning Client** permet de visualiser le planning individuel d’un client.

Pour générer un planning :

- Sélectionner le **nom du client**  
  (voir :ref:`Onglet Clients <onglet-clients>`)
- Sélectionner la **date de début**
- Sélectionner la **date de fin**

Le planning se génère automatiquement.

On peut **exporter en PDF :** le planning en allant dans : Menu **Fichier** → **Télécharger** → **PDF**
