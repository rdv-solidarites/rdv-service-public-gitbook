---
icon: message-question
---

# FAQ : toutes les notions (test)

## Synchronisation calendrier

<details>

<summary>Comment recevoir des notifications d’alertes de rendez-vous ?</summary>

<mark style="background-color:green;">**Cette fonctionnalité permet de recevoir des email de notification quand un rendez-vous est planifié dans un agenda. Elle répond au besoin des agents qui souhaitent être alertés quand une modification est effectuée dans leur agenda. De cette manière, chaque agent est informé quand une modification est réalisée dans leur agenda.**</mark>&#x20;

Vous pouvez modifier vos préférences de notifications email dans l’espace « Mon Compte » accessible en cliquant sur votre prénom en haut à droite depuis votre vue calendrier.

Cette synchronisation envoie un email pour chaque création, modification ou annulation de RDV.&#x20;

Chaque email contient une pièce jointe au format ICS, un format largement supporté. Votre logiciel de calendrier externe reconnaîtra ces emails et mettra automatiquement à jour les évènements dans votre calendrier. Certains logiciels de calendrier demandent « d’accepter » chaque modification.

</details>

<details>

<summary>Comment synchroniser avec mon agenda ?</summary>

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

## Prise de rendez-vous en ligne

<details>

<summary>Comment mettre en place de la prise de rende-vous en ligne ?</summary>

Pour activer la prise de rendez-vous en ligne, il est nécessaire de réaliser 3 actions :

* Configurer des motifs « ouverts aux agents, aux prescripteurs et aux usagers »
* Associer ces motifs à des plages d'ouverture dans les agendas des agents
* Partager votre URL de prise de rendez-vous en ligne

#### Configurer des motifs ouvert à la réservation en ligne

Vous devez configurer au moins un motif dans les paramètres en activant l'option _**ouvert aux agents et aux usagers**_. Vous pouvez personnaliser ce champ en indiquant un délai minimum et un délai maximum de réservation. De plus, vous pouvez ajouter des instructions depuis l'onglet "instruction et notification".&#x20;

#### Configurer une plage d’ouverture

Vous devez créer une _**plage d'ouverture**_ avec des motifs configurés comme _**ouverts à la réservation en ligne**_.

**Les motifs configurés comme ouverts à la réservation en ligne sont identifiés par une pastille en ligne depuis l'écran de suivi des motifs.**&#x20;

#### Partager votre URL de prise de rendez-vous

Vous pouvez extraire un lien URL depuis le menu _**Réservation en ligne**_ qui dirigera l'usager ou le prescripteur vers la page de vos disponibilités via un navigateur web.

Vous pouvez ensuite communiquer ce lien aux prescripteurs de votre territoire ou l'intégrer dans divers supports (site internet, plaquette numérique).

</details>

<details>

<summary>Comment les usagers prennent-ils rendez-vous ?</summary>



</details>

## Notification usagers

<details>

<summary>Quand sont envoyées les notifications SMS et email des usagers ?</summary>

Plusieurs actions déclenchent l'envoi de SMS :&#x20;

* Une notification de **confirmation** est envoyée immédiatement après la création du rendez-vous.
* Une notification de **rappel** est envoyée à l'usager 48h avant le rendez-vous (hors jours fériés et dimanches).
* Une notification de **rendez-vous modifié** : l'usager reçoit immédiatement une notification en cas de modification du rendez-vous.
* Une notification de **rendez-vous annulé** : l'usager reçoit immédiatement une notification en cas d'annulation du rendez-vous. Si l'usager est à l'origine de l'annulation, il doit le faire au moins 4 heures avant l'heure prévue du rendez-vous.

</details>

<details>

<summary>Qu’est-ce que peut faire un usager depuis ces notification SMS et email ?</summary>



</details>

## Les rendez-vous

<details>

<summary>Comment utiliser les plages d’ouvertures ?</summary>

<mark style="background-color:green;">Les plages d'ouvertures permettent de renseigner les disponiblités d'un agent. Une fois configurées, les agents pourront planifier des rendez-vous simplement en recherchant des disponiblités depuis le bouton</mark> <mark style="background-color:green;"></mark><mark style="background-color:green;">**Trouver un RDV.**</mark> <mark style="background-color:green;"></mark><mark style="background-color:green;">C'est un gage de simplicité et d'efficacité dans les organisations. Cette fonctionnalité permet d'éviter la recherche chronophage dans les agendas individuels des agents</mark>.&#x20;

Pour créer une plage d'ouverture, accédez au menu _**plages d'ouverture**_ depuis le menu _**planning**_.

Vous y verrez vos différentes plages d'ouverture existantes ainsi qu'un bouton _**créer une plage d'ouverture**_.

Lors de la création, vous devez sélectionner un ou plusieurs motifs. Cette fonctionnalité permet de préciser votre disponibilité pour différents types de rendez-vous sur une période donnée, particulièrement utile si certains nécessitent un matériel spécifique.

**Si vous sélectionnez un motif ouvert à la réservation en ligne, votre plage d'ouverture sera accessible à la réservation en ligne.**&#x20;

Une plage d'ouverture peut être exceptionnelle (un jour unique) ou récurrente (tous les jours de la semaine). Si vous souhaitez une répétition, indiquez d'abord la plage horaire, puis cochez la case _**Répéter**_.

