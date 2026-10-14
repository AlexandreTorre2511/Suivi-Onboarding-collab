# Suivi de Mission · Inov Team

Prototype de l'application interne de suivi des collaborateurs en mission. Il couvre le PRD « Suivi de Mission » du wiki GitLab : trois rôles qui suivent les mêmes collaborateurs (managers, RH, commerciaux) et un rôle Admin.

## Fonctionnalités

| Écran | Contenu |
| --- | --- |
| Tableau de bord | Suivis à réaliser, retards, alertes ouvertes, événements spéciaux, derniers échanges tous rôles |
| Collaborateurs | Liste filtrée selon le rôle (un manager ne voit que ses collaborateurs), recherche, synchronisation simulée depuis l'outil RH |
| Profil collaborateur | Prochain jalon par rôle, alertes client et collaborateur, événements spéciaux, résumé des entretiens, missions, historique des suivis, personnes à notifier |
| Suivi | Questionnaire dynamique (texte, choix unique, oui ou non) avec commentaire libre, verrouillé après validation |
| Calendrier | Barre d'aujourd'hui à la date limite tant qu'un suivi n'est pas planifié, planification de rendez-vous, invitation Outlook (.ics) |
| Notifications | Rappels J+1, J+7, J+30 puis récurrents, une relance unique trois jours après l'échéance |
| Templates et jalons (Admin) | Création de questionnaires, activation, versionnage : un template publié n'est jamais modifié |

## Données

Les collaborateurs et les suivis sont des exemples. Ce qui est saisi reste dans le `localStorage` du navigateur : rien n'est envoyé à un serveur. Le bouton « Réinitialiser la démo » remet les données d'exemple.

Le pré-remplissage par IA, le résumé des entretiens et le téléchargement de l'invitation .ics ne fonctionnent que dans la version publiée sur Claude. Sur GitHub Pages, ces boutons sont masqués ou désactivés.

## Lancer en local

Ouvrir `index.html` dans un navigateur. Rien à installer, rien à compiler.

## Mettre en ligne

GitHub Pages : **Settings → Pages → Source : Deploy from a branch → `main` / `(root)`**.
