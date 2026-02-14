# GitHub Projects & GitLab Boards - 10 minutes

## Introduction

Pour les équipes de développement qui utilisent déjà **GitHub** ou **GitLab** pour le versionnage du code, ces plateformes proposent désormais des outils intégrés de gestion de projet agile.

**Avantage majeur :** Tout au même endroit (code + gestion de projet)

---

## GitHub Projects

### Présentation

**GitHub Projects** est l'outil de gestion de projet natif de GitHub, entièrement refondu en 2022.

**Fonctionnalités :**
- Tableaux Kanban et vues multiples
- Lien automatique avec Issues et Pull Requests
- Automation intégrée
- Gratuit pour les projets publics et privés

**Cibles :** Équipes de développement de toutes tailles

---

### Concepts de base

#### 1. Issues
**Équivalent des User Stories / Tasks / Bugs dans Jira**

**Création d'une issue :**
```markdown
Title: Ajouter authentification Google

## Description
En tant qu'utilisateur,
Je veux me connecter avec mon compte Google
Afin de ne pas créer un nouveau mot de passe

## Critères d'acceptation
- [ ] Bouton "Sign in with Google"
- [ ] OAuth 2.0 configuré
- [ ] Profil utilisateur créé automatiquement

## Labels
`feature`, `authentication`, `high-priority`

## Assignees
@alice, @bob
```

**Labels prédéfinis :**
- `bug`, `enhancement`, `documentation`
- Personnalisables (couleurs, noms)

**Milestones :**
- Regrouper des issues par version/release
- Ex : "v1.0", "Sprint 1"

#### 2. Pull Requests (PR)
- Intégration native avec les issues
- `Closes #123` dans la description → ferme automatiquement l'issue à la fusion

#### 3. Projects (Tableaux)

**Deux vues principales :**

**a) Table View (vue tableur)**
```
| Title               | Status      | Assignee | Priority |
|---------------------|-------------|----------|----------|
| Add Google login    | In Progress | Alice    | High     |
| Fix password reset  | To Do       | Bob      | Medium   |
```

**b) Board View (vue Kanban)**
```
┌───────────┬─────────────┬──────────┬──────┐
│ Backlog   │ In Progress │ Review   │ Done │
├───────────┼─────────────┼──────────┼──────┤
│ Issue #45 │ Issue #42   │ PR #40   │ #38  │
│ Issue #46 │ PR #43      │          │ #39  │
│ Issue #47 │             │          │      │
└───────────┴─────────────┴──────────┴──────┘
```

**Autres vues :**
- **Roadmap** : Timeline des milestones
- **Custom views** : Filtres personnalisés

---

### Fonctionnalités clés

#### Champs personnalisés
- Text, Number, Date, Single/Multiple select
- Ex : Story Points, Priority, Sprint

#### Automation
**Workflows automatiques :**
- "Quand une PR est mergée → passer l'issue en Done"
- "Quand une issue est créée avec label `bug` → passer en Triage"

**Configuration :** Graphique (no-code)

#### Itérations / Sprints
- Créer des cycles (ex : Sprint 1, Sprint 2)
- Assigner des issues aux itérations
- Tracking de la vélocité

#### Insights (Analytics)
- Burnup charts
- Vélocité par itération
- Nombre d'issues par statut

---

### Intégration code + projet

**Lier une issue à un commit :**
```bash
git commit -m "Add Google OAuth #42"
# → Apparaît dans l'historique de l'issue #42
```

**Lier une PR à une issue :**
```markdown
Closes #42
Fixes #45
Resolves #50
```
→ Issues fermées automatiquement à la fusion

**Bénéfice :** Traçabilité totale code ↔ projet

---

### GitHub Projects : Use cases

**✅ Idéal pour :**
- Équipes déjà sur GitHub
- Projets open source
- Startups / petites équipes
- Besoin de simplicité

**⚠️ Limites :**
- Moins de fonctionnalités que Jira
- Reporting moins avancé
- Pas de time tracking natif

---

### Exemple de workflow

**1. Créer un projet**
- Repository → Projects → New Project
- Choisir un template (Kanban, Scrum, Roadmap)

**2. Ajouter des issues**
- Créer depuis le board
- Ou lier des issues existantes du repo

**3. Configurer les colonnes**
- Ex : Backlog / Ready / In Dev / Review / Done

