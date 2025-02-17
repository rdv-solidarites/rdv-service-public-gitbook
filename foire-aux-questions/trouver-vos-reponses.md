---
icon: message-question
---

# Trouver vos réponses

## Synchronisation calendrier

<details>

<summary><strong>Comment synchroniser avec mon agenda ?</strong></summary>

Cette fonctionnalité permet d'envoyer les informations des rendez-vous planifié dans un agenda extérieur à RDV Service Public. Elle répond au besoin de faire afficher les rendez-vous planifié dans un agenda du quotidien, souvent utilisé dans les administrations pour gérer leur quotidien métier en dehors des rendez-vous (réunion d'équipe etc ...)

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

## Notification agents

<details>

<summary><strong>Comment recevoir des notifications d’alertes de rendez-vous ?</strong></summary>

Cette fonctionnalité permet de recevoir des notifications par email lorsqu’un rendez-vous est ajouté, modifié ou annulé dans un agenda. Elle répond au besoin des agents souhaitant être alertés en cas de changement dans leur planning.

Vous pouvez personnaliser vos préférences de notification dans l’onglet **"Mon Compte"**, accessible en cliquant sur votre prénom en haut à droite de votre calendrier.

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

Cette autorisation est appliquée à titre individuel et vos collègues auront potentiellement le même problème. Vous pouvez suggérer au responsable technique de votre administration de consulter [cette page](../documentation-technique/informations-pour-les-dsi.md) pour corriger ce problème pour tout le monde.

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

Si vous vous retrouvez dans cette situation, il est probable que plusieurs de vos collègues soient dans la même situation. Vous pouvez suggérer aux responsables techniques de votre SI de consulter [cette page](../documentation-technique/informations-pour-les-dsi.md) pour corriger le problème durablement et à l’échelle de tout votre service.

</details>

## Prise de rendez-vous en ligne

<details>

<summary><strong>Comment mettre en place de la prise de rende-vous en ligne ?</strong></summary>

Cette fonctionnalité permet aux usagers d’accéder aux disponibilités de votre organisation et de planifier un rendez-vous en toute autonomie, depuis un ordinateur ou un téléphone.

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

<summary><strong>Puis-je utiliser une solution d'intégration type iFrame sur mon site internet ?</strong> </summary>

Nous ne proposons pas encore ce type d'ingtégration. Nous proposons une intégration simple via un URL à intégrer dans votre site internet :&#x20;

* soit directement en corps de texte d'une page web
* soit via un bouton CTA avec l'URL en hyperlien.&#x20;

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

<details>

<summary><strong>Comment donner accès à mes disponiblités à des partenaires ?</strong> </summary>

La fonctionnalité **prescripteur** permet à un partenaire extérieur (ex. : association, administration, collectivité) de planifier des rendez-vous pour un usager dans vos disponibilités. Cela facilite le parcours des usagers en permettant à différentes entités administratives de rediriger les usagers vers un rendez-vous dans votre structure.&#x20;

#### **Comment ça fonctionne ?**

1. **Configuration** : Activez des motifs de rendez-vous ouverts à la réservation en ligne dans vos disponibilités.
2. **Partage de l'URL** : Envoyez l'URL de réservation en ligne à vos partenaires.&#x20;
3. **Notifications** :
   * **Prescripteur** : Reçoit un e-mail de confirmation du rendez-vous.
   * **Usager** : Reçoit une confirmation et un rappel 48 heures avant le rendez-vous.
   * **Professionnel** : Le rendez-vous apparaît dans son agenda, avec synchronisation possible.

**Que doit faire un prescripteur ?**

1. Accédez à la **prise de rendez-vous en ligne** et sélectionnez :
   * **Motif du rendez-vous**
   * **Créneau de rendez-vous**
2. Cliquez sur **"Je suis un prescripteur qui oriente un bénéficiaire"**.
3. Saisissez vos coordonnées et celles de l'usager.
4. Confirmez le rendez-vous. Un récapitulatif sera généré à la fin.

</details>

## Notification usagers

<details>

<summary><strong>Puis-je modifier les informations du SMS ?</strong> </summary>

Il n’est pas possible de modifier le modèle SMS : le nombre de caractères pour les SMS est limité. Aussi certaines informations comme le nom du motif peut porter atteinte à l’usager. Nous avons donc fait le choix de limiter les informations.

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

<summary><strong>Qu’est-ce que peut faire un usager depuis ces notification SMS ?</strong></summary>

Chaque usager recevra une notification par SMS et/ou email.

* Le SMS contiendra un lien "Infos/Annulation".
* En cliquant dessus, il accèdera à une page web où il devra saisir les trois premières lettres de son nom de famille.
* S'il les saisit correctement, il verra un récapitulatif de son rendez-vous avec les instructions associées ainsi que les informations de contact de votre organisation.&#x20;