**Conservation des données : les plages d'ouverture de plus d'un an sont automatiquement supprimée**

</details>

<details>

<summary>Comment gérer une indisponibilité ponctuelle ?</summary>

Les indisponibilités permettent de signaler vos absences ponctuelles ou régulières à vos collègues et aux usagers.

**Les indisponibilités apparaissent en gris sur votre agenda et ceux de vos collègues.**

**Si une indisponibilité couvre la période d'une plage d'ouverture, les disponibilités de cette période seront supprimées.**

Pour créer une indisponibilité :

1. Accédez au menu _**planning**_
2. Sélectionnez _**indisponibilité**_
3. Cliquez sur "créer une indisponibilité"
4. Renseignez les informations demandées

Vous pouvez configurer des absences ponctuelles ou récurrentes en utilisant l'option _**répéter**_.

**Pour une indisponibilité récurrente, il n'est pas possible de supprimer une seule occurrence. Vous devrez supprimer l'indisponibilité récurrente entière et en créer une nouvelle excluant l'occurrence non désirée.**

</details>

<details>

<summary>Comment trouver une disponibilité dans mon organisation ?</summary>

Le bouton _**trouver un rendez-vous**_ est un moteur de recherche permettant de trouver les disponibilités au sein de votre organisation ou de votre service.

**Cette fonctionnalité n'est disponible que si les agents ont configuré leurs plages d'ouverture**.

**Le statut d'agent administrateur et le service de secrétariat permettent d'accéder aux disponibilités des agents de toute l'organisation. En revanche, le statut d'agent simple vous donne uniquement la visibilité sur les disponibilités des agents de votre service.**

En cliquant sur le bouton _**trouver un rendez-vous**_, vous accéderez à un moteur de recherche. Vous serez invité à spécifier les critères de la disponibilité souhaitée : le service, le motif, l'agent, le lieu et la date. Une fois ces informations saisies, cliquez sur _**Afficher les créneaux**_. Un écran affichera alors les disponibilités correspondant aux critères que vous avez indiqués.

**Si plusieurs agents indiquent des disponibilités sur le même créneau pour le même motif, la solution sélectionnera la première disponibilité enregistrée.**

</details>

<details>

<summary>Comment planifier un rendez-vous ?</summary>

Après avoir sélectionné une disponibilité via le parcours _Trouver une disponibilité_, vous entrerez dans le parcours de planification du rendez-vous. Plusieurs informations vous seront demandées :

#### L’u**sager**

Dans ce champ, vous devez indiquer l'usager concerné par le rendez-vous. Utilisez le moteur de recherche en saisissant les premières lettres du nom ou du prénom de l'usager.

**Les fiches usagers proposées seront celles créées dans votre organisation. Vous verrez également s'afficher les fiches usagers créées dans d'autres organisations de votre territoire. Par respect pour la confidentialité des données, les informations personnelles des fiches usagers d'autres organisations de votre territoire seront partiellement masquées.**

***

## Les horaires et le lieux

Vous devez renseigner la date et l’heure. Ces informations seront pré-remplies sur la base de votre sélection (soit depuis l’_**agenda**_ ; soit depuis le bouton _**trouver un rendez-vous**_). Vous devez ensuite renseigner une durée. Par défaut, cette information sera pré-remplie sur la base des paramètres du motifs sélectionné. Enfin, il faudra sélectionner un lieu parmi les lieux de votre organisation.

Vous avez la possibilité de créer un lieu ponctuel. Il s’agit d’un rendez-vous à une adresse inhabituelle. La saisie de ce champ est libre.

***

## L’a**gent**

Vous devrez également indiquer l'agent responsable de ce rendez-vous. Si le rendez-vous nécessite l'intervention de deux professionnels, il est possible d'associer deux agents à un même rendez-vous. Si vous avez utilisé le parcours _**trouver un rendez-vous**_, un agent sera présélectionné.

***

## **Les préférences de notifications**

Enfin, le champ _**« notification »**_ résume le comportement et les informations de notification. Le comportement est lié au motif, tandis que les notifications se rapportent principalement à la fiche usager. Pour informer l'usager du rendez-vous par e-mail et par SMS, il est impératif de renseigner ces informations dans sa fiche usager _(**plus d'informations ici**)_.

</details>

<details>

<summary>Comment exporter une liste de rendez-vous ?</summary>



</details>

<details>

<summary>Comment trouver une disponiblités dans d’autres organisations ?</summary>



</details>

## Les fiches usagers

<details>

<summary>Comment créer une fiche usager ?</summary>



</details>

<details>

<summary>Comment gérer un doublon de fiche usager ?</summary>



</details>

## Les agents

<details>

<summary>Quels sont les différents droits d’accès des agents ?</summary>



</details>

<details>

<summary>Comment inviter des agents dans mon organisations ?</summary>



</details>

<details>

<summary>Comment modifier le services d’un agent ?</summary>



</details>

## Les motifs

<details>

<summary>Comment créer et configurer un motif ?</summary>



</details>

<details>

<summary>Comment gérer en masse des motifs à l’échelle de mon territoire ?</summary>



</details>

## Les organisations

<details>

<summary>À quoi sert les organisations ?</summary>



</details>

<details>

<summary>Comment créer des organisations ?</summary>



</details>



Statistiques
