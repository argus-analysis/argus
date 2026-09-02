# ARGUS Wrapper — Historique des versions

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
