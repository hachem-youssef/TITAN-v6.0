# TITAN v6.0

**TITAN — cadre d'assurance adversariale bornée**

Auteur : **Hachem Youssef**  
Date : **27/09/2026**  
Statut : **dernière version documentaire — suivie d'exécution empirique**

> TITAN v6.0 clôt la phase documentaire. La phase suivante est empirique : appliquer le noyau formel à des cas publics, mesurer FCI-C et recueillir des catches confirmés par un reviewer externe.

## Positionnement

TITAN n'est ni un moteur de vérité, ni un calculateur de probabilité, ni un score de sécurité, ni un substitut à une décision.

Il organise l'examen d'une affirmation critique par :
- explicitation d'un modèle borné ;
- génération adversariale d'hypothèses de falsification ;
- séparation stricte entre attaque, test, observation et évidence ;
- représentation des chemins résiduels de falsification (RFS) ;
- enregistrement explicite des lacunes du modèle (MSG) ;
- traitement séparé des inconnues et contradictions ;
- arrêt à une profondeur méta déclarée ;
- versionnement et invalidation des évidences ;
- séparation stricte entre verdict épistémique et décision de gouvernance.

## Règle centrale

```text
Conclusion ≤ Coverage
```

Et :

```text
World ≠ Model ≠ Tested Domain ≠ Observation ≠ Evidence ≠ Conclusion
```

## Critère de falsifiabilité

Le document v6.0 contient un engagement explicite :

> Si, sur 10 cas réellement traités avec reviewer externe, TITAN produit 0 catch confirmé au sens de §VII.1, la thèse centrale est considérée comme fausse et le cadre doit être abandonné en tant que contribution scientifique.

Aucune version documentaire ultérieure ne doit être produite avant l'exécution de la phase empirique.

## Structure

```text
TITAN-v6.0/
├── README.md
├── CITATION.cff
├── LICENSE
├── docs/
│   └── TITAN-v6.0.md
├── diagrams/
│   ├── architecture.mmd
│   ├── decidability.mmd
│   └── lifecycle.mmd
├── experimental/
│   ├── protocol.md
│   ├── qualification-grid.md
│   └── phase-1-report.md
└── cases/
    ├── C-ABS-32.md
    ├── C-LOCK-VNE4.md
    ├── C-LOCK-PROD.md
    ├── C-SORT-2.md
    └── C-INDET-DISAGREE.md
```

## État du projet

| Élément | État |
|---|---|
| Doctrine | documentée |
| Noyau formel | documenté |
| Spécification d'implémentation | documentée |
| Versionnement | documenté |
| Robustesse | documentée |
| FCI-C | défini |
| Critère de mort | défini |
| Protocole Phase 1 | défini |
| Grille reviewer | définie |
| Cas candidats | proposés |
| Résultats empiriques Phase 1 | **à produire** |
| Reviewer externe | **à organiser** |

## Important

Les cas présents dans `cases/` sont des **fiches de travail** reprises du document v6.0. Elles ne constituent pas, à elles seules, une validation empirique indépendante.

Le dépôt doit rester fidèle à cette distinction.

## Licence

La documentation de ce dépôt est distribuée sous **CC BY 4.0**. Voir `LICENSE`.