**4. Ajouter des champs**
- Story Points (number)
- Priority (select)
- Sprint (iteration)

**5. Activer l'automation**
- Auto-move to "In Progress" when assigné
- Auto-move to "Done" when closed

**6. Utiliser le board**
- Drag & drop des cartes
- Filtrer par sprint, assignee, label

---

## GitLab Boards

### Présentation

**GitLab** est une plateforme DevOps complète (Git + CI/CD + Project Management).

**GitLab Issue Boards** = tableaux Kanban intégrés

**Disponible dans :**
- GitLab.com (SaaS gratuit ou payant)
- GitLab Self-Managed (on-premise)

---

### Concepts de base

#### Issues
- Similaires à GitHub
- Labels, Milestones, Assignees, Weight (points)

**Spécificités GitLab :**
- **Weight** : Équivalent des Story Points (1-10)
- **Epic** : Groupement d'issues (GitLab Premium/Ultimate)
- **Health Status** : On Track / Needs Attention / At Risk

**Exemple d'issue :**
```markdown
Title: Implémenter le reset de mot de passe

Description:
En tant qu'utilisateur ayant oublié mon mot de passe...

Labels: feature, authentication
Milestone: v1.2
Assignee: @carol
Weight: 5
```

#### Labels et Scoped Labels

**Labels classiques :** `bug`, `feature`

**Scoped Labels (GitLab exclusif) :**
- Format : `status::todo`, `status::doing`, `status::done`
- **Mutuellement exclusifs** : Une issue ne peut avoir qu'un seul label `status::`
- Utile pour les workflows

---

### Issue Boards (Tableaux)

**Board = Vue Kanban des issues**

**Colonnes basées sur labels :**
```
Colonne "To Do"    → Issues avec label `status::todo`
Colonne "Doing"    → Issues avec label `status::doing`
Colonne "Review"   → Issues avec label `status::review`
Colonne "Done"     → Issues fermées
```

**Drag & drop :**
- Déplacer une carte change automatiquement son label

**Multiple boards :**
- Board par équipe
- Board par feature
- Board backend vs frontend

---

### Fonctionnalités avancées

#### 1. Milestones (Sprints)
- Créer des milestones avec dates de début/fin
- Assigner des issues aux milestones
- Burndown chart par milestone (GitLab Premium)

#### 2. Epics (GitLab Premium/Ultimate)
- Regrouper plusieurs issues
- Roadmap visuelle
- Tracking de progression

#### 3. Swimlanes
- Grouper les issues sur le board par Epic ou Assignee

#### 4. WIP Limits (Work In Progress)
- Limiter le nombre de cartes par colonne (Premium/Ultimate)

#### 5. Intégration CI/CD
- Voir le statut des pipelines directement dans les issues
- Lier les déploiements aux issues

---

### GitLab vs GitHub Projects

| Critère | GitHub Projects | GitLab Boards |
|---------|-----------------|---------------|
| **Gratuit** | Oui (complet) | Oui (basique), Premium pour fonctions avancées |
| **Vues** | Table, Board, Roadmap, Custom | Board, List |
| **Epics** | Via Milestones | Natif (Premium) |
| **CI/CD** | GitHub Actions (séparé) | Intégré nativement |
| **Scoped Labels** | Non | Oui |
| **Burndown** | Limité | Oui (Premium) |
| **Self-hosted** | Non | Oui |

**GitLab = DevOps tout-en-un**
**GitHub = Écosystème plus large (mais plus fragmenté)**

---

### Workflow GitLab typique

**1. Créer un board**
- Project → Issues → Boards → New Board
- Configurer les colonnes (basées sur labels)

**2. Créer des labels scoped**
```
status::backlog
status::ready
status::doing
status::review
status::done
```

**3. Créer des issues**
- Directement depuis le board ou depuis Issues

**4. Créer un milestone (Sprint)**
- Project → Issues → Milestones → New Milestone
- Dates : 01/03/2024 - 14/03/2024

**5. Assigner des issues au milestone**

**6. Travailler sur le board**
- Drag & drop pour changer de colonne
- Labels mis à jour automatiquement

**7. Lier code et issues**
```bash
git commit -m "Fix login bug

Closes #42"
```

**8. Merge Request (MR) = Pull Request**
- Créer une MR liée à l'issue
- Pipeline CI/CD s'exécute
- Code review
- Merge → ferme l'issue

---

