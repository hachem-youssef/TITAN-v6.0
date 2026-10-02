# TITAN — Grille de qualification reviewer

Pour chaque attaque `a ∈ A(TITAN) \ A(EA)` :

| Critère | Question | Réponse |
|---|---|---|
| C1 — Falsifiabilité | L'attaque est-elle falsifiable ? | O/N |
| C2 — Domaine | Le domaine est-il défini ? | O/N |
| C3 — Lien au claim | L'attaque peut-elle invalider C ? | O/N |
| C4 — Non-redondance | L'attaque est-elle absente d'EA ? | O/N |
| C5 — Actionnabilité | Une mitigation est-elle concevable ? | O/N |

## Règle

Une attaque est pertinente si les cinq réponses sont `O`.

### Cas limite

Si C4 = `N`, l'attaque est redondante et n'entre pas dans le calcul FCI-C.

### Cas à discuter

Si C3 est ambigu, marquer `À DISCUTER`. L'attaque est tracée mais n'entre ni dans FCI-C ni dans les catches tant que le désaccord n'est pas résolu.

## Fiche

```text
Case ID:
Attack ID:
Reviewer:
Date:

C1:
C2:
C3:
C4:
C5:

Statut: PERTINENTE / NON PERTINENTE / À DISCUTER
Justification:
```
