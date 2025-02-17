---
icon: message-question
---

# FAQ : toutes les notions (test)

## Synchronisation calendrier

<details>

<summary><strong>Comment recevoir des notifications d’alertes de rendez-vous ?</strong></summary>

<mark style="background-color:purple;">**Cette fonctionnalité permet de recevoir des notifications par email lorsqu’un rendez-vous est ajouté, modifié ou annulé dans un agenda. Elle répond au besoin des agents souhaitant être alertés en cas de changement dans leur planning.**</mark>

Vous pouvez personnaliser vos préférences de notification dans l’onglet **"Mon Compte"**, accessible en cliquant sur votre prénom en haut à droite de votre calendrier.

Chaque email contient une pièce jointe au format **ICS**, compatible avec la plupart des logiciels de calendrier. Votre calendrier externe reconnaîtra automatiquement ces mises à jour, bien que certains logiciels demandent une validation manuelle des modifications.

</details>

<details>

<summary><strong>Comment synchroniser avec mon agenda ?</strong></summary>

**Cette fonctionnalité permet d'envoyer les informations des rendez-vous planifié dans un&#x20;**<mark style="background-color:purple;">**agenda extérieur à RDV Service Public. Elle répond au besoin de faire afficher les rendez-vous planifié dans un agenda du quotidien, souvent utilisé dans les administrations pour gérer leur quotidien métier en dehors des rendez-vous (réunion d'équipe etc ...)**</mark>

#### Notes générales&#x20;

RDV Service Public propose différents mécanismes de synchronisation. Voici quelques remarques importantes valables pour tous les mécanismes :

* Pour protéger les données personnelles de vos usagers, les événements envoyés à votre logiciel de calendrier externe ne contiendront que le motif, l'adresse du rendez-vous et un lien vers les détails dans RDV Service Public ;&#x20;
* Nous proposons de synchroniser les créations, changements et annulations depuis RDV Service Public vers les logiciels de calendrier externes mais pas l’inverse. Si vous supprimez un RDV depuis votre logiciel de calendrier externe, cela ne sera pas répercuté dans RDV Service Public et l’usager n’en sera pas averti.

#### S**ynchronisation par email**

Cette synchronisation envoie un email pour chaque création, modification ou annulation de RDV.&#x20;

Chaque email contient une pièce jointe au format ICS, un format largement supporté. Votre logiciel de calendrier externe reconnaîtra ces emails et mettra automatiquement à jour les évènements dans votre calendrier. Certains logiciels de calendrier demandent « d’accepter » chaque modification.

Vous pouvez modifier vos préférences de notifications email dans l’espace « Mon Compte » accessible en cliquant sur votre prénom en haut à droite depuis votre vue calendrier.

#### **Synchronisation Webcal**

Webcal est un protocole largement supporté par les logiciels de calendrier.&#x20;

Nous vous fournissons une URL individuelle fournissant le contenu de votre agenda au format ICS. Cette URL peut être récupérée depuis dans l’espace « Mon Compte » accessible en cliquant sur votre prénom en haut à droite depuis votre vue calendrier. Il suffit de copier cette URL dans votre logiciel de calendrier externe et la synchronisation se fera automatiquement.

Si vous synchronisez votre agenda RDV Solidarités avec Google Agenda, la mise à jour peut prendre jusqu'à 12 heures. Avec le calendrier Outlook, l'affichage est plus rapide, généralement dans l'heure suivant la prise de rendez-vous.

La synchronisation WebCal n’est pas instantanée. \
\
La fréquence de mise à jour dépend de chaque logiciel de calendrier externe. Avec Google Agenda par exemple, la mise à jour peut prendre jusqu’à 12h. Avec Outlook, cette fréquence est généralement d’environ une heure mais chaque logiciel peut se comporter différemment.

#### Synchronisation spécifique Outlook

Il existe deux grandes versions d'Outlook :&#x20;

* Outlook hébergé à distance, aussi appelé Microsoft 365
* Outlook hébergé sur place par l’administration, aussi appelé Microsoft Exchange

Nous avons un prototype de synchronisation spécifique pour la version hébergée à distance (Microsoft 365). N’hésitez pas à nous contacter si vous souhaitez l’expérimenter sur votre territoire.&#x20;

