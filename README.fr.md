# Protocole ARGUS

**ARGUS** — *Analyse Rigoureuse Guidée par un protocole Universel et Systématique* — est un protocole libre d’analyse critique des textes argumentatifs avec l’aide d’une intelligence artificielle.

- **Version actuelle du protocole :** ARGUS V5.1.0
- **Version actuelle du wrapper :** ARGUS Skill 1.0.0
- **Site :** https://www.argus-protocol.org
- **Dépôt GitHub :** https://github.com/argus-analysis/argus
- **Auteur :** François Vadrot

Le protocole et le Skill ont des **numérotations distinctes**. Le Skill est une couche d’exécution destinée à faciliter l’appel du protocole sur les plateformes compatibles ; il ne remplace ni ne redéfinit le protocole. **ARGUS V5.1.0 demeure la référence normative.**

## Protocole V5.1.0

Le protocole est disponible dans six langues :

| Langue | Source |
|---|---|
| Français | [argus-protocol-fr.md](protocol/V5.1.0/argus-protocol-fr.md) |
| English | [argus-protocol-en.md](protocol/V5.1.0/argus-protocol-en.md) |
| Español | [argus-protocol-es.md](protocol/V5.1.0/argus-protocol-es.md) |
| Deutsch | [argus-protocol-de.md](protocol/V5.1.0/argus-protocol-de.md) |
| Italiano | [argus-protocol-it.md](protocol/V5.1.0/argus-protocol-it.md) |
| Português | [argus-protocol-pt.md](protocol/V5.1.0/argus-protocol-pt.md) |

La source française est normative. Les cinq autres fichiers sont des traductions auditées du même protocole V5.1.0.

V5.1.0 ajoute le **contrôle de constance modale**, test directionnel de la rétractation modale : une même proposition portante est posée fortement là où elle accomplit le travail argumentatif et affaiblie là où l’engagement fort aurait un coût. Les catégories existantes, les seuils, la norme de preuve et la procédure d’ensemble de V5.0.0 restent inchangés.

## ARGUS Skill 1.0.0

Le wrapper stable destiné à ARGUS V5.1.0 se trouve dans [`skill/V1.0.0`](skill/V1.0.0/).

Il contient le ZIP installable [`argus-wrapper-v1.0.0.zip`](skill/V1.0.0/argus-wrapper-v1.0.0.zip), le code source décompressé du Skill, le protocole normatif V5.1.0 en français, les règles techniques d’exécution, le gabarit de sortie et un historique propre des versions du wrapper.

La version 1.0.0 fixe pour la première fois le périmètre public stabilisé du **wrapper générique d’exécution ARGUS**. Il reste indépendant de tout site et de tout workflow éditorial ou de publication. Les conventions propres aux Case Studies et aux pipelines éditoriaux relèvent d’outils séparés.

Le durcissement 1.0.0 impose aussi la propagation des corrections de l’étape 8 jusqu’au jugement final de 7.c, explicite le seuil 2 → 3 en termes de convergence effective plutôt que d’accumulation de défauts, et préserve entre passes les constats explicitement figés sauf apparition d’un élément matériel nouveau identifié.

La branche expérimentale 0.7.0 n’a jamais été publiée comme successeur stable de 0.6.0 ; son travail propre à la publication a été séparé avant 1.0.0.

Commande minimale après installation :

> Analyse ce texte avec ARGUS.

Pour une exécution courte :

> Analyse ce texte avec ARGUS Light.

Pour plusieurs textes liés :

> Analyse ces textes comme un corpus avec ARGUS.

Voir [Utilisation du Skill ARGUS](docs/skill.md) pour les détails et limites connues.

## Intégrité

Les fichiers de publication sont recensés dans [`CHECKSUMS.sha256`](CHECKSUMS.sha256).

- Source française normative V5.1.0 : `4d4929996358cd1359d0349c3cee93c8e54d39a4ca5f3143861b2bff8dc7feee`
- ZIP du Skill 1.0.0 : `8e48404edfc95371191825ca77a06c5ce7b62dba71aa85aff415dd2e6a321cef`

## Licence

Le protocole ARGUS est publié sous **Creative Commons Attribution - Partage dans les Mêmes Conditions 4.0 International (CC BY-SA 4.0)**. Voir [LICENSE.md](LICENSE.md).
