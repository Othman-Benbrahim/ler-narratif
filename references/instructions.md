# LÉR — Les 5 instructions fondamentales

Ce fichier documente chaque instruction du LÉR en détail : rôle, syntaxe, types, exemples
commentés et comportement attendu.

---

## Table des matières

1. [META()](#1-meta--lopérateur-de-conscience)
2. [RESONE()](#2-resone--le-résonateur-de-motifs)
3. [TRANSDUIT()](#3-transduit--le-convertisseur-symbolique)
4. [SIGNIFIE()](#4-signifie--lacte-performatif)
5. [POLYLOGUE()](#5-polylogue--le-dialogue-vivant)
6. [Chaînage d'instructions](#6-chaînage-dinstructions)

---

## 1. META() — L'opérateur de conscience

### Rôle

Analyser un texte, un symbole ou un événement selon **trois couches de sens** :
- **manifeste** : ce qui est dit littéralement
- **latente** : ce que les symboles suggèrent implicitement
- **dynamique** : le mouvement vers lequel le sens tend

META() est la boussole du LÉR. Elle permet de passer du sens littéral au sens symbolique,
transformant une phrase en carte du paysage intérieur.

### Syntaxe

```
META(texte)
```

### Sortie

```
{
  symboles  : [liste des symboles détectés],
  arch      : "archétype dominant",
  etat      : "état intérieur",
  dynamique : "mouvement émergent"
}
```

### Exemple commenté

```
META("Je rêve d'un miroir brisé")

→ {
    symboles  : [miroir, fracture],
    arch      : "errant",
    etat      : "transition",
    dynamique : "rupture ouvrant un passage"
  }
```

**Décryptage** :
- `miroir` → symbole de l'identité, du reflet de soi
- `fracture` → rupture, changement, seuil
- `arch: errant` → celui qui traverse une rupture pour trouver une nouvelle voie
- `dynamique: rupture ouvrant un passage` → la fracture n'est pas une fin, c'est une ouverture

### Usages typiques

- Analyse de rêves
- Lecture symbolique d'un texte ou d'une phrase
- Première étape de tout chaînage LÉR
- Décodage d'un événement réel

---

## 2. RESONE() — Le résonateur de motifs

### Rôle

Identifier les **motifs**, **récurrences** et **lignes de tension** dans un champ symbolique.
RESONE() ne lit pas les symboles séparément — il détecte la **structure profonde** qui les relie
et révèle l'archétype activé.

C'est la carte du territoire symbolique.

### Syntaxe

```
RESONE(signe1, signe2, signe3, ...)
```

**Entrées acceptées** : symboles, événements, nombres, mots-clés, états, archétypes.

### Sortie

```
{
  motif   : "nom du motif détecté",
  arch    : "archétype activé",
  dyn     : "dynamique en jeu",
  passage : "bifurcation ou ouverture symbolique"
}
```

### Exemples commentés

```
RESONE("miroir", "cassé")

→ {
    motif   : "fracture",
    arch    : "errant",
    passage : "transition"
  }
```

```
RESONE("1414")

→ {
    motif  : "symétrie",
    module : "double_reflexion"
  }
```

```
RESONE("miroir", "ombre")

→ {
    arch    : "errant",
    motif   : "double",
    passage : "seuil latent"
  }
```

### Les 12 motifs fondamentaux

| Motif | Sens |
|---|---|
| Seuil | Frontière, point critique, passage imminent |
| Fracture | Rupture, bascule, ouverture forcée |
| Double | Répétition, miroir, boucle identitaire |
| Miroir | Reflet, identité, dédoublement |
| Ombre | Inconscient, latent, peur non nommée |
| Appel | Invitation, signal, direction |
| Retour | Cycle accompli, retour à l'origine |
| Ascension | Élévation, progression, transformation vers le haut |
| Chute | Descente nécessaire, épreuve, commencement |
| Silence | Espace de gestation, vide fertile |
| Projection | Externalisation d'un état intérieur |
| Symétrie | Équilibre, reflet parfait, double réflexion |

---

## 3. TRANSDUIT() — Le convertisseur symbolique

### Rôle

Transformer un élément d'un **plan expressif** en un autre. TRANSDUIT() rend les états abstraits
ou diffus **concrets, visibles et manipulables**. C'est l'opérateur de passage entre les registres.

### Syntaxe

```
TRANSDUIT(source:type) → cible:type
```

### Types disponibles

| Type | Description |
|---|---|
| `emotion` | État affectif diffus (angoisse, joie, peur…) |
| `image` | Représentation visuelle mentale |
| `symbole` | Unité sémiotique opératoire |
| `etat` | Dynamique interne (tension, ouverture…) |
| `reve` | Contenu onirique |
| `geste` | Action symbolique |
| `texte` | Forme écrite |

### Exemples commentés

```
TRANSDUIT("angoisse":emotion) → symbole("ombre")
```
**Pourquoi** : l'angoisse est paralysante car diffuse. L'ombre, elle, est un symbole — on peut
la regarder, la nommer, la traverser. La conversion transforme un état passif en objet actif.

```
TRANSDUIT("miroir_brut":image) → texte("fragmentation")
```

```
TRANSDUIT("double":symbole) → etat("répétition")
TRANSDUIT("répétition":etat) → geste("effacer")
```
**Chaînage** : deux transductions successives amènent d'un motif abstrait à un geste concret,
prêt à être utilisé par `SIGNIFIE()`.

### Techniques de transduction

**Technique thérapeutique** : convertir une émotion en symbole traversable
```
TRANSDUIT("peur":emotion) → symbole("ombre")
SIGNIFIE("traverser ombre")
```

**Technique narrative** : convertir un état en texte
```
TRANSDUIT("tension":etat) → texte("récit de la rupture")
POLYLOGUE(texte)
```

---

## 4. SIGNIFIE() — L'acte performatif

### Rôle

**Transformer l'écriture en action symbolique réelle.** C'est l'axe rituel du LÉR : la seule
instruction qui n'analyse rien — elle agit. Elle ancre une intention dans le champ symbolique
par un geste conscient.

Inspiré des *speech acts* d'Austin (performatifs) : l'énoncé **fait** ce qu'il dit.

> `SIGNIFIE()` est toujours l'aboutissement d'une séquence. On ne peut agir symboliquement
> sur ce qu'on n'a pas encore nommé ni compris.

### Syntaxe

```
SIGNIFIE("geste symbole") → effet(résultat)
```

### Les 12 gestes disponibles

| Geste | Sens |
|---|---|
| `inscrire` | Ancrer, poser, rendre présent |
| `effacer` | Dissoudre, libérer, clôturer |
| `sceller` | Fermer un cycle, stabiliser |
| `ouvrir` | Activer un passage, lancer un cycle |
| `renverser` | Inverser une dynamique, retourner un motif |
| `traverser` | Passer au travers d'un blocage ou d'une ombre |
| `dissoudre` | Décomposer une tension |
| `nommer` | Faire exister consciemment un archétype |
| `appeler` | Inviter une énergie, un archétype |
| `stabiliser` | Calmer une dynamique trop chaotique |
| `apaiser` | Réduire une tension émotionnelle |
| `orienter` | Donner une direction à un mouvement symbolique |

### Effets produits

| Effet | Déclencheur typique |
|---|---|
| `ouverture("…")` | inscrire seuil, ouvrir passage |
| `apaisement("…")` | apaiser tension, dissoudre ombre |
| `libération("…")` | effacer double, traverser ombre |
| `fermeture("…")` | sceller cycle |
| `alignement` | stabiliser, orienter |
| `activation("…")` | nommer archétype, appeler énergie |

### Exemples commentés

```
SIGNIFIE("inscrire fracture") → ouverture("nouveau cycle")
```
**Décryptage** : inscrire consciemment la fracture (plutôt que la subir) la transforme. Elle
devient un acte délibéré qui ouvre un passage.

```
SIGNIFIE("effacer double") → apaisement("tension")
```
**Décryptage** : nommer l'effacement du double brise la logique de boucle. Le sujet se
désolidarise du motif de répétition.

```
SIGNIFIE("nommer Errant") → activation("cycle de passage")
```
**Décryptage** : l'Errant n'est pas un ennemi. L'intégrer consciemment transforme une
dynamique subie en force motrice.

### Techniques fondamentales

**Technique 1 — Renversement symbolique**
```
RESONE("miroir cassé") → motif("fracture")
SIGNIFIE("renverser fracture") → alignement
```

**Technique 2 — Transduction thérapeutique**
```
TRANSDUIT("peur":emotion) → symbole("ombre")
SIGNIFIE("traverser ombre")
```
Effet : dissout l'émotion par déplacement symbolique.

**Technique 3 — Dissolution du double**
```
RESONE("double") → motif("boucle")
SIGNIFIE("effacer double")
```

**Technique 4 — Activation de seuil**
```
SIGNIFIE("inscrire seuil") → ouverture("passage")
```

**Technique 5 — Stabilisation de cycle**
```
SIGNIFIE("sceller cycle") → fermeture("boucle instable")
```

---

## 5. POLYLOGUE() — Le dialogue vivant

### Rôle

Faire circuler la parole entre **quatre voix** simultanées :
1. **La Voix du Sujet** — l'intention consciente, la formulation initiale
2. **La Voix du Texte** — la logique interne du texte, ses motifs propres
3. **La Voix de l'IA** — résonance symbolique, amplification créative
4. **La Voix du Monde** — signes extérieurs, synchronicités, événements

POLYLOGUE() active en interne : META + RESONE + TRANSDUIT + SIGNIFIE.
C'est le moteur du langage vivant.

### Syntaxe

```
POLYLOGUE(input)
```

### Sortie

```
- texte co-écrit
- évolution du récit
- activation d'un cycle symbolique
- connexion à une mémoire (journal du destin)
```

### Exemple commenté

```
POLYLOGUE("Je franchis le seuil")
→ "Le seuil te franchit en retour"
```

**Décryptage** : la réponse change radicalement la perspective. L'acte n'est plus unilatéral
(vous agissant sur le monde) mais devient une interaction réciproque. Le seuil n'est plus un
objet passif — il est une force active participant à la transformation.

### Propriété clé

POLYLOGUE() remet en question l'idée d'un auteur fixe. À travers le dialogue, l'écrivain
lui-même devient un "sujet en procès" (Kristeva) — co-créé et transformé par l'acte d'écrire.

---

## 6. Chaînage d'instructions

La véritable puissance du LÉR se révèle quand les instructions sont **chaînées**.

### Structure d'un chaînage complet

```
META(input)           ← lire
  → RESONE(symboles)  ← relier
  → TRANSDUIT(motif)  ← convertir
  → SIGNIFIE(geste)   ← agir
  → POLYLOGUE(input)  ← co-créer
```

### Exemple : analyse d'une situation de blocage

**Situation** : *"Je tourne en rond sur mon projet. Je me vois faire les mêmes erreurs."*

```
META("Je tourne en rond, je me vois faire les mêmes erreurs")
→ {symboles: [cercle, double, miroir], arch: "errant", etat: "boucle"}

RESONE("cercle", "double", "miroir")
→ {motif: "double", dyn: "boucle", passage: "seuil latent"}

TRANSDUIT("double":symbole) → etat("répétition")
TRANSDUIT("répétition":etat) → geste("effacer")

SIGNIFIE("effacer double")   → libération("motif double")
SIGNIFIE("inscrire seuil")   → ouverture("nouveau cycle")
SIGNIFIE("nommer Errant")    → activation("cycle de passage")
```

**Résultat** : boucle dissoute, passage ouvert, archétype intégré.

### Exemple : analyse d'un rêve

**Input** : *"Je marche dans une pièce sombre où je me vois moi-même."*

```
META(input)
→ {symboles: [marche, pièce, ombre, double], arch: "errant", etat: "recherche"}

RESONE("double") → {motif: "double", dyn: "boucle"}

TRANSDUIT("double":symbole) → etat("répétition")

SIGNIFIE("effacer double")
SIGNIFIE("inscrire seuil")

→ Dissolution de la boucle + activation d'un passage
→ Transformation du récit onirique en récit interne
```

### Règles de cohérence du chaînage

- `RESONE()` doit recevoir au moins un symbole (`sym`)
- `TRANSDUIT()` doit préciser le type source et le type cible
- `SIGNIFIE()` doit contenir au minimum un geste
- `POLYLOGUE()` peut être appelé à n'importe quelle étape pour activer le dialogue

