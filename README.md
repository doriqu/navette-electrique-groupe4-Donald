# Navette électrique — Groupe IV : Simulation et PCB

Simulation du circuit basse tension (12 V) de la navette électrique 8 places, sous KiCad/ngspice.

## Contenu du dépôt

- `*.kicad_pro`, `*.kicad_sch` — projet KiCad (schéma + directives de simulation)
- `Donald_OKE_Groupe4.pdf` — rapport d'analyse des signaux (dimensionnement, résultats, interprétation)

## Blocs simulés

1. Convertisseur DC-DC (buck 72V → 12V)
2. Batterie tampon 12 V
3. Charges commutables (nominal / pointe)
4. ECU (test d'inrush à la mise sous tension)

## Résultats clés

| Simulation | Résultat |
|---|---|
| Ondulation en régime établi | ≈ 24 mV crête-à-crête |
| Variation de charge | ΔV ≈ 230 mV entre paliers nominal/pointe |
| Courant d'appel (inrush) | ≈ 68–70 A |

Voir le rapport PDF pour le détail des calculs et l'interprétation complète.

## Ouverture du projet

KiCad 7 ou 8, avec ngspice intégré pour lancer les simulations (`Inspect → Simulator`).
