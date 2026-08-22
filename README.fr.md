# Protocole ARGUS

**ARGUS** — *Analyse Rigoureuse Guidée par un protocole Universel et Systématique* — est un protocole libre d’analyse critique des textes argumentatifs avec l’aide d’une intelligence artificielle.

- **Version actuelle du protocole :** ARGUS V5.0.0
- **Version actuelle du wrapper :** ARGUS Skill 0.4.3
- **Site :** https://www.argus-protocol.org
- **Dépôt GitHub :** https://github.com/argus-analysis/argus
- **Auteur :** François Vadrot

Le protocole et le Skill ont des **numérotations distinctes**. Le Skill est une couche d’exécution destinée à faciliter l’appel du protocole sur les plateformes compatibles ; il ne remplace ni ne redéfinit le protocole. **ARGUS V5.0.0 demeure la référence normative.**

## Protocole V5.0.0

Le protocole est disponible dans six langues :

| Langue | Source |
|---|---|
| Français | [argus-protocol-fr.md](protocol/V5.0.0/argus-protocol-fr.md) |
| English | [argus-protocol-en.md](protocol/V5.0.0/argus-protocol-en.md) |
| Español | [argus-protocol-es.md](protocol/V5.0.0/argus-protocol-es.md) |
| Deutsch | [argus-protocol-de.md](protocol/V5.0.0/argus-protocol-de.md) |
| Italiano | [argus-protocol-it.md](protocol/V5.0.0/argus-protocol-it.md) |
| Português | [argus-protocol-pt.md](protocol/V5.0.0/argus-protocol-pt.md) |

La source française est la source normative embarquée dans le Skill actuel. Les traductions publiées reproduisent le même protocole V5.0.0 pour usage dans les langues correspondantes.

## ARGUS Skill 0.4.3

Le wrapper stable destiné à ARGUS V5.0.0 se trouve dans [`skill/V0.4.3`](skill/V0.4.3/).

Il contient le ZIP installable, le code source décompressé du Skill, le protocole normatif V5.0.0 en français, les règles techniques d’exécution et le gabarit de sortie.

Commande minimale après installation :

> Analyse ce texte avec ARGUS.

Pour une exécution courte :

> Analyse ce texte avec ARGUS Light.

Pour plusieurs textes liés :

> Analyse ces textes comme un corpus avec ARGUS.

## Intégrité

Les fichiers de publication sont recensés dans [`CHECKSUMS.sha256`](CHECKSUMS.sha256).

- Source française normative V5.0.0 : `4da638b15145c5f13183cf5d9e6b9dfb4f503b425ba3f576eded8c9aed53ca85`
- ZIP du Skill 0.4.3 : `a5d7b0bffeaff1717e6b58fafff1bf91cd68fdcc68eafc02aa9196af0c752f60`

## Licence

Le protocole ARGUS est publié sous **Creative Commons Attribution - Partage dans les Mêmes Conditions 4.0 International (CC BY-SA 4.0)**. Voir [LICENSE.md](LICENSE.md).
