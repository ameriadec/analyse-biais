# analyse-biais

Une skill qui analyse une situation et identifie les biais cognitifs qui déforment le jugement.

Elle ne valide pas ce que vous pensez déjà. Elle cherche ce que vous ne voyez pas.

## Ce qu'elle fait

Vous décrivez une situation — une décision à prendre, un projet qui traîne, un désaccord, un doute. Elle produit une analyse structurée :

- une reformulation en faits, sans jugement
- deux à quatre biais identifiés, chacun ancré dans une phrase précise de votre description
- pour chaque biais : ce qu'il coûte, la question qui le teste, le geste qui le corrige
- ce qui manque pour trancher
- une question unique pour débloquer

## Ce qu'elle ne fait pas

Elle ne fait pas d'horoscope. Un diagnostic qui pourrait s'appliquer à n'importe qui est supprimé.

Elle n'empile pas. Trouver huit biais donne l'illusion de la profondeur et produit du bruit.

Elle n'invente pas. Si aucun biais n'est identifiable, elle le dit.

Elle ne psychologise pas. L'analyse porte sur le raisonnement décrit, pas sur la personnalité.

## Installation

Cloner le dépôt dans le répertoire des skills de votre agent.

**Claude Code / Claude.ai**

```bash
git clone https://github.com/ameriadec/analyse-biais.git ~/.claude/skills/analyse-biais
```

**Hermes Agent**

```bash
git clone https://github.com/ameriadec/analyse-biais.git ~/.hermes/skills/productivity/analyse-biais
```

La skill se déclenche seule sur les formulations du type « j'hésite entre », « je ne sais pas quoi faire », « est-ce que j'ai raison de », « aide-moi à y voir clair ».

## Structure

```
analyse-biais/
├── SKILL.md              Les 8 biais principaux, le format de sortie, un exemple complet
└── references/
    └── catalogue.md      33 biais complémentaires, classés par usage
```

Le SKILL.md se charge à chaque déclenchement. Le catalogue n'est lu que si les huit biais principaux ne suffisent pas.

## Les huit biais principaux

Coût irrécupérable · Escalade d'engagement · Confirmation · Ancrage · Optimisme · Surconfiance · Statu quo · Attribution fondamentale

Le catalogue couvre cinq domaines supplémentaires : lecture d'une situation, estimation et prévision, perception d'autrui, regard rétrospectif, décision en groupe.

## Exemple

> « J'ai un consultant que je paie depuis six mois. Il ne livre pas grand-chose mais il connaît bien le dossier maintenant. Si je le lâche, je perds tout ce qu'il a appris. »

La skill identifie le coût irrécupérable et le biais de statu quo, et retourne la question qui tranche : *si ce consultant se présentait aujourd'hui, sans historique, avec son niveau de production actuel, tu l'embaucherais ?*

L'exemple complet est dans `SKILL.md`.

## Langue

Français.

## Contribuer

Les issues sont ouvertes. Ce qui intéresse le plus : des cas où la skill produit une analyse creuse ou passe à côté d'un biais évident.

## Licence

MIT.