Un bouton "Annuler le rendez-vous" lui permettra d’annuler sans vous contacter, jusqu’à **4 heures avant** l’heure prévue. Au-delà, il devra vous contacter via les informations de contact disponible dans le récapitulatif de rendez-vous. &#x20;

</details>

## Les agendas et les rendez-vous

<details>

<summary><strong>Qui peut voir et modifier mon agenda ?</strong> </summary>

Par défaut, seuls les agents de votre service et de votre organisation peuvent consulter et planifier des rendez-vous dans votre agenda. De plus, les agents du service secrétariat de votre organisation ont un accès étendu : ils peuvent voir, modifier et planifier des rendez-vous de tous les agendas.&#x20;

</details>

<details>

<summary><strong>Comment utiliser les plages d’ouvertures ?</strong></summary>

Les plages d’ouverture permettent de définir les disponibilités d’un agent. Une fois configurées, elles simplifient la prise de rendez-vous : les agents peuvent directement rechercher un créneau via le bouton "Trouver un RDV", évitant ainsi une consultation fastidieuse des agendas individuels.

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

Les indisponibilités permettent de signaler vos absences ponctuelles ou régulières à vos collègues et aux usagers. Cette fonctionnalité évite de modifier les plages d'ouvertures en cas d'indisponiblité ponctuelle des agents. Si une indisponibilité couvre la période d'une plage d'ouverture, les disponibilités de cette période seront supprimées.

Pour créer une indisponibilité :

1. Accédez au menu _**planning**_
2. Sélectionnez _**indisponibilité**_
3. Cliquez sur "créer une indisponibilité"
4. Renseignez les informations demandées

Vous pouvez configurer des absences ponctuelles ou récurrentes en utilisant l'option _**répéter**_.

Les indisponibilités apparaissent en gris sur votre agenda et ceux de vos collègues.&#x20;

Pour une indisponibilité récurrente, il n'est pas possible de supprimer une seule occurrence. Vous devrez supprimer l'indisponibilité récurrente entière et en créer une nouvelle excluant l'occurrence non désirée.

</details>

<details>

<summary><strong>Comment trouver une disponibilité chez les agents de mon organisation ?</strong></summary>

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

<summary><strong>Puis-je modifier ou supprimer les données des usagers ?</strong> </summary>

Vous pouvez supprimer ou modifier les données des usagers. Sur la fiche des usagers, des options Modifier et Supprimer sont prévues à cet effet. Si aucunes modifications n’est apportée et que l’usager n’a pris aucun RDV durant deux ans, alors ses données seront supprimées automatiquement.

</details>

<details>

<summary><strong>Comment créer une fiche usager ?</strong></summary>

Pour créer une fiche :&#x20;

1. Dans le menu **"Usager"**, cliquez sur **"Créer un usager"** ou depuis le parcours **"Trouver un RDV"** cliquer sur **"Créer un usager"**
2. Seuls le nom et le prénom sont obligatoires.
3. La fiche sera rattachée à **l’organisation de l’agent** qui l’a créée.
4. Cliquez sur **"Créer usager"** pour valider.

**💡 Vérifiez l’orthographe des noms et prénoms pour éviter les doublons.**

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

**💡 L’outil ne fusionne pas automatiquement les fiches, car l’unicité repose uniquement sur l’e-mail.**

Pour fusionner des fiches usagers :&#x20;

1. Allez dans le menu **"Usagers"**.
2. Cliquez sur **"Fusionner deux usagers"**.
3. Entrez le nom de l’usager en double dans chaque colonne.
4. Comparez les fiches :
   * **Différences en orange**, **similitudes en vert**.
   * Sélectionnez les informations à conserver.
5. Validez pour créer une **fiche unique fusionnée**.

</details>

## Les agents

<details>

<summary><strong>Puis-je associer un agent à plusieurs organisations ?</strong> </summary>

Un agent peut être associé à plusieurs organisations. Cette association lui donnera accès aux agendas des agents rattachés à son service dans chacune de ces organisations. Seul un agent administrateur de territoire peut associer un agent à plusieurs organisations.

Pour ajouter un agent à plusieurs organisations :&#x20;

* Accéder à votre Espace Admin&#x20;
* Sélectionner "Agent"&#x20;
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

💡 **Sa visibilité est limitée aux agents de son service et de son organisation. Pour associer un agent à plusieurs services ou organisations.**&#x20;

#### **Agent Admin**

L'**Agent Admin** a une **visibilité étendue** sur toutes les organisations auxquelles il est associé. Il peut :

