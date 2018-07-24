# Influencer Data

## Objectifs

Ce "test" vise à  évaluer ta capacité à manipuler un set de données et à en extraire des analyses intéressantes. Plus spécifiquement, il s'agit d'évaluer ton aisance:
- à manipuler "beaucoup" de données à partir de fichiers bruts en CSV,
- à imaginer / explorer / réaliser différentes analyses "statistiques",
- et à présenter tes résultats.


## Set de données

Les données proposées sont des données réelles, extraites de la plateforme [YOÔ](www.yoo.paris) que nous avons développée pour l'agence d'influence WOÔ et que nous opérons. Les données ont été extraites courant mai 2018 et anonymisées.

En préambule:
- un `influencer` est une personne qui développe une communauté de followers sur ses réseaux sociaux (Instagram, Facebook, Twitter, etc.) en "postant" régulièrement et en intéragissant avec sa communauté (réponse aux commentaires, likes, etc.). Plus la communauté des followers d'un influencer est grosse et engagée, plus l'influencer est dit "influent". Plus un influencer est influent, plus les "marques" peuvent vouloir réaliser des opérations de communication avec cet influencer: des campagnes d'influences.
- une `campagne d'influence` est une opération de communication à l'occasion de laquelle des influencers vont réaliser des publications sur leurs réseaux sociaux en mettant en avant un produit ou une marque.
- une agence d'influence organise pour le compte de marques des campagnes d'influence en sélectionnant les influencers, en les briefant, en suivant le déroulé de la campagne et en analysant l'efficacité de la campagne.
- La plateforme YOÔ permet à WOÔ de gérer en ligne et automatiquement toutes les étapes d'une campagne d'influence.

Aussi, chaque jour nous collectons pour tous les influencers inscrits sur la plateforme YOÔ, l'ensemble de leurs publications Instagram. Avec ces données, nous pouvons notamment évaluer différentes métriques:
- le nombre de followers d'un influencer (et donc sa capacité à toucher beaucoup de monde lors d'une publication)
- l'engagement moyen: le nombre moyen d'engagements (commentaires et likes) par post pour un influencer
- son taux d'engagement: le nombre d'enagements moyen par post divisé par le nombre de followers de l'influencer. Plus le taux est élevé, plus la "communauté" de l'influencer est engagée.
- les hashtags utilisés: hashtags le plus fréquent, variation des hashtags, etc.

Le set de données proposé dérive de ces données extraites quotidiennement.

### YOO STAT Content Test - raw export

Ce fichier correspond à un extrait des hashtags récupérés. Il comprend pour chaque ligne:

- `post_id` : L'identifiant du post Instagram contenant de hashtag
- `hashtag` : Le hashtag récupéré
- `comments` : Le nombre de commentaires sur ce post
- `like` : Le nombre de likes sur ce post
- `engagement` : Le nombre d'engagements sur ce post (commentaires + likes)
- `post_engagement_rate` : Le rapport du nombre d'engagement sur le nombre de follower en +
- `identity_id` : Un identifiant de l'influencer
- `user_name` : Le username anonymisé de l'influencer
- `number_of_followers` : Le nombre de followers Instagram de l'influencer
- `engagement_rate` : Le taux d'engagement moyen de l'influencer
- `sex` : Le sexe de l'influencer
- `birthdate` : La date de naissance de l'influencer
- `age` : L'âge de 'influencer

NB: Les 2 jeux de données sont indépendants ! Il n'y a pas de correspondances entre les id et les user_nme entre les 2 jeux.


### YOO STAT DISTRIB EXPORT - raw export

Ce fichier correspond à un extrait des influencers inscrits sur YOÔ. Il comprend pour chaque ligne:


- `id`: L'identifiant de l'influencer
- `sex`: Le sexe de l'influencer
- `birthdate`: La date de naissance de l'influencer
- `Year of birth`: L'année de naissance de l'influencer
- `Age`: L'âge de l'influencer
- `user_name`: Le username anonymisé de l'influencer
- `instagram_number_of_posts`: Le nombre de posts en base de données pour cet influencer
- `instagram_number_of_followers`: Le nombre de followers Instagram de l'influencer
- `instagram_average_number_of_comments`: Le nombre de commentaires moyen sur un post de l'influencer
- `instagram_average_number_of_reactions`: Le nombre de likes moyen sur un post de l'influencer
- `instagram_average_engagement`: Le nombre d'engagements moyen (commentaires + likes) sur un post de l'influencer
- `instagram_average_engagement_rate`: Le taux d'engagement moyen constaté sur les posts de l'influencer

NB: Les 2 jeux de données sont indépendants ! Il n'y a pas de correspondances entre les id et les user_nme entre les 2 jeux.

## Instructions

### TODO

Choisis 1 des 2 jeux de données et proposent une analyse de ce jeux de données.

La consigne est volontairement très large, l'idée étant de te donner un champs d'étude ouvert et de te laisser explorer les thèmes que tu souhaites. Voici quelques exemples de "thèmes" (plein d'autres sont possibles !) :
- Existe-il un ou plusieurs influencers type ? Qui sont-ils ?
- Comment varie le taux d'engagement ?
- Peut-on prédire le "succès" d'un post ?
- Y-a-t-il des corrélations contenus - age - sexe ?
- etc.

### Outils

Tu es libre d'utiliser les outils / techno que souhaites: Google Sheet, Excel, Pyhthon, Ruby, etc. On attachera plus d'importance aux analyses / réflexions proposées qu'à la façon dont la donnée a été manipulée.

### Rendu

Tu es libre de proposer un rendu sous forme de slides, de rapport pdf, wiki, readme Github, de page web, etc. On attachera de l'importance à la qualité du rendu et à la présentation de beaux graphiques !
