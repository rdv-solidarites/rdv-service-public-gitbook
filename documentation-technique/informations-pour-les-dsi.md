---
description: >-
  Cette page s’adresse aux responsables des services d’informations dans des
  administrations ou organismes qui utilise RDV Service Public ou RDV
  Solidarités
icon: gear
---

# Informations pour les DSI

### Les emails de RDV Service Public ne sont pas reçus par les agents

Veuillez dans un premier temps prendre connaissance de cette page qui explique les problèmes fréquents pour les agents et les solutions :&#x20;

{% content-ref url="../documentation-agents/problemes-de-reception-des-emails.md" %}
[problemes-de-reception-des-emails.md](../documentation-agents/problemes-de-reception-des-emails.md)
{% endcontent-ref %}

Si un des agents de votre service rencontre ce genre de problèmes de réception d’emails, il est probable que d’autres le rencontrent à leur tour.

En tant que responsable technique vous avez la possibilité de configurer le SI pour corriger ces problèmes pour tous les agents.

Le but est de faire en sorte que les serveurs mails de votre SI ne refusent jamais les emails envoyés par RDV Service Public. L’idée est de mettre sur une liste d’acceptations tous les mails émis par RDV Service Public (on parle aussi de _whitelist_).

Il faut le cas échéant faire cette configuration à deux niveaux :&#x20;

* le système de détection de spam natif du serveur mail de votre SI
* le(s) logiciel(s) de filtrage d’email branchés sur votre serveur comme MailInBlack

Le plus robuste est d’ajouter dans les listes d’acceptations l’adresse IP suivante : \`212.146.241.127\`. Nous envoyons tous nos emails depuis cette adresse.

Si vous ne trouvez pas l’option pour ajouter une IP dans une liste d’acceptation, vous pouvez en repli ajouter les domaines émetteurs suivants comme domaines de confiance  :&#x20;

<details>

<summary>domaines de confiances</summary>

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

</details>

N’hésitez pas à nous contacter à support@rdv-service-public.fr pour que nous puissions vous aider à faire ces configurations.