Nous ne fournissons pour l’instant pas de solution spécifique pour Outlook hébergé sur place (Microsoft Exchange). Certaines structures utilisant RDV Service Public et ce type d’Outlook ont cependant mis en place des solutions via webhooks (voir ci-dessous).

#### Synchronisation via webhooks

Cette solution demande du développement spécifique en interne par votre DSI.

Les webhooks sont une manière de communiquer entre deux systèmes d’information. Nous proposons d’émettre des webhooks vers le SI de votre organisation.&#x20;

Il est possible de développer un logiciel dans votre SI pour recevoir ces webhooks et mettre à jour les calendriers des agents en conséquence. Cette solution est déjà en place dans plusieurs structures utilisant RDV Service Public.

Vous trouverez des informations techniques ici : [https://github.com/betagouv/rdv-service-public/blob/production/docs/api/webhooks/api-notifications-webhooks.md](https://github.com/betagouv/rdv-service-public/blob/production/docs/api/webhooks/api-notifications-webhooks.md)

</details>

## Interopérabilité&#x20;

<details>

<summary><strong>France Titres portail ANTS &#x3C;> Commune avec dispositif de recueil (DR)</strong> </summary>



</details>

<details>

<summary> <strong>Cartographie nationale médiateur numérique &#x3C;> Conseillers Numériques</strong></summary>



</details>

## Prise de rendez-vous en ligne

<details>

<summary><strong>Comment mettre en place de la prise de rende-vous en ligne ?</strong></summary>

<mark style="background-color:purple;">**Cette fonctionnalité permet aux usagers d’accéder aux disponibilités de votre organisation et de planifier un rendez-vous en toute autonomie, depuis un ordinateur ou un téléphone.**</mark>

Pour activer cette option, trois étapes sont nécessaires :

**1. Configurer des motifs ouverts à la réservation en ligne**

Dans les paramètres des motifs, sélectionnez au moins un motif et activez l’option **"Ouvert aux agents et aux usagers"**. Vous pouvez également :

* Définir un délai minimum et maximum de réservation.
* Ajouter des instructions personnalisées dans l’onglet **"Instruction et notification"**.

**2. Configurer une plage d’ouverture**

Créez une plage d’ouverture en y associant des motifs configurés pour la réservation en ligne. Ces motifs sont identifiés par une pastille spécifique dans l’écran de suivi des motifs.

**3. Partager votre URL de prise de rendez-vous**

Un lien URL est disponible dans le menu **"Réservation en ligne"**. Ce lien permet aux usagers et prescripteurs d’accéder directement à vos disponibilités via un navigateur web. Vous pouvez partager cette URL ou l’intégrer dans différents supports, tels que votre site internet ou une plaquette numérique.

</details>

<details>

<summary><strong>Comment les usagers prennent-ils rendez-vous ?</strong></summary>

Les usagers peuvent prendre rendez-vous en ligne si cette option est activée et que vous avez partagé votre lien de réservation. Ce lien peut être diffusé sur votre site web ou tout autre support.

Une fois sur la plateforme, ils pourront :

1. Choisir un service et un motif de rendez-vous.&#x20;
2. Sélectionner un créneau disponible
3. S’identifier pour confirmer leur rendez-vous.

Deux options d’identification :

1. **FranceConnect** : les informations de contact sont récupérées automatiquement. C'est le parcours le plus rapide et sécurisé.&#x20;
2. **Création de compte** : si l’usager ne passe pas par FranceConnect, il doit renseigner son nom, prénom, email et (optionnellement) son numéro de téléphone. Un email de vérification lui sera envoyé, et en cliquant sur le lien de vérificatio présent dans le mail, il sera redirigé vers son parcours et pourra finaliser son rendez-vous.&#x20;

</details>

## Notification usagers

<details>

<summary><strong>Quand sont envoyées les notifications SMS et email des usagers ?</strong></summary>

**Cette fonctionnalité permet d'automatiser les informations de rendez-vous à vos usagers. Elle répond à plusieurs besoins agents et usagers. Elle permet de diminuer l'absentéisme et d'éviter les manipulation de rappel chronophage pour les agents. Elle permet aussi à l'usager de garder une trace des informations du rendez-vous dans son téléphone.**&#x20;

Plusieurs actions déclenchent l'envoi de SMS :&#x20;

* Une notification de **confirmation** est envoyée immédiatement après la création du rendez-vous.
* Une notification de **rappel** est envoyée à l'usager 48h avant le rendez-vous (hors jours fériés et dimanches).
* Une notification de **rendez-vous modifié** : l'usager reçoit immédiatement une notification en cas de modification du rendez-vous.
* Une notification de **rendez-vous annulé** : l'usager reçoit immédiatement une notification en cas d'annulation du rendez-vous. Si l'usager est à l'origine de l'annulation, il doit le faire au moins 4 heures avant l'heure prévue du rendez-vous.

</details>

<details>

<summary><strong>Qu’est-ce que peut faire un usager depuis ces notification SMS ?</strong></summary>

Chaque usager recevra une notification par SMS et/ou email.

* Le SMS contiendra un lien "Infos/Annulation".
* En cliquant dessus, il accèdera à une page web où il devra saisir les trois premières lettres de son nom de famille.
* S'il les saisit correctement, il verra un récapitulatif de son rendez-vous avec les instructions associées ainsi que les informations de contact de votre organisation.&#x20;

Un bouton "Annuler le rendez-vous" lui permettra d’annuler sans vous contacter, jusqu’à **4 heures avant** l’heure prévue. Au-delà, il devra vous contacter via les informations de contact disponible dans le récapitulatif de rendez-vous. &#x20;

</details>

## Les rendez-vous

<details>

<summary><strong>Comment utiliser les plages d’ouvertures ?</strong></summary>

**Les plages d’ouverture permettent de définir les disponibilités d’un agent. Une fois configurées, elles simplifient la prise de rendez-vous : les agents peuvent directement rechercher un créneau via le bouton "Trouver un RDV", évitant ainsi une consultation fastidieuse des agendas individuels.**

Pour créer une plage d’ouverture :&#x20;

* &#x20;Accédez au menu **"Plages d’ouverture"** dans l’onglet **"Planning"**.&#x20;
* Cliquer sur **"Créer une plage d’ouverture"**.

Lors de la création, sélectionnez un ou plusieurs motifs pour indiquer les types de rendez-vous possibles. Cette option est particulièrement utile si certains motifs nécessitent du matériel spécifique.

Si un motif est ouvert à la réservation en ligne, la plage d’ouverture sera accessible aux réservations en ligne depuis votre url de prise de rendez-vous en ligne.&#x20;

Vous pouvez créer une plage exceptionnelle (pour un jour unique) ou récurrente (tous les jours de la semaine). Pour une répétition, indiquez d’abord les horaires, puis cochez l’option **"Répéter"**.

Les plages d’ouverture de plus d’un an sont automatiquement supprimées.

</details>

<details>

<summary><strong>Comment gérer une indisponibilité ponctuelle ?</strong></summary>

**Les indisponibilités permettent de signaler vos absences ponctuelles ou régulières à vos collègues et aux usagers. Cette fonctionnalité évite de modifier les plages d'ouvertures en cas d'indisponiblité ponctuelle des agents. Si une indisponibilité couvre la période d'une plage d'ouverture, les disponibilités de cette période seront supprimées.**

Pour créer une indisponibilité :

1. Accédez au menu _**planning**_
2. Sélectionnez _**indisponibilité**_
3. Cliquez sur "créer une indisponibilité"
4. Renseignez les informations demandées

Vous pouvez configurer des absences ponctuelles ou récurrentes en utilisant l'option _**répéter**_.

Les indisponibilités apparaissent en gris sur votre agenda et ceux de vos collègues.&#x20;

**Pour une indisponibilité récurrente, il n'est pas possible de supprimer une seule occurrence. Vous devrez supprimer l'indisponibilité récurrente entière et en créer une nouvelle excluant l'occurrence non désirée.**

</details>

<details>

<summary><strong>Comment trouver une disponibilité dans mon organisation ?</strong></summary>

Le bouton **"Trouver un rendez-vous"** permet de rechercher rapidement des disponibilités dans votre organisation ou service, évitant ainsi une consultation manuelle des agendas.

Pour utiliser cette fonctionnalité :&#x20;

1. Cliquez sur **"Trouver un rendez-vous"** pour accéder au moteur de recherche.
2. Spécifiez vos critères : service, motif, agent, lieu et date.
3. Cliquez sur **"Afficher les créneaux"** pour voir les disponibilités correspondantes.

Conditions d’accès :

* Disponible uniquement si les agents ont configuré leurs plages d’ouverture.
* **Administrateurs et secrétariats** : accès à toutes les disponibilités.
* **Agents simples** : accès uniquement aux créneaux de leur service.

Si plusieurs agents sont disponibles sur le même créneau et motif, la première disponibilité enregistrée sera sélectionnée.

</details>

<details>

<summary><strong>Comment planifier un rendez-vous ?</strong></summary>

Après avoir sélectionné une disponibilité via **"Trouver un RDV"**, vous passerez à la planification du rendez-vous :&#x20;

1. **Associer un usager** :&#x20;

* Recherchez l’usager en tapant les premières lettres de son nom ou prénom.
* Vous verrez les fiches usagers de votre organisation et, de façon partiellement masquée, celles d’autres organisations de votre territoire

💡 **Plusieurs usagers peuvent être ajoutés à un rendez-vous.**

2. **Vérifier et modifier les informations** :

* Un récapitulatif s’affiche avec la date, l’heure, l’agent et le lieu du rendez-vous.

💡 **Chaque champ peut être modifié si nécessaire.**

3. **Gérer les notifications** :

* Un dernier récap vous permet d’activer ou désactiver les notifications pour ce rendez-vous.

</details>

<details>

<summary><strong>Comment exporter une liste de rendez-vous ?</strong></summary>

Le **statut d’agent administrateur** permet d’extraire les statistiques de votre organisation au format **.xls**, en complément de leur visualisation dans l’onglet **Statistiques**.

#### Pour exporter les données :

1. Accédez au menu **"Liste des RDV"**.
2. Compléter les différents champ pour affiner les critères de votre export&#x20;
3. Cliquer sur **"rafraichir la liste"**&#x20;
4. Cliquez sur **"Exporter"** après avoir renseigné vos critères.
5. Retrouvez vos exports dans la page **"Vos exports"**, accessible depuis votre compte (en haut à droite).

💡 **L’extraction se fait par organisation. Si vous en gérez plusieurs, vous devez effectuer une exportation pour chacune.**

</details>

<details>

<summary><strong>Comment trouver une disponiblités dans d’autres organisations ?</strong></summary>

Vous pouvez permettre aux agents de planifier des rendez-vous dans d'autres organisations si vous disposez de plusieurs organisations. Ce parcours est possible par la fonctionnalité **"prescripteur".**&#x20;

Elle permet aux agents de partager leurs disponibilités et de planifier des rendez-vous dans **toutes les organisations** de leur territoire.

Pour configurer :&#x20;

Il est nécessaire de configurer vos motifs **"ouvert aux prescripteur"** depuis l'écran de configuration des motifs. Plus précisément, depuis l'onglet "réservation en ligne" présent dans l'écran de configuration des motifs.&#x20;

Pour l’utiliser :&#x20;

Si des motifs ouverts aux prescripteurs ont été configurés, vous pouvez accéder aux disponibilités d’autres organisations via **"Trouver un rendez-vous"** :

1. Cliquez sur **"Élargir votre recherche"**.
2. Sélectionnez les informations du rendez-vous (motif, lieu, créneau, usagers).
3. Cliquez sur **"Confirmer le RDV"** pour finaliser le rendez-vous.&#x20;

</details>

## Les fiches usagers

<details>

<summary><strong>Comment créer une fiche usager ?</strong></summary>



</details>

<details>

<summary><strong>Comment gérer un doublon de fiche usager ?</strong></summary>



</details>

## Les agents

<details>

<summary><strong>Quels sont les différents droits d’accès des agents ?</strong></summary>



</details>

<details>

<summary><strong>Comment inviter des agents dans mon organisations ?</strong></summary>



</details>

<details>

<summary><strong>Comment modifier le services d’un agent ?</strong></summary>



</details>

## Les motifs

<details>

<summary><strong>Comment créer et configurer un motif ?</strong></summary>



</details>

<details>

<summary><strong>Comment gérer en masse des motifs à l’échelle de mon territoire ?</strong></summary>



</details>

## Les organisations

<details>

<summary><strong>À quoi sert les organisations ?</strong></summary>



</details>

<details>

<summary><strong>Comment créer des organisations ?</strong></summary>



</details>



Statistiques
