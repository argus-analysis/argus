# Protocole ARGUS

**ARGUS** â€” *Analyse Rigoureuse GuidÃ©e par un protocole Universel et SystÃ©matique* â€” est un protocole libre dâ€™analyse critique des textes argumentatifs avec lâ€™aide dâ€™une intelligence artificielle.

- **Version actuelle du protocole :** ARGUS V5.1.0
- **Version actuelle du wrapper :** ARGUS Skill 0.6.0
- **Site :** https://www.argus-protocol.org
- **DÃ©pÃ´t GitHub :** https://github.com/argus-analysis/argus
- **Auteur :** FranÃ§ois Vadrot

Le protocole et le Skill ont des **numÃ©rotations distinctes**. Le Skill est une couche dâ€™exÃ©cution destinÃ©e Ã  faciliter lâ€™appel du protocole sur les plateformes compatibles ; il ne remplace ni ne redÃ©finit le protocole. **ARGUS V5.1.0 demeure la rÃ©fÃ©rence normative.**

## Protocole V5.1.0

Le protocole est disponible dans six langues :

| Langue | Source |
|---|---|
| FranÃ§ais | [argus-protocol-fr.md](protocol/V5.1.0/argus-protocol-fr.md) |
| English | [argus-protocol-en.md](protocol/V5.1.0/argus-protocol-en.md) |
| EspaÃ±ol | [argus-protocol-es.md](protocol/V5.1.0/argus-protocol-es.md) |
| Deutsch | [argus-protocol-de.md](protocol/V5.1.0/argus-protocol-de.md) |
| Italiano | [argus-protocol-it.md](protocol/V5.1.0/argus-protocol-it.md) |
| PortuguÃªs | [argus-protocol-pt.md](protocol/V5.1.0/argus-protocol-pt.md) |

La source franÃ§aise est normative. Les cinq autres fichiers sont des traductions auditÃ©es du mÃªme protocole V5.1.0.

V5.1.0 ajoute le **contrÃ´le de constance modale**, test directionnel de la rÃ©tractation modale : une mÃªme proposition portante est posÃ©e fortement lÃ  oÃ¹ elle accomplit le travail argumentatif et affaiblie lÃ  oÃ¹ lâ€™engagement fort aurait un coÃ»t. Les catÃ©gories existantes, les seuils, la norme de preuve et la procÃ©dure dâ€™ensemble de V5.0.0 restent inchangÃ©s.

## ARGUS Skill 0.6.0

Le wrapper stable destinÃ© Ã  ARGUS V5.1.0 se trouve dans [`skill/V0.6.0`](skill/V0.6.0/).

Il contient le ZIP installable [`argus-wrapper-v0.6.0.zip`](skill/V0.6.0/argus-wrapper-v0.6.0.zip), le code source dÃ©compressÃ© du Skill, le protocole normatif V5.1.0 en franÃ§ais, les rÃ¨gles techniques dâ€™exÃ©cution, le gabarit de sortie et un historique propre des versions du wrapper.

La rÃ©vision 0.6.0 met Ã  jour la cible vers V5.1.0 et formalise la provenance de lâ€™analyste par trois champs â€” modÃ¨le, version/build et intensitÃ© de raisonnement au label du fournisseur â€” tout en conservant les mÃ©tadonnÃ©es hÃ´te et rÃ©gime dâ€™exÃ©cution.

Commande minimale aprÃ¨s installation :

> Analyse ce texte avec ARGUS.

Pour une exÃ©cution courte :

> Analyse ce texte avec ARGUS Light.

Pour plusieurs textes liÃ©s :

> Analyse ces textes comme un corpus avec ARGUS.

## IntÃ©gritÃ©

Les fichiers de publication sont recensÃ©s dans [`CHECKSUMS.sha256`](CHECKSUMS.sha256).

- Source franÃ§aise normative V5.1.0 : `4d4929996358cd1359d0349c3cee93c8e54d39a4ca5f3143861b2bff8dc7feee`
- ZIP du Skill 0.6.0 : `949a375fc3a52b1c402e4026e843cb58a2a5d935253cf4fb3da6324f170ce817`

## Licence

Le protocole ARGUS est publiÃ© sous **Creative Commons Attribution - Partage dans les MÃªmes Conditions 4.0 International (CC BY-SA 4.0)**. Voir [LICENSE.md](LICENSE.md).
