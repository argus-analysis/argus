# ARGUS Wrapper — Historique des versions

## Wrapper 1.0.0

Cible : ARGUS V5.1.0.

Nature :

Première version publique stabilisée du wrapper d'exécution générique. Elle fixe explicitement sa frontière : exécuter ARGUS fidèlement, indépendamment de tout site, pipeline éditorial ou dispositif de publication.

Changements :
- passage de la série pré-1.0 à 1.0.0 pour déclarer un périmètre public stable ;
- retrait du wrapper public des conventions propres aux Case Studies et de la couche de publication ;
- maintien des règles génériques de 0.6.0 : provenance de l'analyste, portabilité des références, segmentation, contraintes d'environnement et garde-fous correctifs ;
- durcissement prépublication du contrôle de cohérence : toute correction de l'étape 8 qui affecte un mécanisme utilisé en 7.c doit être propagée jusqu'au niveau final ; au seuil 2 → 3, le wrapper impose de distinguer convergence effective des mécanismes et simple accumulation de défauts, avec une démonstration symétrique lorsque le niveau 2 est maintenu, fondée sur les observations candidates effectivement examinées ;
- intégrité inter-passes : dans une adjudication conduite en plusieurs passes, un constat explicitement figé devient une prémisse opératoire de la passe suivante et ne peut être requalifié qu'à partir d'une contradiction factuelle démontrable ou d'un élément matériel auparavant indisponible, identifié et cité ;
- cible normative inchangée : ARGUS V5.1.0.

Non modifié :
- protocole ARGUS V5.1.0 ;
- étapes analytiques ;
- catégories de conclusion ;
- règles de preuve ;
- décisions d'activation des annexes.

Frontière wrapper / protocole : le wrapper public 1.0.0 ne définit aucun site, aucune Case Study, aucune synthèse de publication ni aucun pipeline éditorial. Ces traitements éventuels sont postérieurs à l'analyse et relèvent d'outils séparés.

## Branche 0.7.0 — développement, non publiée

La branche 0.7.0 a servi à expérimenter une couche de synthèse et de publication. Elle n'a jamais remplacé 0.6.0 comme wrapper stable publié. Les fonctions propres à la publication ont été séparées du wrapper public avant 1.0.0.

## Wrapper 0.6.0

Cible : ARGUS V5.1.0 (détecteur de constance modale intégré). Remplace la V5.0.0 comme cible.

Nature :

Extension de traçabilité de l'analyste et mise à jour de cible.

Ajouts :
- formalisation de la provenance de l'analyste en trois champs : modèle, version ou build, intensité de raisonnement ; le champ modèle était déjà présent parmi les métadonnées d'exécution, tandis que la version/build et l'intensité sont ajoutées par 0.6.0 ;
- conservation des métadonnées d'exécution existantes, notamment l'hôte et le régime d'exécution ;
- intensité enregistrée au label du fournisseur, verbatim, sans normalisation sur une échelle commune, les intensités n'étant pas comparables d'un fournisseur à l'autre ; « non exposée » lorsque l'environnement n'en expose aucune, jamais inférée du comportement du modèle ;
- rappel de restitution : signaler la confiance d'un verdict de constance modale rendu près de la frontière révision assumée / rétractation déguisée.

Non modifié :
- protocole ARGUS, hormis l'ajout V5.1.0 lui-même, qui relève du protocole et non du wrapper ;
- étapes analytiques ;
- catégories de conclusion ;
- règles de preuve.

Frontière wrapper / protocole : les champs de provenance et la restitution sont de la métadonnée d'exécution ; les règles du détecteur, annotation modale, contrôle de constance, garde et interactions, sont de protocole et figurent dans le protocole V5.1.0.

## Wrapper 0.5.0

Nature :

Extension de traçabilité et de restitution.

Ajouts :
- principe de neutralité d’entrée explicité ;
- métadonnées d’exécution ;
- couche de publication Case Studies.

Non modifié :
- protocole ARGUS ;
- étapes analytiques ;
- catégories de conclusion ;
- règles de preuve.
