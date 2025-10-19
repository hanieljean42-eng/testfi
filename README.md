# 💕 Je Teste Mon Partenaire - Guide d'installation et d'utilisation

## Description

"Je Teste Mon Partenaire" est une application web interactive qui permet aux utilisateurs d'évaluer la fidélité et la confiance dans leur relation. Les utilisateurs remplissent un questionnaire et reçoivent un score ainsi qu'un message indicatif sur leur relation.

L'application envoie également les résultats de manière sécurisée au créateur via EmailJS.

## Fonctionnalités

* Page d'inscription avec nom, email, nom du partenaire et durée de la relation.
* Questionnaire de 10 questions avec options multiples.
* Barre de progression indiquant l'avancement.
* Résultat affiché avec pourcentage et message indicatif.
* Envoi automatique des résultats à l'adresse configurée via EmailJS.
* Modal pour afficher les conditions d'utilisation.

## Technologies Utilisées

* HTML5
* CSS3
* JavaScript (vanilla)
* EmailJS v4 pour l'envoi d'emails

## Installation

1. Cloner ou télécharger le projet.
2. Ouvrir le fichier `index.html` dans un navigateur web.
3. Vérifier que vous êtes connecté à Internet pour que EmailJS fonctionne.

## Configuration EmailJS

1. Créer un compte sur [EmailJS](https://www.emailjs.com/).
2. Créer un **service** (exemple: `service_eohctur`).
3. Créer un **template** (exemple: `template_gqz33dm`) avec les variables suivantes :

   ```
   {{from_name}}, {{from_email}}, {{partner_name}}, {{relationship_duration}}, {{test_score}}, {{total_score}}, {{max_score}}, {{answers_detail}}, {{completion_date}}, {{security_code}}
   ```
4. Récupérer la **clé publique** (exemple: `KUgeC6svqfm7r4DTa`).
5. Vérifier que les IDs et la clé dans le fichier `index.html` correspondent.

## Usage

1. L'utilisateur remplit le formulaire d'inscription.
2. L'utilisateur coche la case pour accepter les conditions d'utilisation.
3. L'utilisateur répond à toutes les questions du questionnaire.
4. Les réponses sont automatiquement envoyées via EmailJS.
5. L'utilisateur voit son score et un message indicatif.
6. L'utilisateur peut recommencer le test en cliquant sur "Recommencer un test".

## Personnalisation

* Modifier les questions et options dans le tableau `questions` dans le script JavaScript.
* Changer les couleurs et styles dans la section CSS selon votre charte graphique.

## Support

Pour toute question ou problème, contacter : `hanieljean42@gmail.com`.

---

**Note :** Ce test est indicatif et ne remplace pas une communication ouverte dans votre couple.
