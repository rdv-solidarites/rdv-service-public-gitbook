# Synchronisation Outlook (Microsoft 365)

Ce document explique comment synchroniser votre calendrier Outlook (Microsoft 365) avec RDV Service Public.

### Distinction des versions d’Outlook <a href="#distinction-des-versions-doutlook" id="distinction-des-versions-doutlook"></a>

Il existe deux versions d’Outlook :

1. Outlook hébergé à distance (Microsoft 365)
2. Outlook hébergé sur place par l’administration (Microsoft Exchange)

{% hint style="warning" %}
**Nous proposons une solution de synchronisation uniquement pour la première version : Outlook hébergé à distance (Microsoft 365)**.
{% endhint %}

Ce guide décrit cette solution. N’hésitez pas à nous contacter si vous avez besoin d’aide pour la mettre en place sur votre territoire.

RDV Service Public ne propose pour l’instant pas de solution de synchronisation clé en main pour Outlook hébergé sur place. Certaines structures utilisant RDV Service Public et ce type d’Outlook ont mis en place des solutions via webhooks, qui nécessitent du développement en interne.

### Fonctionnement <a href="#fonctionnement" id="fonctionnement"></a>

Une application Microsoft Outlook 365 permet aux agents de synchroniser leur agenda RDV Service Public avec leur agenda Microsoft Outlook.

Cette application requiert les droits d’écriture sur les calendriers Outlook.

Elle utilise l’API de Microsoft pour créer et mettre à jour des événements correspondants aux RDV pris dans RDV Service Public.

### Procédure à suivre <a href="#procedure-a-suivre" id="procedure-a-suivre"></a>

Pour que les agents puissent utiliser l’application Microsoft 365, un·e administrateur·ice du compte Outlook du département doit au préalable l’autoriser via un flux OAuth.

{% hint style="info" %}
Cette procédure doit être effectuée une seule fois pour tout un compte Microsoft 365
{% endhint %}

**Étape 1** : L’administrateur·ice Outlook du département doit être invité à créer un compte sur RDV Service Public.

**Étape 2** : Une fois connecté·e sur RDV Service Public, l’administrateur·ice doit cliquer sur son nom en haut à droite > Mon Compte > Synchronisation d’agenda > Connexion Outlook > Se connecter avec Microsoft

![Chemin à suivre pour la connexion Outlook](https://storage.gra.cloud.ovh.net/v1/AUTH_0f20d409cb2a4c9786c769e2edec0e06/padnumerique/uploads/874bafcf-66ea-4a17-b07f-23b1406d3c1b.png)

**Étape 3** : L’administrateur·ice doit accepter les permissions. Il faut nécessairement cocher la case **“Consentement pour le compte de votre organisation”** pour que les agents non-administrateur·ices puissent à leur tour utiliser l’application.

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption><p><em>L’application Oauth est actuellement indiquée comme “non vérifiée” car le processus de validation avec Microsoft n’a pas encore été finalisé.</em></p></figcaption></figure>

### Sécurité et code source <a href="#securite-et-code-source" id="securite-et-code-source"></a>

Pour des raisons de sécurité et de confidentialité, les événements créés dans Outlook ne contiennent pas d’informations personnelles sur les usagers. Ils contiennent uniquement un lien vers RDV Service Public. Ce lien permet à l’agent, une fois authentifié et autorisé, d’accéder aux détails du rendez-vous.

Le code source de RDV Service Public est accessible en open source sur [GitHub (betagouv/rdv-solidarites.fr)](https://github.com/betagouv/rdv-solidarites.fr) :

* **Configuration du client OAuth** : [https://github.com/betagouv/rdv-service-public/blob/production/config/initializers/omniauth.rb#L6](https://github.com/betagouv/rdv-service-public/blob/production/config/initializers/omniauth.rb#L6)
* **Code du client REST** : [https://github.com/betagouv/rdv-service-public/blob/production/app/models/outlook/api\_client.rb](https://github.com/betagouv/rdv-service-public/blob/production/app/models/outlook/api_client.rb)
