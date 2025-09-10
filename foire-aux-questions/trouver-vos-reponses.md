---
icon: message-question
---

# Trouver vos réponses

## Notifications agent

<details>

<summary><strong>Comment recevoir des notifications d’alertes de rendez-vous ?</strong></summary>

Cette fonctionnalité permet de recevoir des notifications par email lorsqu’un rendez-vous est ajouté, modifié ou annulé dans un agenda. Elle répond au besoin des agents souhaitant être alertés en cas de changement dans leur planning.

Vous pouvez personnaliser vos préférences de notification dans l’onglet _**Mon Compte**_, accessible en cliquant sur votre prénom en haut à droite de votre calendrier.

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

Chaque email contient une pièce jointe au format **ICS**, compatible avec la plupart des logiciels de calendrier. Votre calendrier externe reconnaîtra automatiquement ces mises à jour, bien que certains logiciels demandent une validation manuelle des modifications.

</details>

<details>

<summary><strong>Je ne reçois pas les emails de RDV·SP. Comment y remédier ?</strong></summary>

### Votre client mail classe nos emails en spam

Les emails provenant de l’adresse RDV Service Public peuvent être classifiés à tort comme du spam par votre client mail (Outlook, Thunderbird, etc).

**Solution** : Dans votre boîte e-mail, vérifiez les dossiers « spam » ou « indésirables ». En complément, vous pouvez signaler l’adresse RDV Service Public comme n’étant pas un spam. De cette façon, vous recevrez les e-mails RDV Services Publics directement

### Un autre logiciel de filtrage d’email classe nos emails en spam

Le domaine RDV Service Public peut être bloqué par un outil de protection des e-mails, tel que **MailinBlack**.

**Solution** : Autorisez notre adresse e-mail en suivant ces étapes :

* Connectez-vous à votre interface MailinBlack.
* Sur la page principale, sélectionnez l’onglet « Newsletter »
* Cliquez sur l’icône de droite et autorisez les adresses du domaine @rdv-solidarites.fr / @rdv-service-public.fr / @rdv-aide-numerique.fr
* Confirmez en validant le message "Autoriser les messages de ces domaines".

Cette autorisation est appliquée à titre individuel et vos collègues auront potentiellement le même problème. Vous pouvez suggérer au responsable technique de votre administration de consulter [cette page](../toutes-les-notions/informations-pour-les-dsi.md) pour corriger ce problème pour tout le monde.

### Un problème temporaire sur les serveurs de RDV Service Public empêche l’envoi des emails

Il arrive que les serveurs de RDV Service Public rencontrent des ralentissements ou soient temporairement inaccessibles.

**Solution** :  Vous pouvez suivre en temps réel l'évolution du dysfonctionnement sur notre [page de statut](https://rdv-service-public.instatus.com).

### Un problème temporaire sur les serveurs de votre système informatique (SI) empêche la réception des emails

Il peut arriver que le système d’information ou le réseau interne sur lequel vous naviguez rencontre des ralentissements ou soit inacessible temporairement.

**Solution** :&#x20;

* Contactez le service informatique
* Vous pouvez effectuer les tests suivants pour comprendre si le problème vient du SI de votre service ou de RDV Service Public :
  * Demander à un collègue de vous envoyer un e-mail
  * Envoyez-vous un e-mail depuis une adresse personnelle (Gmail, Outlook, etc.)

Si le problème est lié au SI de votre service, nous ne pourrons malheureusement pas intervenir directement.

### Votre adresse a été bloquée par notre fournisseur d’envoi d’e-mails

Votre adresse e-mail peut être bloquée par notre fournisseur d’envoi.&#x20;

Cette situation peut se produire dans deux cas :&#x20;

* vous avez cliqué sur les liens de nos e-mails qui vous permettent de vous désabonner
* le serveur mail de votre SI a refusé la réception des emails envoyés par RDV Service Public car il les considérant comme du spam. Cela se produit suite à une classification manuelle d’un de nos mails comme du spam par un agent au sein de votre SI, ou par une classification automatique.

**Solution** :  Envoyez-nous un e-mail à [support@rdv-service-public.fr](mailto:support@rdv-service-public.fr)

Si vous vous retrouvez dans cette situation, il est probable que plusieurs de vos collègues soient dans la même situation. Vous pouvez suggérer aux responsables techniques de votre SI de consulter le sinformations ci-dessous pour corriger le problème durablement et à l’échelle de tout votre service :&#x20;

### Les emails de RDV Service Public ne sont pas reçus par les agents

