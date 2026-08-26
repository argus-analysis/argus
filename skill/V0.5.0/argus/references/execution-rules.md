# ARGUS — Règles d'exécution du wrapper, révision 0.5.0

Ce fichier règle uniquement des questions d'exécution. Il ne modifie pas ARGUS V5.0.0 et n'introduit aucune catégorie, aucun niveau de gravité, aucun seuil d'activation ni aucune rubrique normative absents du protocole. En cas de conflit, `argus-protocol-fr.md` prévaut.

## 1. Frontière entre protocole et wrapper

Une règle appartient au protocole dès lors que sa suppression changerait un constat ARGUS possible, son niveau de gravité, l'activation d'une annexe ou une conclusion. Le wrapper ne peut régler que la manière d'exécuter, de segmenter, de restituer ou de vérifier matériellement une exigence déjà présente.

Toute analyse complète déclare deux numéros distincts : ARGUS V5.0.0 et wrapper 0.5.0.

## 2. Priorité pratique des vérifications externes

Lorsque plusieurs contrôles simples sont obligatoires ou utiles, les traiter dans cet ordre pratique, sans créer de nouvelle hiérarchie normative :

1. éléments susceptibles de modifier la thèse centrale, la qualification d'un défaut ou sa gravité ;
2. fidélité ou attribution décisive d'une source, d'une citation ou d'un chiffre ;
3. contrôle nécessaire à la qualification d'une absence ou à la symétrie de la vérification ;
4. contexte utile sans effet probable sur le jugement, seulement si la proportionnalité le permet.

Cette priorité réduit le risque de consommer la capacité d'exécution sur des vérifications secondaires. Elle ne change aucune condition du protocole.

L'unité de contrôle reste celle formulée au départ conformément à 3.B. Ne jamais scinder a posteriori un contrôle partiel en un contrôle abouti et un contrôle infructueux.

## 3. Portabilité des références

### 3.1 Principe

Une analyse destinée à être exportée, archivée ou publiée ne doit pas dépendre uniquement d'un mécanisme de citation propre à l'interface hôte. Les références produites par le wrapper doivent donc exister dans le Markdown restitué, sous une forme qui reste exploitable hors de l'interface.

### 3.2 Dispositif

#### Lien de l'objet analysé

Lorsque l'URL originale de l'objet exact analysé est explicitement disponible dans le document fourni, dans la demande de l'utilisateur ou dans une métadonnée fiable associée à cet objet, la restituer dans l'en-tête de l'analyse sous forme de lien Markdown.

Ne jamais inventer ou déduire une URL à partir du seul titre. L'absence d'URL n'affecte ni l'analyse ni le statut de l'objet et ne justifie pas, à elle seule, une recherche externe destinée uniquement à fabriquer ce lien.

Lorsque plusieurs URL sont disponibles, préférer l'URL canonique si elle est identifiable sans ambiguïté. À défaut, les paramètres manifestement destinés au suivi peuvent être retirés uniquement lorsque leur suppression ne modifie ni l'identité ni l'accessibilité de la ressource. En cas de doute, conserver l'URL originale.

#### Sources des vérifications externes

Pour chaque contrôle externe abouti ou partiel qui produit une source utilisable :

- si la source possède une URL utilisable, placer dans le corps un renvoi Markdown cliquable `[S1](URL)`, `[S2](URL)`, etc. ;
- si aucune URL utilisable n'est disponible, conserver le renvoi portable `[S1]`, `[S2]`, etc. ;
- produire en fin d'analyse une liste `## Sources des vérifications externes` ;
- donner une entrée par élément contrôlé, et non une entrée par URL consultée ;
- pour une source en ligne : auteur ou institution, titre cliquable, date, URL et date de consultation ;
- pour une pièce fournie sans URL utilisable : titre, date et localisation dans le document — page, section ou paragraphe lorsque disponible ;
- pour un contrôle infructueux : nommer l'objet recherché et déclarer l'absence de résultat, sans fabriquer de référence.

