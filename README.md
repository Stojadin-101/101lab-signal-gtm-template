# 101lab Signal - template Google Tag Manager

**Le consentement qui fiabilise vos signaux Google et Meta.**

Template GTM de **101lab Signal**, la plateforme de gestion du consentement (CMP) de [101lab](https://101-lab.com), compatible Google Consent Mode v2.

> 101lab Signal n'a aucun lien avec Google Signals (GA4) ni avec Meta Signals Gateway.

## Ce que fait le template

- Pose les valeurs par défaut du Consent Mode v2 :
  - refusé dans les pays configurés (par défaut EEE, Royaume-Uni, Suisse, Serbie) ;
  - accordé ailleurs ;
  - `security_storage` toujours accordé.
- Réapplique le choix déjà mémorisé du visiteur, sans recharger le bandeau.
- Sinon, charge le bandeau de consentement 101lab Signal depuis une URL figée et versionnée sur `cdn.101-lab.com`. C'est le seul script injecté, et aucun service tiers n'est appelé avant le consentement.

## Installation

1. Ajouter le modèle « 101lab Signal - Consent Mode v2 » depuis la galerie de modèles de la communauté, ou importer `template.tpl`.
2. Créer une balise avec ce modèle et renseigner au minimum l'URL de la politique de confidentialité.
3. Déclencheur : **Consent Initialization - All Pages**.
4. Tester en mode Aperçu avant de publier le conteneur.

## Réglages

- **Consent Mode :** pays où le bandeau s'affiche, `wait_for_update`, `ads_data_redaction`, `url_passthrough`.
- **Apparence :** logo, couleurs, police, lien « Powered by 101lab ».
- **Textes :** surtitre, titre et introduction du bandeau.
- **Cookies :** tableau des cookies par catégorie.
- **Configuration avancée :** JSON.

## Versions

| Version | Script chargé |
|---|---|
| 2.0.1 | `https://cdn.101-lab.com/signal/2.0.1/101lab-signal.min.js` |
| 2.0.0 | `https://cdn.101-lab.com/signal/2.0.0/101lab-signal.min.js` |

## Licence

Le code du template est sous licence Apache 2.0 (voir `LICENSE`). Le script du bandeau chargé par le template est la propriété de 101lab.