Si un des agents de votre service rencontre ce genre de problèmes de réception d’emails, il est probable que d’autres le rencontrent à leur tour. En tant que responsable technique vous avez la possibilité de configurer le SI pour corriger ces problèmes pour tous les agents.

Le but est de faire en sorte que les serveurs mails du SI ne refusent jamais les emails envoyés par RDV Service Public. L’idée est de mettre dans des listes d’acceptations tous les emails émis par RDV Service Public (on parle aussi de _whitelists_).

Il faut le cas échéant faire cette configuration à deux niveaux :&#x20;

* le système de détection de spam natif du serveur mail de votre SI
* le(s) logiciel(s) de filtrage d’email branchés sur votre serveur comme MailInBlack

Le plus robuste est d’ajouter dans les listes d’acceptations l’adresse IP suivante,  nous envoyons tous nos emails depuis cette adresse :

```
212.146.241.127
```

Si vous ne trouvez pas l’option pour ajouter une IP dans une liste d’acceptation, vous pouvez en repli ajouter les domaines émetteurs suivants comme domaines de confiance  :&#x20;

```
reply.demo.rdv-solidarites.fr
reply.staging.rdv-service-public.fr
reply.rdv-service-public.fr
reply.demo.rdv-aide-numerique.fr
reply.demo.rdv-service-public.fr
reply.rdv-aide-numerique.fr
rdv-aide-numerique.fr
rdv-service-public.fr
reply.rdv-solidarites.fr
email.rdv-solidarites.fr
rdv-solidarites.fr
```

N’hésitez pas à nous contacter à support@rdv-service-public.fr pour que nous puissions vous aider à faire ces configurations.

</details>

## Synchronisation calendrier

<details>

<summary><strong>Comment synchroniser les rendez-vous avec mon agenda ?</strong></summary>

Cette fonctionnalité permet d'envoyer les informations des rendez-vous planifié dans un agenda extérieur à RDV Service Public. Elle répond au besoin de faire afficher les rendez-vous planifié dans un agenda du quotidien, souvent utilisé dans les administrations pour gérer leur quotidien métier en dehors des rendez-vous (réunion d'équipe etc ...)

#### Notes générales&#x20;

RDV Service Public propose différents mécanismes de synchronisation. Voici quelques remarques importantes valables pour tous les mécanismes :

* Pour protéger les données personnelles de vos usagers, les événements envoyés à votre logiciel de calendrier externe ne contiendront que le motif, l'adresse du rendez-vous et un lien vers les détails dans RDV Service Public ;&#x20;
* Nous proposons de synchroniser les créations, changements et annulations depuis RDV Service Public vers les logiciels de calendrier externes mais pas l’inverse. Si vous supprimez un RDV depuis votre logiciel de calendrier externe, cela ne sera pas répercuté dans RDV Service Public et l’usager n’en sera pas averti.

#### S**ynchronisation par email**

Cette synchronisation envoie un email pour chaque création, modification ou annulation de RDV.&#x20;

Chaque email contient une pièce jointe au format ICS, un format largement supporté. Votre logiciel de calendrier externe reconnaîtra ces emails et mettra automatiquement à jour les évènements dans votre calendrier. Certains logiciels de calendrier demandent « d’accepter » chaque modification.

Vous pouvez modifier vos préférences de notifications email dans l’espace « Mon Compte » accessible en cliquant sur votre prénom en haut à droite depuis votre vue calendrier.

#### **Synchronisation Outlook (Microsoft 365)**

Une application Microsoft 365 permet de synchroniser vos RDV vers votre agenda Outlook. Cette application ne fonctionne que pour les versions d’Outlook hébergées par Microsoft, pas pour les versions hébergées sur site.

Vous trouverez plus d’informations sur cette page :&#x20;

[synchronisation-outlook-microsoft-365.md](../toutes-les-notions/synchronisation-outlook-microsoft-365.md "mention")

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

<details>

<summary><strong>Pourquoi certains RDV ne sont pas synchronisés dans mon calendrier externe ?</strong></summary>

Les raisons de ce genre de problèmes dépendent du type de synchronisation avec votre calendrier externe (voir question précédente).

Le mécanisme de synchronisation le plus répandu est celui utilisant les emails avec des pièces-jointes ICS. Dans ce cas, la raison la plus fréquente pour laquelle une partie des RDV ne se synchronisent pas c’est que vos préférences de notifications par mail sont trop restrictives.

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

cf cette question pour apprendre à modifier ces préférences :

