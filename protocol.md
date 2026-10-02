# TITAN — Protocole expérimental Phase 1

## Objectif

Tester empiriquement si l'intégration TITAN produit des informations nouvelles et confirmées par un reviewer externe par rapport à une méthode de référence.

## Comparaison

Pour chaque cas :

1. TITAN complet
2. TITAN dégradé
3. Méthode de référence (EA ou GSN selon le cas)
4. Revue non structurée

## Mesures

- verdict ;
- statut `INDETERMINATE` ;
- `FCI-C` ;
- nombre de catches ;
- nature des catches ;
- confirmation ou rejet par reviewer externe.

## Corpus proposé

### Famille A — cas bien bornés

- TLS 1.3 hybride (X25519MLKEM768)
- Signal Protocol (Double Ratchet)
- Tri par insertion sur C99
- Modbus TCP
- CBOR

### Famille B — cas moins bornés

- chaînes logistiques
- MFA
- cloud
- vote

## Procédure minimale

1. Le reviewer externe sélectionne les cas finaux parmi une liste élargie.
2. Le modèle et le domaine sont gelés avant analyse.
3. Les attaques produites sont enregistrées sans suppression a posteriori.
4. Les résultats TITAN et de la référence sont conservés séparément.
5. Les attaques supplémentaires sont qualifiées avec la grille `qualification-grid.md`.
6. Les désaccords sont enregistrés.
7. Le FCI-C est calculé après qualification.
8. Les catches sont confirmés indépendamment.
9. Le rapport est publié quel que soit le résultat.

## Règle de falsification

Sur 10 cas avec reviewer externe :

`0 catch confirmé ⇒ abandon de la thèse centrale de TITAN en tant que contribution scientifique.`

## Interdiction

Aucune nouvelle version documentaire de TITAN avant publication des résultats de la phase empirique.
