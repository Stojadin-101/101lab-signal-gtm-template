# 101lab Signal - template Google Tag Manager

**Le consentement qui fiabilise vos signaux Google et Meta.**

Template GTM de **101lab Signal**, la plateforme de gestion du consentement (CMP) de [101lab](https://101-lab.com), compatible Google Consent Mode v2.

> 101lab Signal n'a aucun lien avec Google Signals (GA4) ni avec Meta Signals Gateway.

## Ce que fait le template

- Pose les valeurs par défaut du Consent Mode v2 sur le déclencheur « Consent Initialization - All Pages » :
  - refusé dans les pays configurés (par défaut EEE, Royaume-Uni, Suisse), accordé ailleurs ;
  - `security_storage` toujours accordé.
- Réapplique le choix déjà mémorisé du visiteur.
- Sinon, charge le bandeau de consentement 101lab Signal depuis une URL figée et versionnée.

## Statut

En préparation : le template sera publié ici lors de la première version (2.0.0).

Ce dépôt suit la structure demandée par la [galerie de modèles de la communauté GTM](https://developers.google.com/tag-platform/tag-manager/templates/gallery). Le code du template sera sous licence Apache 2.0.