Les renvois `[Sn]` constituent un espace de noms volontairement distinct de notes automatiques éventuelles de l'hôte. Le lien Markdown améliore la portabilité ; il ne remplace pas l'entrée descriptive terminale.

### 3.3 Contrôle terminal

Avant remise :

1. reprendre les trois compteurs de 3.B et les rapprocher des contrôles réellement décrits ;
2. vérifier que chaque contrôle abouti ou partiel associé à une source possède un renvoi `[Sn]` résolu ;
3. vérifier que l'URL de l'objet exact figure dans l'en-tête lorsqu'elle était explicitement disponible, et qu'aucune URL n'a été inventée ou déduite du seul titre ;
4. vérifier que tout renvoi `[Sn]` associé à une source disposant d'une URL utilisable est cliquable et que son entrée terminale contient un titre également cliquable ;
5. vérifier que la source citée contient réellement l'information qui lui est attribuée ;
6. rechercher les marqueurs non résolus, crochets vides, placeholders, liens cassés ou renvois sans entrée ;
7. corriger ce qui est observable avant remise ;
8. ne pas déclarer un défaut d'export que l'exécution ne peut pas observer. Si le rendu après export est hors de portée, déclarer seulement cette limite.

## 4. Exécution longue et segmentation

ARGUS V5.0.0 peut produire des sorties longues, surtout avec plusieurs documents et annexes. La segmentation est une technique de livraison, pas une modification du protocole.

- Annoncer la segmentation avant qu'une limite de sortie ne force une coupure.
- Conserver l'ordre du protocole et l'état déjà établi.
- Dans un corpus, exécuter C.1 et C.1 bis avant le premier texte, puis conserver leur résultat pour tous les segments.
- Ne jamais fusionner des étapes, supprimer une section obligatoire ou réduire les textes analysés en fin de corpus pour tenir dans une seule réponse.
- Si le contexte ou l'état nécessaire n'est plus disponible, ne pas présenter la continuation comme une exécution ARGUS complète.

## 5. Contraintes de l'environnement

Une exécution complète suppose une capacité effective d'exécution longue : contexte effectif, capacité de sortie, ingestion documentaire et persistance des instructions suffisants.

Si une capacité manque :

- déclarer la limitation ;
- ne pas transformer une omission imposée par l'environnement en choix méthodologique ;
- proposer, selon le cas, ARGUS Light, un corpus réduit, des analyses indépendantes ou un environnement capable de maintenir l'exécution complète.

L'absence d'accès au Web n'interdit pas toute vérification externe : une source fournie peut satisfaire un contrôle. Inversement, la mémoire du modèle ne remplace jamais une source effectivement consultée.

## 6. Différentiel et consolidation

Lorsque deux analyses ARGUS indépendantes sont fournies :

- conserver leur indépendance et ne pas reconstruire rétroactivement une fausse exécution à l'aveugle ;
- séparer convergence, divergence de position et divergence de couverture ;
- qualifier la nature du désaccord selon les catégories prévues par le protocole ;
- isoler les cas où l'une conclut et l'autre déclare les éléments insuffisants ;
- appliquer la règle d'adjudication du protocole ;
- indiquer ce qui permettrait de trancher et à quel coût.

Ne jamais faire de moyenne entre les conclusions.

## 7. Garde-fous correctifs du wrapper 0.4.2

Ces trois garde-fous rendent mécaniques des distinctions déjà présentes dans ARGUS V5.0.0. Ils ne modifient aucun critère du protocole.

### 7.1 Statut du périmètre : une seule branche

Dans l'en-tête et dans 0.a bis, ne jamais juxtaposer plusieurs statuts de périmètre pour la même décision. Choisir exactement une branche :

