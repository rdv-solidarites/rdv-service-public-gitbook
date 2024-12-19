---
icon: circle-check
description: >-
  Cette page détaille les différentes manières de synchroniser vos RDV pris via
  RDV Service Public dans un logiciel de calendrier externe (Outlook,
  Thunderbird…)
---

# Synchronisation avec un logiciel de calendrier externe

## Notes générales&#x20;

RDV Service Public propose différents mécanismes de synchronisation. Voici quelques remarques importantes valables pour tous les mécanismes :

* Pour protéger les données personnelles de vos usagers, les événements envoyés à votre logiciel de calendrier externe ne contiendront que le motif, l'adresse du rendez-vous et un lien vers les détails dans RDV Service Public ;&#x20;
* Nous proposons de synchroniser les créations, changements et annulations depuis RDV Service Public vers les logiciels de calendrier externes mais pas l’inverse. Si vous supprimez un RDV depuis votre logiciel de calendrier externe, cela ne sera pas répercuté dans RDV Service Public et l’usager n’en sera pas averti.

## S**ynchronisation par email**

Cette synchronisation envoie un email pour chaque création, modification ou annulation de RDV.&#x20;

Chaque email contient une pièce jointe au format ICS, un format largement supporté. Votre logiciel de calendrier externe reconnaîtra ces emails et mettra automatiquement à jour les évènements dans votre calendrier. Certains logiciels de calendrier demandent « d’accepter » chaque modification.

Vous pouvez modifier vos préférences de notifications email dans l’espace « Mon Compte » accessible en cliquant sur votre prénom en haut à droite depuis votre vue calendrier.

## **Synchronisation Webcal**

Webcal est un protocole largement supporté par les logiciels de calendrier.&#x20;

Nous vous fournissons une URL individuelle fournissant le contenu de votre agenda au format ICS. Cette URL peut être récupérée depuis dans l’espace « Mon Compte » accessible en cliquant sur votre prénom en haut à droite depuis votre vue calendrier. Il suffit de copier cette URL dans votre logiciel de calendrier externe et la synchronisation se fera automatiquement.

Si vous synchronisez votre agenda RDV Solidarités avec Google Agenda, la mise à jour peut prendre jusqu'à 12 heures. Avec le calendrier Outlook, l'affichage est plus rapide, généralement dans l'heure suivant la prise de rendez-vous.

{% hint style="danger" %}
La synchronisation WebCal n’est pas instantanée. \
\
La fréquence de mise à jour dépend de chaque logiciel de calendrier externe. Avec Google Agenda par exemple, la mise à jour peut prendre jusqu’à 12h. Avec Outlook, cette fréquence est généralement d’environ une heure mais chaque logiciel peut se comporter différemment.
{% endhint %}

## Synchronisation spécifique Outlook

Il existe deux grandes versions d'Outlook :&#x20;

* Outlook hébergé à distance, aussi appelé Microsoft 365
* Outlook hébergé sur place par l’administration, aussi appelé Microsoft Exchange

Nous avons un prototype de synchronisation spécifique pour la version hébergée à distance (Microsoft 365). N’hésitez pas à nous contacter si vous souhaitez l’expérimenter sur votre territoire.&#x20;

Nous ne fournissons pour l’instant pas de solution spécifique pour Outlook hébergé sur place (Microsoft Exchange). Certaines structures utilisant RDV Service Public et ce type d’Outlook ont cependant mis en place des solutions via webhooks (voir ci-dessous).

## Synchronisation via webhooks

{% hint style="info" %}
Cette solution demande du développement spécifique en interne par votre DSI.
{% endhint %}

Les webhooks sont une manière de communiquer entre deux systèmes d’information. Nous proposons d’émettre des webhooks vers le SI de votre organisation.&#x20;

Il est possible de développer un logiciel dans votre SI pour recevoir ces webhooks et mettre à jour les calendriers des agents en conséquence. Cette solution est déjà en place dans plusieurs structures utilisant RDV Service Public.

Vous trouverez des informations techniques ici : [https://github.com/betagouv/rdv-service-public/blob/production/docs/api/webhooks/api-notifications-webhooks.md](https://github.com/betagouv/rdv-service-public/blob/production/docs/api/webhooks/api-notifications-webhooks.md)



