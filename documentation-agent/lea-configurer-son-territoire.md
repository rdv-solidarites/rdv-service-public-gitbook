---
icon: map-location
---

# (Léa) Configurer son territoire

Pour découvrir et comprendre l’essentiel des fonctionnalités d’un <mark style="color:red;">**Agent Admin de Territoire**</mark>, nous vous recommandons de consulter le tutoriel ci-dessous.

<details>

<summary>Agents</summary>

En tant qu’**Administrateur d’Espace**, vous avez la possibilité d’inviter des agents à rejoindre votre espace RDV Service Public.

#### Inviter un agent

Pour inviter un agent :

1. Saisissez l’adresse e-mail de l’agent.
2. Sélectionnez le ou les services auxquels il sera affecté.
3. Associez-le à la ou aux organisations concernées.

{% hint style="danger" %}
**Vous devez inviter les agents individuellement. Il n'est pas possible d'envoyer des invitations à plusieurs adresses e-mail simultanément.**

**L’invitation doit être validée par l’agent dans un délai de 48 heures. Passé ce délai, vous devrez procéder à une nouvelle invitation.**
{% endhint %}

Une fois l’invitation envoyée, l’agent recevra un e-mail contenant un lien lui permettant de rejoindre votre espace.\
L’agent devra obligatoirement valider cette invitation avant que vous puissiez gérer ses paramètres.

#### Gérer les agents

Après validation de l’invitation par l’agent, vous pourrez :

* Modifier ses affectations aux services et organisations.
* Définir ou ajuster ses droits d’accès au sein de chaque organisation.

</details>

<details>

<summary>Webhook </summary>



</details>

<details>

<summary>Fiches usagers</summary>

En tant qu’**Administrateur d’Espace**, vous pouvez personnaliser les informations affichées dans les fiches usagers.

Vous avez la possibilité :

* D’**ajouter des champs personnalisés** qui seront visibles dans les fiches usagers.
* De **masquer certains champs standards** que vous ne souhaitez pas afficher.

Ces ajustements vous permettent d’adapter les fiches aux besoins spécifiques de votre organisation et de vos agents.

{% hint style="warning" %}
**Les modifications que vous apportez s’appliqueront à l’ensemble des organisations et des services de votre espace.**
{% endhint %}



</details>

<details>

<summary>Fiches RDV </summary>

Vous avez la possibilité de personnaliser l’affichage des **fiches RDV** en activant ou désactivant certains champs selon les besoins de vos organisations.

**Champ Contexte**

Le champ **Contexte** permet aux agents, lors de la prise de rendez-vous, d’ajouter des informations complémentaires utiles à la gestion du rendez-vous.\
Ces informations sont :

* **Uniquement visibles en interne**, par les agents disposant des droits d’accès au rendez-vous concerné.
* Non accessibles aux usagers.

{% hint style="warning" %}
**Lorsque ce champ est désactivé, il est masqué dans l’interface.**\
**Les informations déjà saisies resteront enregistrées mais ne seront plus visibles.**
{% endhint %}

#### Salle d’attente

Vous pouvez également configurer les paramètres liés à la **salle d’attente**, notamment :

* Définir le **mode de notification des agents** lorsqu’un usager est présent en salle d’attente (notification visuelle, par mail).

Ces options vous permettent d’adapter l’organisation de la prise en charge selon les pratiques internes de votre structure.

</details>

<details>

<summary>Motifs </summary>

Le motif est la raison du rendez-vous. Il permet de catégoriser les prises de rendez-vous, d’informer l’agent sur le contenu attendu et d’affiner les options (présentiel, téléphone, visio, option de prise de rendez-vous en ligne).&#x20;

En tant qu’Administrateur, vous pouvez créer des **motifs à l’échelle de votre espace**. Cela vous permet de mutualiser les motifs entre plusieurs organisations, sans avoir à les recréer pour chacune.&#x20;

Lors de la création, vous pouvez sélectionner les **organisations concernées** par ce motif.

La configuration d’un motif s’effectue via 3 onglets :

***

#### **Information générale**&#x20;

Un motif est avant tout un objet de rendez-vous qui se configure par un nom, une durée par défaut, un type et un service associé.&#x20;

{% hint style="success" %}
**Vos motifs seront accessibles par les agents des services associés**
{% endhint %}

Les agents pourront créer des plages de disponibilités avec des motifs configurés et ainsi faciliter la recherche de créneaux dans votre organisation et planifier des rendez-vous.

Si vous souhaitez proposer plusieurs modalités de rendez-vous (sur place, par téléphone, par visioconférence ou à domicile) ou plusieurs durée par défaut (30 minutes ou 60 minutes) pour un même motif, il sera nécessaire de dupliquer et créer plusieurs motifs.&#x20;

***

#### **Réservation en ligne**&#x20;

Un motif peut-être ouvert ou non à la prise de rendez-vous en ligne. Vous pouvez sélectionner cette option depuis l'onglet _**réservation en ligne**_ de l'écran de configuration des motifs. Vous devez cocher la case _ouvert aux usagers_.&#x20;

{% hint style="success" %}
**Une pastille&#x20;**_**en ligne**_**&#x20;s'affichera pour chaque motif.**&#x20;
{% endhint %}

Dès lors que vous ouvrez la prise de rendez-vous en ligne pour un motif, vous accéderez à des options de configurations supplémentaires liées au **délais minimum et maximum de réservation**. En configurant ces options, vous pouvez limiter la visibilités des disponibilités des plages de disponibilités des agents dans le parcours de prise de rendez-vous en ligne.

Aussi, vous pouvez offrir la possibilité à vos usagers de **modifier leur créneau de rendez-vous en autonomie**. Un bouton déplacer le RDV s'affichera depuis leur récapitulatif de rendez-vous accessible depuis les notifications email et SMS.&#x20;

***

#### **Instruction et notification**

Vous pouvez personnaliser des instructions de rendez-vous, motif par motif. Vous pouvez personnaliser ces instructions depuis l'onglet _**notification et instruction.**_&#x20;

Cette fonctionnalité permet de faire afficher ces instructions :&#x20;

* **Avant le rendez-vous** : dans le parcours en ligne, avant qu'un usager sélectionne un créneau

- **Après le rendez-vous** : dans l'écran de confirmation du rendez-vous ainsi que dans la notification SMS, via l'URL _info/annulation_ et dans la notification email, via le champ _information supplémentaires_

</details>

<details>

<summary>Services </summary>

Vous pouvez gérer les services auxquels vos agents peuvent être affectés dans les différentes organisations.

Vous avez la possibilité d’**activer un service** pour qu’il soit disponible dans votre espace.

Vous pouvez également **désactiver un service**. Les agents ne pourront alors plus être affectés à ce service.

Si le service souhaité n’apparaît pas dans la liste proposée, vous pouvez **en faire la demande en nous contactant via ce** [**formulaire**](https://rdv.anct.gouv.fr/aide/demande_support/new?role=agent\&sujet=Ajout+d%E2%80%99un+service).

</details>

<details>

<summary>Organisations </summary>

En tant qu’administrateur, vous pouvez accéder à la liste de vos organisations présentes dans votre espace et consulter ou modifier leur configuration.

Vous avez également la possibilité d’ajouter une nouvelle organisation à votre espace.

</details>