- pertinence forte : `périmètre égal au texte complet — [raison]` ; ne jamais ajouter la formule de validation dispensée ;
- périmètre fixé par l'utilisateur : reproduire la formule du protocole indiquant qu'aucune validation supplémentaire n'est requise ;
- périmètre soumis puis validé : indiquer qu'il a été validé par l'utilisateur ;
- validation expressément dispensée sans périmètre fixé par l'utilisateur : utiliser uniquement la formule `périmètre non validé par l'utilisateur, fixé unilatéralement par l'analyste`.

Ces branches sont mutuellement exclusives pour une même décision de périmètre.

### 7.2 Normalisation mécanique des puces Markdown

Avant remise, effectuer une passe de conformité à la Règle 15. Cette passe est une porte binaire de livraison : hors blocs de code clôturés, la sortie finale doit contenir **zéro** ligne de liste correspondant au motif `^\s*[\*\+] `. Toute ligne de liste à puces, après une indentation éventuelle, commence par `- `. Remplacer les marqueurs de liste `* ` et `+ ` par `- ` sans modifier les astérisques d'emphase, les citations, les blocs de code ni les listes numérotées. Ne pas se contenter d'avoir formulé la règle : refaire le contrôle sur la restitution finale après les corrections de l'étape 8.

### 7.3 Limite d'application du Test A de l'Annexe 4

Une simple comparaison entre une distance à parcourir et une portée annoncée ne suffit pas à constituer le raisonnement d'impossibilité du Test A. Ne pas inventer une « unité comptée » ou un ensemble borné pour faire entrer une telle comparaison dans ce test.

Lorsque la structure requise par le protocole n'est pas présente — extrapolation ou cumul sur une fenêtre temporelle, ensemble ou limite de référence pertinent, et condition d'unité non répétable ou renouvellement borné lorsqu'une impossibilité est envisagée —, ne pas conclure à une impossibilité par le Test A. Examiner la revendication quantitative par les autres tests applicables de l'Annexe 4 et/ou par 3.B.

### 7.4 Garde 3.E : absence effective et accessibilité démontrée

Avant toute qualification en « omission stratégique », satisfaire séparément les deux conditions déjà imposées par 3.E.

Premièrement, confirmer l'**absence effective**. Si l'information est mentionnée dans l'objet analysé, même pour être écartée, minimisée, recodée ou privée d'effet, elle n'est pas absente. Ne pas la faire entrer dans 3.E ; examiner son traitement au titre du contradictoire effectif, de la symétrie épistémique, de la cohérence ou de l'adaptation au public selon le cas.

Deuxièmement, établir l'**accessibilité à la date pertinente** en nommant l'information absente et le support concret qui la rendait aisément disponible à la date de publication : article antérieur, déclaration officielle, donnée, document, autre pièce déjà publiée, etc. Les formules « largement disponible », « bien connu », « publiquement documenté » ou équivalentes ne constituent jamais à elles seules la preuve d'accessibilité.

Si ce constat d'accessibilité a nécessité une recherche externe ou la consultation d'une source fournie, cette opération est un contrôle 3.B : la compter avec son statut abouti, partiel ou infructueux et son mode d'accès. Si l'antériorité ou l'accessibilité n'est pas établie, ne pas conclure à une omission stratégique ; utiliser la branche appropriée du protocole (simple faiblesse, absence non imputable ou qualification non déterminable en l'état).

## Régime d'exécution

Le régime d'exécution peut être déclaré :

- wrapper
- contexte
- non déclaré

Lorsque le régime vaut « contexte », aucune révision de wrapper n'est applicable :
la révision du wrapper est indiquée comme « sans objet ».

## Couche de publication

Une présentation publique de type Case Study référence une analyse ARGUS existante.

Elle ne constitue pas un nouveau format analytique.

Elle ne peut pas :
- augmenter le niveau de certitude ;
- supprimer une réserve conditionnant l'interprétation ;
- transformer une indétermination en conclusion.