* Rechercher des disponibilités dans tous les services de son organisation,
* Accéder à l'onglet **Paramètres** pour créer des motifs, lieux et inviter des agents,
* Être associé à plusieurs organisations.

#### **Agent Admin de Territoire**

L'**Agent Admin de Territoire** a une **visibilité totale** sur tous les agendas du territoire et tous les services/organisations. Il a également accès aux paramètres de tous les services et organisations du territoire et peut :

* Modifier les droits d'accès des agents,
* Créer des organisations et former des équipes.

💡 **Plusieurs Agents Admin de Territoire peuvent être définis.**&#x20;

#### **Agent Secrétariat**

Un **Agent du service secrétariat** bénéficie de droits de visibilité supérieurs. Il peut :

* Rechercher des disponibilités sur tous les agendas de l'organisation mais avec des droits d'un agent basique.&#x20;
* Planifier des rendez-vous dans n'importe quel agenda de l'organisation (tous services confondus).\
  Sa principale fonction est de planifier des rendez-vous, mais il peut aussi planifier dans son propre agenda.

💡 **Un Agent Admin doit ouvrir les motifs de prise de rendez-vous pour les agents du service secrétariat s'ils doivent réaliser des rendez-vous.**&#x20;

</details>

<details>

<summary><strong>Comment inviter des agents dans mon organisations ?</strong></summary>

Pour inviter un agent :&#x20;

1. Allez dans **"Paramètres"**, puis **"Agents"**.
2. Cliquez sur **"Inviter un agent"**.
3. Choisissez un niveau d'accès.&#x20;
4. Entrez l’adresse e-mail de l'agent.&#x20;
5. Enfin, sélectionnez un service auquel associer l'agent.&#x20;
6. Il recevra une invitation pour créer son compte. Une fois l’invitation acceptée, l'agent devra créer un mot de passe pour se connecter.&#x20;

💡 **Si vous invitez un agent dans plusieurs organisations, chaque invitation sera validée automatiquement après la première, sans nouvel email d'invitation.**&#x20;

</details>

<details>

<summary><strong>Comment modifier le services d’un agent ?</strong></summary>

Pour modifier le service d'un agent :&#x20;

* Accéder à votre espace Admin de Territoire&#x20;
* Cliquer sur "agent" et sélectionner "modifier".&#x20;
* Associer l'agent à un ou plusieurs services pour définir ses droits d'accès.&#x20;

**💡 Seul un agent admin de territoire pour modifier les services d'un agent.**&#x20;

</details>

<details>

<summary><strong>Comment supprimer un agent ?</strong> </summary>

Pour supprimer un agent :&#x20;

1. Allez dans **"Paramètres"**, puis **"Agents"**.
2. Cliquez sur l’icône **"Supprimer"** à côté de l'agent.
3. Si l'agent a des rendez-vous à venir, une alerte vous empêchera de le supprimer. Vous devrez réaffecter ces rendez-vous avant de supprimer l'agent.

**💡 Les agents inactifs (non connectés depuis 30 jours) auront l’étiquette "inactif" à côté de leur nom.**

</details>

## Les motifs

<details>

<summary><strong>À</strong> <strong>quoi servent les motifs ?</strong> </summary>

Le motif est la raison du rendez-vous. Il permet de catégoriser les prises de rendez-vous, d’informer l’agent sur le contenu attendu et d’affiner les options (présentiel, téléphone, visio, option de prise de rendez-vous en ligne). Il permet également une configuration fine des disponibilités des agents selon leurs compétences ou capacités dans leurs plages d'ouverture.&#x20;

</details>

<details>

<summary><strong>Comment créer et configurer un motif ?</strong></summary>



</details>

<details>

<summary><strong>Puis-je modifier des motifs en masse ?</strong> </summary>



</details>

## Les services&#x20;

<details>

<summary><strong>Comment activer un nouveau service ?</strong> </summary>

Par défaut, lors de la création de votre compte, un seul service sera actif dans votre territoire. Vous pourrez activer d'autres services pour y associer des agents selon vos besoins.

Pour activer un nouveau service, rendez-vous dans le menu _**espace admin**_ accessible depuis le menu _**paramètres**_. Vous y trouverez un menu _**services**_ où vous pourrez activer des services à partir d'une liste préétablie.

**-> Sélectionnez le service que vous souhaitez activer sur votre territoire.**

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

1. Allez dans le **menu "Espace Admin"** depuis **Paramètres**.
2. Cliquez sur **"Organisations"**, puis sur **"Créer une organisation"**.
3. L'agent admin de territoire qui crée l'organisation devient automatiquement le premier agent associé.
4. Cet agent admin pourra ensuite inviter d'autres agents dans cette organisation si nécessaire.

**💡 Seul un agent admin de territoire pour créer des organisations.**&#x20;

</details>



Statistiques
