# Templates — Fichiers Externes (gérés par l'utilisateur)

Ces fichiers sont externes à l'agent. Tu les gères toi-même.
Tu les injectes en début de session selon le besoin.
L'agent les lit s'ils sont fournis, ne les modifie jamais lui-même.

---

## FICHIER 1 : rdm-custom.md
### Répertoire Dynamique des Motifs — Version Personnalisée

Copier ce template sous le nom `rdm-custom.md`.
Enrichir avec les nouveaux motifs détectés dans les sessions (apparaissent dans les blocs MER).

```markdown
# RDM Custom — [Ton Nom / Projet]
# Version : X.X — Dernière mise à jour : [DATE]

## Archétypes Personnels Actifs

| Archétype | Polarité | Récit associé | Activé le | Notes |
|---|---|---|---|---|
| [Nom] | [+/–] | [Phrase type] | [Date] | [Contexte d'activation] |

## Archétypes Collectifs Actifs

| Archétype | Domaine | Récit collectif | Activé le | Notes |
|---|---|---|---|---|
| [Nom] | [Domaine] | [Récit] | [Date] | [Contexte] |

## Motifs Nouveaux (issus des sessions MER)

| Motif | Source | Date | À intégrer dans quelle catégorie |
|---|---|---|---|
| [Motif observé] | Session MER du [DATE] | [Date] | [Perso / Collectif] |

## Connexions Récurrentes Observées

[Notes libres sur les patterns qui se répètent entre sessions]
```

---

## FICHIER 2 : mer-log.md
### Log des Sessions — Base d'Apprentissage Externe

```markdown
# MER Log — Module d'Évaluation Rétrospective
# Format : une entrée par session

---

=== ENTRÉE MER — [DATE] ===
Mode : [A / B / C]
Contexte initial : [Résumé en 1-2 phrases de l'input utilisateur]
Archétypes actifs : [Liste depuis RDM]
Récit dominant identifié : [Phrase extraite]
Score IPC dominant : [Signal + score]

Phrase réécrite :
[Phrase ancienne] → [Phrase réécrite]

Phrase FdD générée :
[Événement] → [Archétype] → [Influence] → [Modulation]

Protocole d'ancrage proposé : [Type + description]

Scénarios PNB+ (si Mode B) :
- Optimiste [X%] : [...]
- Probable [X%] : [...]
- Critique [X%] : [...]

Points à surveiller pour la prochaine session :
- [Indicateur 1]
- [Indicateur 2]

Motifs nouveaux détectés (à intégrer dans rdm-custom.md) :
- [Motif observé] : [Description]

Évaluation rétrospective (à remplir lors de la session suivante) :
- La réécriture a-t-elle vibré juste ? [Oui / Partiellement / Non]
- Des changements observés depuis ? [Notes libres]
- Scénario réalisé (Mode B) : [Optimiste / Probable / Critique / Autre]
=================

```

---

## FICHIER 3 : contexte-session.md
### Contexte Optionnel — Injection en Début de Session

```markdown
# Contexte de Session — [DATE]

## Contexte actuel
[Ce qui se passe dans ma vie / mon projet / la situation analysée]

## Dernière session — Points ouverts
[Ce qui avait été identifié à surveiller]

## RDM actif
[Archétypes que je veux prioriser pour cette session]

## Intention de session
[Ce que j'espère explorer ou transformer aujourd'hui]

## Fichiers à fournir à l'agent
- [ ] rdm-custom.md
- [ ] mer-log.md (3 dernières entrées)
- [ ] ce fichier contexte-session.md
```

---

## Convention d'utilisation recommandée

**Début de session :**
1. Remplir `contexte-session.md`
2. Ouvrir une nouvelle conversation avec l'agent
3. Joindre les fichiers pertinents
4. L'agent lit et intègre avant de répondre

**Fin de session :**
1. Copier le bloc MER généré par l'agent
2. Le coller dans `mer-log.md`
3. Vérifier si des motifs nouveaux sont à intégrer dans `rdm-custom.md`
4. Compléter l'évaluation rétrospective de la session précédente

**Fréquence de mise à jour RDM :**
- Après 3-5 sessions, relire le `rdm-custom.md` et fusionner les motifs récurrents
- Supprimer les archétypes qui ne résonnent plus
- Amplifier ceux qui sont devenus centraux
```