[#comment-recevoir-des-notifications-dalertes-de-rendez-vous](trouver-vos-reponses.md#comment-recevoir-des-notifications-dalertes-de-rendez-vous "mention")

</details>

## Prise de rendez-vous en ligne

<details>

<summary><strong>Comment mettre en place de la prise de rendez-vous en ligne ?</strong></summary>

Cette fonctionnalité permet aux usagers d’accéder aux disponibilités de votre organisation et de planifier un rendez-vous en toute autonomie, depuis un ordinateur ou un téléphone.

Pour activer cette option, trois étapes sont nécessaires :

* **Configurer des motifs ouverts à la réservation en ligne**

Dans les paramètres des motifs, sélectionnez au moins un motif et activez l’option _**Ouvert aux agents, aux prescripteurs et aux usagers**_. Vous pouvez également définir un délai minimum et maximum de réservation et ajouter des instructions personnalisées dans l’onglet _**Instruction et notification**_.

* **Configurer une plage d’ouverture**

Créez une plage d’ouverture en y associant des motifs configurés pour la réservation en ligne. Ces motifs sont identifiés par une pastille spécifique dans l’écran de suivi des motifs.

* **Partager votre URL de prise de rendez-vous**

Un lien URL est disponible dans le menu _**Réservation en ligne**_. Ce lien permet aux usagers et prescripteurs d’accéder directement à vos disponibilités via un navigateur web. Vous pouvez partager cette URL ou l’intégrer dans différents supports, tels que votre site internet ou une plaquette numérique.



</details>

<details>

<summary><strong>Est-il possible d'ajouter un formulaire dans le parcours en ligne ?</strong></summary>

Il n'est pas possible d'intégrer de formulaire ou de questionnaire en amont du choix du créneaux. Cette fonctionnalité n'exsite pas encore dans notre solution. Toutefois, vous pouvez personnaliser un message d'instruction qui s'affichera dans le parcours de prise de rendez-vous en ligne. Ce message est personnalisable motif par motif.&#x20;

Pour ajouter un message d'instruction :&#x20;

* Sélectionner un motif à modifier depuis _**paramètre**_ puis _**motif**_&#x20;
* Accéder à l'onglet _**notifications et instructions**_&#x20;
* Compléter le champ _**instructions affichées avant la prise de rendez-vous**_

Ces informations apparaîtront entre la sélection du lieu de rendez-vous et du créneau de rendez-vous dans le parcours en ligne.&#x20;

</details>

<details>

<summary><strong>Puis-je utiliser une solution d'intégration type iFrame sur mon site internet ?</strong> </summary>

Nous ne proposons pas encore ce type d'intégration. Nous proposons une intégration simple via un URL à intégrer dans votre site internet :&#x20;

* Soit directement en corps de texte d'une page web
* Soit via un bouton CTA avec l'URL en hyperlien.&#x20;

</details>

<details>

<summary><strong>Comment les usagers prennent-ils rendez-vous ?</strong></summary>

Les usagers peuvent prendre rendez-vous en ligne si cette option est activée et que vous avez partagé votre lien de réservation. Ce lien peut être diffusé sur votre site web ou tout autre support.

Une fois sur la plateforme, ils pourront :

* Choisir un service et un motif de rendez-vous.&#x20;
* Sélectionner un créneau disponible
* S’identifier pour confirmer leur rendez-vous.

Deux options d’identification :

1. **FranceConnect** : les informations de contact sont récupérées automatiquement. C'est le parcours le plus rapide et sécurisé.&#x20;
2. **Création de compte** : si l’usager ne passe pas par FranceConnect, il doit renseigner son nom, prénom, email et (optionnellement) son numéro de téléphone. Un email de vérification lui sera envoyé, et en cliquant sur le lien de vérificatio présent dans le mail, il sera redirigé vers son parcours et pourra finaliser son rendez-vous.&#x20;

</details>

<details>

<summary><strong>Comment rendre accessible mes disponiblités à des partenaires ?</strong> </summary>

La fonctionnalité **prescripteur** permet à un partenaire extérieur (ex. : association, administration, collectivité) de planifier des rendez-vous pour un usager dans vos disponibilités. Cela facilite le parcours des usagers en permettant à différentes entités administratives de rediriger les usagers vers un rendez-vous dans votre structure.&#x20;

#### **Comment ça fonctionne ?**

* **Configuration** : Activez des motifs de rendez-vous ouverts à la réservation en ligne dans vos disponibilités.
* **Partage de l'URL** : Envoyez l'URL de réservation en ligne à vos partenaires.&#x20;

Des notifications seront envoyées une fois le rendez-vous planifié :&#x20;

* **Prescripteur** : Reçoit un e-mail de confirmation du rendez-vous.
* **Usager** : Reçoit une confirmation et un rappel 48 heures avant le rendez-vous.
* **Professionnel** : Le rendez-vous apparaît dans son agenda, avec synchronisation possible.

**Que doit faire un prescripteur ?**

* Accéder à la prise de rendez-vous en ligne et réaliser le parcours &#x20;
* Cliquer sur _**Je suis un prescripteur qui oriente un bénéficiaire**_ lors du dernier écran d'authentification usager.&#x20;
* Saisir les coordonnées prescripteurs et celles de l'usager.
* Confirmer le rendez-vous. Un récapitulatif sera généré à la fin.

</details>

## Notification usagers

<details>

<summary><strong>Puis-je modifier les informations du SMS ?</strong> </summary>

Il n’est pas possible de modifier le modèle SMS : le nombre de caractères pour les SMS est limité. Aussi certaines informations comme le nom du motif peut porter atteinte à l’usager. Nous avons donc fait le choix de limiter les informations présentes dans le SMS.&#x20;

</details>

<details>

<summary><strong>Quand sont envoyées les notifications SMS et email des usagers ?</strong></summary>

Cette fonctionnalité permet d'automatiser les informations de rendez-vous à vos usagers. Elle répond à plusieurs besoins agents et usagers. Elle permet de diminuer l'absentéisme et d'éviter les manipulation de rappel chronophage pour les agents. Elle permet aussi à l'usager de garder une trace des informations du rendez-vous dans son téléphone.&#x20;

Plusieurs actions déclenchent l'envoi de SMS :&#x20;

* Une notification de **confirmation** est envoyée immédiatement après la création du rendez-vous.
* Une notification de **rappel** est envoyée à l'usager 48h avant le rendez-vous (hors jours fériés et dimanches).
* Une notification de **rendez-vous modifié** : l'usager reçoit immédiatement une notification en cas de modification du rendez-vous.
* Une notification de **rendez-vous annulé** : l'usager reçoit immédiatement une notification en cas d'annulation du rendez-vous. Si l'usager est à l'origine de l'annulation, il doit le faire au moins 4 heures avant l'heure prévue du rendez-vous.

</details>

<details>

<summary><strong>Puis-je ajouter des instructions dans les notifications des usagers ?</strong> </summary>

Vous pouvez ajouter des instructions dans les notifications emails que recevront les usagers. Ces instructions peuvent être personnalisées motif par motif.&#x20;

Pour ajouter des instructions dans les notification email :&#x20;

* Sélectionner un motif à modifier depuis _**paramètre**_  puis _**motif**_&#x20;
* Accéder à l'onglet  _**notifications et instructions**_&#x20;
* Compléter le champ _**instructions affichées après la prise de rendez-vous**_

Ces informations apparaîtront à 3 niveaux :&#x20;

* Dans le dernier écran de confirmation du parcours usager&#x20;
* Dans la notification email de création et de rappel usager
* Dans la note d'information accessible depuis l'URL du SMS

</details>

<details>

<summary><strong>Qu’est-ce que peut faire un usager depuis ces notification SMS ?</strong></summary>

Chaque usager recevra une notification par SMS et/ou email.

* Le SMS contiendra un lien _**Infos/Annulation**_.
* En cliquant dessus, il accèdera à une page web où il devra saisir les trois premières lettres de son nom de famille.
* S'il les saisit correctement, il verra un récapitulatif de son rendez-vous avec les instructions associées ainsi que les informations de contact de votre organisation.&#x20;

Un bouton  _**Annuler le rendez-vous**_ lui permettra d’annuler sans vous contacter, jusqu’à **4 heures avant** l’heure prévue. Au-delà, il devra vous contacter via les informations de contact disponible dans le récapitulatif de rendez-vous. &#x20;

</details>

## Les agendas et les rendez-vous

<details>

<summary><strong>Qui peut voir et modifier mon agenda ?</strong> </summary>

Par défaut, seuls les agents de votre service et de votre organisation peuvent consulter et planifier des rendez-vous dans votre agenda. De plus, les agents du service secrétariat de votre organisation ont un accès étendu : ils peuvent voir, modifier et planifier des rendez-vous de tous les agendas.&#x20;

</details>

<details>

<summary><strong>Comment utiliser les plages d’ouvertures ?</strong></summary>

Les plages d’ouverture permettent de définir les disponibilités d’un agent. Une fois configurées, elles simplifient la prise de rendez-vous : les agents peuvent directement rechercher un créneau via le bouton _**Trouver un RDV**_, évitant ainsi une consultation fastidieuse des agendas individuels.

Pour créer une plage d’ouverture :&#x20;

* &#x20;Accédez au menu  _**Plages d’ouverture**_ dans l’onglet  _**Planning**_
* Cliquer sur  _**Créer une plage d’ouverture**_

Lors de la création, sélectionnez un ou plusieurs motifs pour indiquer les types de rendez-vous possibles. Cette option est particulièrement utile si certains motifs nécessitent du matériel spécifique.

Si un motif est ouvert à la réservation en ligne, la plage d’ouverture sera accessible aux réservations en ligne depuis votre url de prise de rendez-vous en ligne.&#x20;

Vous pouvez créer une plage exceptionnelle (pour un jour unique) ou récurrente (tous les jours de la semaine). Pour une répétition, indiquez d’abord les horaires, puis cochez l’option _**Répéter**_.

Les plages d’ouverture de plus d’un an sont automatiquement supprimées.

</details>

<details>

<summary><strong>Comment gérer une indisponibilité ponctuelle ?</strong></summary>

Les indisponibilités permettent de signaler vos absences ponctuelles ou régulières à vos collègues et aux usagers. Cette fonctionnalité évite de modifier les plages d'ouvertures en cas d'indisponiblité ponctuelle des agents. Si une indisponibilité couvre la période d'une plage d'ouverture, les disponibilités de cette période seront supprimées.

Pour créer une indisponibilité :

* Accédez au menu _**planning**_
* Sélectionnez _**indisponibilité**_
* Cliquez sur  _**créer une indisponibilité**_&#x20;
* Renseignez les informations demandées

Vous pouvez configurer des absences ponctuelles ou récurrentes en utilisant l'option _**répéter**_.

Les indisponibilités apparaissent en gris sur votre agenda et ceux de vos collègues.&#x20;

Pour une indisponibilité récurrente, il n'est pas possible de supprimer une seule occurrence. Vous devrez supprimer l'indisponibilité récurrente entière et en créer une nouvelle excluant l'occurrence non désirée.

</details>

<details>

<summary><strong>Comment trouver une disponibilité auprès des agents de mon organisation ?</strong></summary>

Le bouton _**Trouver un rendez-vous**_ permet de rechercher rapidement des disponibilités dans votre organisation ou service, évitant ainsi une consultation manuelle des agendas.

Pour utiliser cette fonctionnalité :&#x20;

* Cliquez sur _**Trouver un rendez-vous**_ pour accéder au moteur de recherche.
* Spécifiez vos critères : service, motif, agent, lieu et date.
* Cliquez sur _**Afficher les créneaux**_ pour voir les disponibilités correspondantes.

Conditions d’accès :

* Disponible uniquement si les agents ont configuré leurs plages d’ouverture.
* **Administrateurs et secrétariats** : accès à toutes les disponibilités.
* **Agents simples** : accès uniquement aux créneaux de leur service.

Si plusieurs agents sont disponibles sur le même créneau et motif, la première disponibilité enregistrée sera sélectionnée.

</details>

<details>

<summary><strong>Comment planifier un rendez-vous ?</strong></summary>

Après avoir sélectionné une disponibilité via _**Trouver un RDV**_, vous passerez à la planification du rendez-vous :&#x20;

* **Associer un usager** :&#x20;

Recherchez l’usager en tapant les premières lettres de son nom ou prénom. Vous verrez les fiches usagers de votre organisation et, de façon partiellement masquée, celles d’autres organisations de votre espace. **Plusieurs usagers peuvent être ajoutés à un rendez-vous.**

* **Vérifier et modifier les informations** :

Un récapitulatif s’affiche avec la date, l’heure, l’agent et le lieu du rendez-vous. **Chaque champ peut être modifié si nécessaire.**

* **Gérer les notifications :**&#x20;

Un dernier récap vous permet d’activer ou désactiver les notifications pour ce rendez-vous.

</details>

<details>

<summary><strong>Comment exporter une liste de rendez-vous ?</strong></summary>

Le **statut d’agent administrateur** permet d’extraire les statistiques de votre organisation au format **.xls**, en complément de leur visualisation dans l’onglet _**Statistiques**_.

#### Pour exporter les données :

* Accédez au menu _**Liste des RDV**_.
* Compléter les différents champ pour affiner les critères de votre export&#x20;
* Cliquer sur _**rafraichir la liste**_&#x20;
* Cliquez sur _**Exporter**_ après avoir renseigné vos critères.
* Retrouvez vos exports dans la page _**Vos exports**_, accessible depuis votre compte (en haut à droite).

**L’extraction se fait par organisation. Si vous en gérez plusieurs, vous devez effectuer une exportation pour chacune.**

</details>

<details>

<summary><strong>Comment trouver une disponiblités dans d’autres organisations ?</strong></summary>

Vous pouvez permettre aux agents de planifier des rendez-vous dans d'autres organisations si vous disposez de plusieurs organisations. Ce parcours est possible par la fonctionnalité _**prescripteur**_**.**&#x20;

Elle permet aux agents de partager leurs disponibilités et de planifier des rendez-vous dans **toutes les organisations** de leur espace.

Pour configurer :&#x20;

Il est nécessaire de configurer vos motifs _**ouvert aux prescripteur**_ depuis l'écran de configuration des motifs. Plus précisément, depuis l'onglet _**réservation en ligne**_ présent dans l'écran de configuration des motifs.&#x20;

Pour l’utiliser :&#x20;

Si des motifs ouverts aux prescripteurs ont été configurés, vous pouvez accéder aux disponibilités d’autres organisations via _**Trouver un rendez-vous**_ :

* Cliquer sur _**Élargir votre recherche**_.
* Sélectionner les informations du rendez-vous (motif, lieu, créneau, usagers).
* Cliquer sur **C**_**onfirmer le RDV**_ pour finaliser le rendez-vous.&#x20;

</details>

## Les fiches usagers

<details>

<summary><strong>Puis-je modifier ou supprimer les données des usagers ?</strong> </summary>

Vous pouvez supprimer ou modifier les données des usagers. Sur la fiche des usagers, des options Modifier et Supprimer sont prévues à cet effet. Si aucunes modifications n’est apportée et que l’usager n’a pris aucun RDV durant deux ans, alors ses données seront supprimées automatiquement.

</details>

<details>

<summary><strong>Comment créer une fiche usager ?</strong></summary>

Pour créer une fiche :&#x20;

* Dans le menu _**Usager**_, cliquez sur _**Créer un usager**_ ou depuis le parcours _**Trouver un RDV**_ cliquer sur _**Créer un usager**_
* Seuls le nom et le prénom sont obligatoires.
* La fiche sera rattachée à **l’organisation de l’agent** qui l’a créée.
* Cliquez sur _**Créer usager**_ pour valider.

**Pensez à vérifier l’orthographe des noms et prénoms pour éviter les doublons !**&#x20;

Une fois créée, la fiche contient :

* Les **informations générales** de l’usager.
* Son **historique** et le **statut de ses rendez-vous**.
* Une option pour l’**inviter à créer un compte**, afin qu’il puisse **modifier ses infos** et **gérer ses rendez-vous** en autonomie depuis son esapce personnel.&#x20;

</details>

<details>

<summary><strong>Comment gérer un doublon de fiche usager ?</strong></summary>

Les doublons peuvent apparaître lorsque :

* Un professionnel crée une fiche **sans e-mail**, puis l’usager crée un compte avec une adresse e-mail.
* Une faute de frappe lors d’une recherche fait croire qu’aucune fiche n’existe.

**L’outil ne fusionne pas automatiquement les fiches, car l’unicité repose uniquement sur l’e-mail.**

Pour fusionner des fiches usagers :&#x20;

* Accéder au menu _**Usagers**_.
* Cliquer sur _**Fusionner deux usagers**_.
* Entrer le nom de l’usager en double dans chaque colonne.
* Comparez les fiches : **Différences en orange**, **similitudes en vert**.
* Sélectionnez les informations à conserver.
* Validez pour créer une **fiche unique fusionnée**.

</details>

## Les agents

<details>

<summary><strong>Puis-je associer un agent à plusieurs organisations ?</strong> </summary>

Un agent peut être associé à plusieurs organisations. Cette association lui donnera accès aux agendas des agents rattachés à son service dans chacune de ces organisations. Seul un agent administrateur d'espace peut associer un agent à plusieurs organisations.

Pour ajouter un agent à plusieurs organisations :&#x20;

* Accéder à votre _**Espace Admin**_&#x20;
* Sélectionner _**Agent**_&#x20;
* Choisissez l'agent à modifier. Vous trouverez en bas de page les options d'affectations à de nouvelles organisations.

</details>

<details>

<summary><strong>Quels sont les différents droits d’accès des agents ?</strong></summary>

#### **Agent Basique**

L'**Agent Basique** a accès aux fonctionnalités de planification de rendez-vous. Il peut :

* Créer des fiches usagers,
* Planifier des rendez-vous
* Créer des plages d'ouvertures&#x20;
* Rechercher des disponibilités dans les agendas de ses collègues

**Sa visibilité est limitée aux agents de son service et de son organisation. Pour associer un agent à plusieurs services ou organisations.**&#x20;

#### **Agent Admin**

L'**Agent Admin** a une **visibilité étendue** sur toutes les organisations auxquelles il est associé. Il peut :

* Rechercher des disponibilités dans tous les services de son organisation,
* Accéder à l'onglet **Paramètres** pour créer des motifs, lieux et inviter des agents,
* Être associé à plusieurs organisations.

#### **Agent Admin d'Espace**

L'**Agent Admin d'Espace** a une **visibilité totale** sur tous les agendas de l'espace et tous les services/organisations. Il a également accès aux paramètres de tous les services et organisations de l'espace et peut :

* Modifier les droits d'accès des agents,
* Créer des organisations et former des équipes.

**Plusieurs Agents Admin d'Espace peuvent être définis.**&#x20;

#### **Agent Secrétariat**

Un **Agent du service secrétariat** bénéficie de droits de visibilité supérieurs. Il peut :

* Rechercher des disponibilités sur tous les agendas de l'organisation mais avec des droits d'un agent basique.&#x20;
* Planifier des rendez-vous dans n'importe quel agenda de l'organisation (tous services confondus).\
  Sa principale fonction est de planifier des rendez-vous, mais il peut aussi planifier dans son propre agenda.

**Un Agent Admin doit ouvrir les motifs de prise de rendez-vous pour les agents du service secrétariat s'ils doivent réaliser des rendez-vous.**&#x20;

</details>

<details>

<summary><strong>Comment inviter des agents dans mon organisations ?</strong></summary>

Pour inviter un agent :&#x20;

* Allez dans _**Paramètres**_ puis _**Agents**_
* Cliquez sur _**Inviter un agent**_
* Choisissez un niveau d'accès
* Entrez l’adresse e-mail de l'agent
* Enfin, sélectionnez un service auquel associer l'agent
* Il recevra une invitation pour créer son compte. Une fois l’invitation acceptée, l'agent devra créer un mot de passe pour se connecter

**Si vous invitez un agent dans plusieurs organisations, chaque invitation sera validée automatiquement après la première, sans nouvel email d'invitation.**&#x20;

</details>

<details>

<summary><strong>Comment modifier le services d’un agent ?</strong></summary>

Pour modifier le service d'un agent :&#x20;

* Accéder à votre _**Espace Admin**_
* Cliquer sur _**agent**_ et sélectionner _**modifier**_&#x20;
* Associer l'agent à un ou plusieurs services pour définir ses droits d'accès

**Seul un agent admin d'espace pour modifier les services d'un agent.**&#x20;

</details>

<details>

<summary><strong>Comment supprimer un agent ?</strong> </summary>

Pour supprimer un agent :&#x20;

* Allez dans _**Paramètres**_ puis _**Agents**_.
* Cliquez sur l’icône _**Supprimer**_ à côté de l'agent.
* Si l'agent a des rendez-vous à venir, une alerte vous empêchera de le supprimer. Vous devrez réaffecter ces rendez-vous avant de supprimer l'agent.

**Les agents inactifs (non connectés depuis 30 jours) auront l’étiquette "inactif" à côté de leur nom.**

</details>

## Les motifs

<details>

<summary><strong>À</strong> <strong>quoi servent les motifs ?</strong> </summary>

Le motif est la raison du rendez-vous. Il permet de catégoriser les prises de rendez-vous, d’informer l’agent sur le contenu attendu et d’affiner les options (présentiel, téléphone, visio, option de prise de rendez-vous en ligne). Il permet également une configuration fine des disponibilités des agents selon leurs compétences ou capacités dans leurs plages d'ouverture.&#x20;

</details>

<details>

<summary><strong>Puis-je dupliquer des motifs dans une nouvelle organisation ?</strong> </summary>

Vous pouvez dupliquer des motifs déjà créé dans une autre organisation. Cette fonctionnalité permet de répliquer une configuration dans une autre organisation en s'évitant de créer de nouveau tous les motifs.&#x20;

Pour dupliquer un motif :&#x20;

* Accéder à vos motifs depuis _**paramètres**_ puis _**motifs**_&#x20;
* Cliquer sur l'émoticône _**dupliquer**_ à droite de chaque motif
* Sélectionner l'organisation dans laquelle dupliquer le motif
* Au besoin, modifier des configurations du motif&#x20;

</details>

<details>

<summary><strong>Puis-je modifier des motifs en masse ?</strong> </summary>

Vous pouvez modifier des par lot. Cette fonctionnalité permet de changer des configurations pour plusieurs motifs en même temps et ainsi gagner du temps.&#x20;

Pour modifier des motifs en masse :&#x20;

* Accéder à votre _**Espace Admin**_&#x20;
* Sélectionner _**motif**_&#x20;
* Filtrer et rechercher les motifs à modifier et sélectionner les par lot.&#x20;
* Cliquer sur _**modifier les motifs**_&#x20;

**Seul un agent admin d'espace peut modifier des motif en masse.**&#x20;

</details>

## Les services&#x20;

<details>

<summary>À quoi servent les services ? </summary>

Les **services** servent à organiser votre espace et vos organisations en sous-ensembles distincts, chacun avec ses propres **agents** et **motifs**. Concrètement, ils permettent :

* **le cloisonnement** : séparer les activités pour que chaque service ait ses propres règles, agents et motifs.&#x20;
* **la visibilité** : donner à chaque agent une vue adaptée à son service, sans être noyé dans l’ensemble des motifs et informations de toute l'organisation.&#x20;

***

En somme :&#x20;

Sans **services** activés :

* Tous les agents voient l’ensemble des motifs de rendez-vous.
* Par exemple, un agent de l’état civil pourrait avoir accès à des demandes liées à l’urbanisme ou à la petite enfance, ce qui peut générer de la confusion.

Avec **services** activés :

* Vous pouvez créer un **service État civil**, un **service Urbanisme**, un **service Petite enfance.**&#x20;
* Chaque service dispose de ses propres **motifs** (par exemple : “Demande de carte d’identité” pour l’État civil, “Permis de construire” pour l’Urbanisme).
* Vous associez ensuite vos **agents** aux services concernés : les agents de l’État civil ne verront que les motifs qui leur sont liés, et ainsi de suite.

</details>

<details>

<summary><strong>Comment utiliser les services ?</strong> </summary>

Par défaut, lors de la création de votre compte, aucun service ne sera actif dans votre espace.&#x20;

{% hint style="info" %}
**Seul un agent admin d'espace peut activer les services.** &#x20;
{% endhint %}

Pour activer les services :&#x20;

* Accéder à votre _**Espace Admin**_&#x20;
* Sélectionner _**Services**_
* Sélectionner les services que vous souhaitez activer parmi la liste&#x20;
* Cliquer sur _**enregistrer**_ en bas de page

{% hint style="warning" %}
Si vous avez déjà créé des motifs et des agents et que vous choisissez désormais un fonctionnement basé sur les services, il faudra associer vos motifs au service nouvellement activé, ainsi que rattacher vos agents aux services correspondants.
{% endhint %}

En effet, pour profiter des fonctionnalités de cloisonnement et de visibilité, vous devez activer les services, puis répartir vos motifs et vos agents dans les services que vous venez de créer.

</details>

## Les organisations

<details>

<summary><strong>À quoi servent les organisations ?</strong></summary>

Les organisations permettent de gérer différents sites de rendez-vous au sein de la même entité administrative. Par exemple, une commune peut avoir plusieurs organisations : mairie, CCAS, médiathèque, etc. Cette fonctionnalité est utile si vous souhaitez créer des cloisonnements entre les agents de votre structure.&#x20;

En effet, créer plusieurs organisations permet de **cloisonner** vos agents selon le lieu d'exercice de leurs missions. Un agent d'une organisation (A) n’aura pas accès aux agendas ni aux options d’une autre organisation (B). Bien que vous pouvez, au besoin, associer un agent à plusieurs organisations.&#x20;

</details>

<details>

<summary><strong>À quoi servent les options de configuration d'une organisation ?</strong> </summary>

Une fois l'organisation créée, vous allez pouvoir compléter plusieurs informations depuis le menu paramètre > organisation :&#x20;

* **Nom :**&#x20;
* **Téléphone :**&#x20;
* **Email :**&#x20;
* **Site web :**&#x20;
* **Horaires :**&#x20;

Seul le nom est obligatoire. Toutefois, vous pouvez enrichir ces informations. Elles apparaîtront dans le parcours des prises de rendez-vous en ligne des usagers ainsi que dans le récapitualtif des informations du rendez-vous accessible depuis le SMS ou l'email reçu par les usagers.&#x20;

Ces informations aideront l'usager à vous contacter s'il veut annuler son rendez-vous au moins 4 heures à l'avance. En effet, passé ce délai, l'annulation n'est plus possible.

</details>

<details>

<summary><strong>Comment créer des organisations ?</strong></summary>

Pour créer une nouvelle organisation :&#x20;

* Allez dans le menu _**Espace Admin**_
* Cliquez sur _**Organisations**_ puis sur _**Créer une organisation**_.
* L'agent admin d'espace qui crée l'organisation devient automatiquement le premier agent associé.
* Cet agent admin pourra ensuite inviter d'autres agents dans cette organisation si nécessaire.

**Seul un agent admin d'espace peut créer des organisations.**&#x20;

</details>



Statistiques
