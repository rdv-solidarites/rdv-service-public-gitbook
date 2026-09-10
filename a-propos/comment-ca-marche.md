---
icon: gear
layout:
  width: default
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: false
  metadata:
    visible: true
  tags:
    visible: true
  actions:
    visible: true
---

# Comment ça marche ?

Conçue pour s'adapter aux diverses réalités des administrations publiques, RDV Service Public s'articule autour de 3 niveaux d'accès et d'une architecture en 4 concepts.&#x20;

La solution offre une grande liberté : aucune limite n'est imposée quant au nombre de services, d'agents ou d'organisations. De plus, vous disposez d'une totale autonomie pour créer et ajuster chaque configuration. Cela permet notamment un déploiement progressif, que ce soit organisation par organisation ou service par service.

***

## Les niveaux de permission

### <mark style="color:blue;">Agent Basique</mark>

Le statut Agent Basique est le premier niveau d'accès. Il permet d'utiliser toutes les fonctionnalités de planification de rendez-vous. L'agent peut créer des fiches usagers, planifier des rendez-vous et rechercher des disponibilités dans les agendas de ses collègues. Cependant, sa visibilité est limitée aux agendas des _**agents**_ de son _**service**_ et de son _**organisation**_.&#x20;

{% hint style="info" %}
**Vous pouvez associer un Agent Basique à plusieurs services ou plusieurs organsiations au besoin.**&#x20;
{% endhint %}

### <mark style="color:green;">Agent Admin</mark>

Un Agent Admin bénéficie d'une visibilité étendue sur l'ensemble des organisations auxquelles il est associé, tous services confondus. Il peut rechercher des disponibilités dans tous les services de son organisation.

Un Agent Admin a accès à l'onglet _**paramètres**_. Cela lui permet de créer des _**motifs**_, des _**lieux**_ et d'inviter des _**agents**_ dans l'_**organisation**_ à laquelle il est rattaché.&#x20;

{% hint style="info" %}
**Vous pouvez associer un** **Agent Admin** **à plusieurs organisations.**&#x20;
{% endhint %}

### <mark style="color:red;">Agent Admin d'Espace</mark>

Un Agent Admin d'Espace a visibilité et a accès aux options de configuration sur tous les _**services**_ et toutes _<mark style="color:purple;">**o**</mark>**rganisations**_ de l'_**espace**_.&#x20;

Un Agent Admin d'Espace a accès à l'_**espace admin**_. Cet espace lui permet de modifier les droits d'accès de certains agents, de créer des organisations et de former des équipes.

{% hint style="info" %}
**Vous pouvez disposer de plusieurs Agents Admin d'Espace dans votre espace.**
{% endhint %}

***

## L'architecture

### L'Espace

L'Espace est votre compte dans RDV Service Public où vous intégrez vos _**organisations**_, vos _**services**_ et vos _**agents**_.&#x20;

<figure><img src="../.gitbook/assets/Capture d’écran 2025-07-01 à 14.49.54.png" alt=""><figcaption></figcaption></figure>

### Les organisations

Les _**organisations**_ sont les structures physiques, les sites dans lesquels sont planifiés les rendez-vous et où travaillent les agents. Chaque _**organisation**_ est donc obligatoirement associée à un espace, c'est-à-dire à une entité administrative.

{% hint style="info" %}
**Une organisation symbolise un lieu où des agents travaillent et planifient des rendez-vous.**
{% endhint %}

Par exemple, la Maison des Solidarités de Vernoux et la Maison des Solidarités d'Annonay sont deux organisations du département de l'Ardèche (espace). Vous pouvez créer autant d'organisations que nécessaire !

{% hint style="warning" %}
**Chaque organisation peut créer plusieurs lieux. Par défaut, chaque organisation aura un seul lieu (l'adresse de l'organisation). Toutefois, si votre organisation gère des permanences ou des antennes à l'extérieur, vous pouvez créer des lieux supplémentaires**
{% endhint %}

<figure><img src="../.gitbook/assets/Capture d’écran 2025-07-01 à 14.50.06.png" alt=""><figcaption></figcaption></figure>

### Les services

Les services sont rattachés à l'**espace**, c'est-à-dire à l'entité administrative. Les administrations sont généralement organisées en différentes verticales, appelées _**services**_ dans RDV Service Public.

{% hint style="info" %}
**Toutes les organisations de votre espace ont accès aux mêmes services. Une organisation ne peut pas avoir de service qui lui soit propre**.
{% endhint %}

Cette structure permet une organisation plus fine des agents au sein de l'entité administrative globale. Chaque agent est ainsi rattaché à un ou plusieurs _**services**_.

{% hint style="info" %}
**Vous avez la possibilité d'activer ou de désactiver des services dans votre espace.**&#x20;
{% endhint %}

<figure><img src="../.gitbook/assets/Capture d’écran 2025-07-01 à 14.50.31.png" alt=""><figcaption></figcaption></figure>

### Les agents

Les agents sont les utilisateurs de RDV Service Public. Chaque agent obtient un compte utilisateur après avoir été invité par un <mark style="color:green;">Agent Admin</mark> ou un <mark style="color:red;">Agent Admin d'Espace</mark>.&#x20;

<figure><img src="../.gitbook/assets/Capture d’écran 2025-07-01 à 14.50.41.png" alt=""><figcaption></figcaption></figure>

### Exemple 💡

Voici un exemple concret de configuration pour une commune.

La commune de Saint-Péron possède un compte (son espace) et utilise la solution pour gérer ses rendez-vous dans trois sites (ses organisations).

Chaque agent est rattaché à son service au sein de son organisation, ce qui permet de cloisonner l'accès aux informations des usagers et des rendez-vous.&#x20;

<figure><img src="../.gitbook/assets/Capture d’écran 2024-09-25 à 12.47.38.png" alt=""><figcaption></figcaption></figure>