## Comparaison GitHub vs GitLab vs Jira

| Critère | Jira | GitHub Projects | GitLab Boards |
|---------|------|-----------------|---------------|
| **Courbe d'apprentissage** | Élevée | Faible | Moyenne |
| **Personnalisation** | Maximale | Moyenne | Moyenne |
| **Reporting** | Avancé | Basique | Moyen (Premium: Avancé) |
| **Intégration code** | Via plugins | Native | Native |
| **CI/CD** | Externe | GitHub Actions | Intégré |
| **Prix (10 users)** | ~70$/mois | Gratuit | Gratuit (Premium: 200$/mois) |
| **Best for** | Grandes équipes, non-dev | Équipes GitHub | DevOps complet |

---

## Cas d'usage : Quand utiliser quoi ?

### ✅ Utiliser **GitHub Projects** si :
- Vous utilisez déjà GitHub pour le code
- Équipe < 20 personnes
- Besoin de simplicité
- Budget limité

### ✅ Utiliser **GitLab Boards** si :
- Vous voulez un outil DevOps tout-en-un
- Besoin de self-hosting
- CI/CD intégré important pour vous
- Équipe technique pure

### ✅ Utiliser **Jira** si :
- Équipes > 50 personnes
- Organisation multi-équipes
- Besoin de reporting avancé
- Équipes non-techniques incluses
- Budget disponible

---

## Démonstration pratique

### GitHub Projects (5 min)

**Créer un board pour le projet EduTask :**
1. Aller sur un repo GitHub
2. Projects → New Project → Board
3. Ajouter colonnes : Backlog / Todo / Doing / Review / Done
4. Créer 3 issues :
   - "Add task creation form"
   - "Implement task list view"
   - "Add task delete function"
5. Ajouter un champ "Story Points"
6. Drag & drop des issues
7. Configurer automation : "Auto-move to Done when closed"

### GitLab Boards (5 min)

**Créer un board Kanban :**
1. Créer un projet GitLab
2. Créer des labels scoped : `status::todo`, `status::doing`, `status::done`
3. Issues → Boards → Create Board
4. Ajouter colonnes basées sur les labels
5. Créer 2-3 issues
6. Assigner des weights (story points)
7. Déplacer sur le board

---

## Exercice à faire chez vous

**Mission :** Migrer le projet EduTask (de l'exercice Backlog Gardening) sur GitHub Projects OU GitLab Boards

**Tâches :**
1. Créer un repo sur GitHub ou GitLab
2. Créer un board avec colonnes appropriées
3. Créer les issues correspondant aux User Stories
4. Ajouter labels, assignees, story points
5. Configurer une automation
6. Prendre une capture d'écran
7. (Bonus) Faire un commit qui référence une issue

**Livrable :** Screenshot du board + lien vers le repo

---

## Ressources

### GitHub Projects
- **Docs :** https://docs.github.com/en/issues/planning-and-tracking-with-projects
- **Templates :** https://github.com/orgs/community/discussions/categories/project-templates

### GitLab Boards
- **Docs :** https://docs.gitlab.com/ee/user/project/issue_board.html
- **GitLab Learn :** https://about.gitlab.com/learn/

### Comparatifs
- "GitHub vs GitLab" : https://about.gitlab.com/devops-tools/github-vs-gitlab/
- "Jira alternatives" : https://www.g2.com/products/jira-software/competitors/alternatives

---

## Conclusion du module 1

**Ce que nous avons vu :**
1. ✅ **Introduction** : Agilité, Manifeste Agile, pourquoi des outils
2. ✅ **Scrum** : Rôles, événements, artefacts, estimation
3. ✅ **Kanban** : WIP limits, flux, métriques
4. ✅ **Jira** : Leader du marché, personnalisable, adapté aux grandes équipes
5. ✅ **GitHub/GitLab** : Intégré au code, simple, gratuit

**À retenir :**
- Pas d'outil parfait, choisir selon le contexte
- L'outil ne fait pas l'agilité, c'est l'équipe qui fait l'agilité
- Commencer simple, complexifier si nécessaire

---

**Questions / Discussion**

- Quel outil vous semble le plus adapté à vos projets actuels ?
- Avez-vous déjà utilisé l'un de ces outils ? Retour d'expérience ?
- Quelles sont vos principales questions avant de passer à la pratique ?

---

**Pause de 10 minutes avant le Module 2 (pratique)**
