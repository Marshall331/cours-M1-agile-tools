# Jira - 20 minutes

## Présentation générale

### Qu'est-ce que Jira ?

**Jira** est l'outil de gestion de projet agile le plus utilisé au monde, développé par **Atlassian** (société australienne).

**Chiffres clés :**
- 100 000+ organisations clientes
- Leader du marché (65% des équipes agiles)
- Utilisé par : Spotify, eBay, Cisco, NASA, Twitter...

**Prix :**
- Gratuit jusqu'à 10 utilisateurs
- Payant ensuite : à partir de 7$/utilisateur/mois

---

## Les produits Jira

Atlassian propose plusieurs variantes de Jira selon les besoins :

### 1. Jira Software (le plus utilisé)
- **Cible :** Équipes de développement logiciel
- **Méthodes :** Scrum, Kanban, ou hybride
- **Fonctionnalités :** Boards, Sprints, Backlog, Rapports

### 2. Jira Work Management
- **Cible :** Équipes business (marketing, RH, finance...)
- **Focus :** Gestion de projet simple sans jargon dev

### 3. Jira Service Management
- **Cible :** Équipes IT/Support
- **Usage :** Helpdesk, gestion des incidents, ITSM

### 4. Jira Align
- **Cible :** Grandes organisations
- **Usage :** Alignement stratégique et OKRs

**Dans ce cours, nous nous concentrons sur Jira Software.**

---

## Concepts de base

### Hiérarchie des items

```
Epic (Initiative)
    └── Story / Task / Bug
            └── Subtask
```

**Epic**
- Grosse fonctionnalité décomposée en plusieurs stories
- Ex : "Système de paiement en ligne"

**Story / Task / Bug**
- Unité de travail de base
- Story : fonctionnalité côté utilisateur
- Task : tâche technique
- Bug : anomalie à corriger

**Subtask**
- Décomposition d'une story
- Ex : "Créer l'API", "Créer l'interface"

---

## Interface Jira : Les vues principales

### 1. Le Backlog

**Fonctionnalités :**
- Liste de toutes les stories non planifiées
- Drag & drop pour prioriser
- Création rapide de stories
- Estimation (story points)
- Regroupement par Epics

**Actions possibles :**
- Créer des sprints
- Glisser des stories dans un sprint
- Estimer les stories
- Filtrer par epic, assignee, label...

**Vue :**
```
┌─────────────────────────────────────────┐
│ BACKLOG                                 │
├─────────────────────────────────────────┤
│ Epic: Authentification                  │
│   ☐ USER-123 Login par email    [3 pts]│
│   ☐ USER-124 Mot de passe oublié [2 pts]│
│                                         │
│ Epic: Dashboard                         │
│   ☐ DASH-45 Afficher statistiques [5pts]│
└─────────────────────────────────────────┘
```

### 2. Le Board (Tableau)

**Deux types principaux :**

**a) Scrum Board**
- Affiche les issues du sprint actif
- Colonnes : To Do / In Progress / Done
- Burndown chart visible
- Sprint goal affiché

**b) Kanban Board**
- Flux continu (pas de sprints)
- WIP limits configurables
- Cumulative Flow Diagram

**Colonnes personnalisables :**
```
| Backlog | Selected | In Dev | Code Review | QA | Done |
```

**Swimlanes (lignes horizontales) :**
- Par priorité (Highest, High, Medium, Low)
- Par assignee
- Par epic
- Requêtes personnalisées (JQL)

**Exemple visuel :**
```
┌──────────┬──────────┬──────────┬──────────┐
│ To Do    │ In Prog  │ Review   │ Done     │
├──────────┼──────────┼──────────┼──────────┤
│ USER-123 │ USER-125 │ USER-120 │ USER-110 │
│ [Alice]  │ [Bob]    │ [Carol]  │          │
│          │          │          │          │
│ USER-124 │ USER-126 │          │ USER-111 │
│ [Alice]  │ [Bob]    │          │          │
└──────────┴──────────┴──────────┴──────────┘
```

### 3. Les Sprints (Scrum uniquement)

**Fonctionnalités :**
- Créer un sprint (donner un nom, date début/fin)
- Démarrer / Terminer un sprint
- Voir le contenu du sprint
- Burndown chart en temps réel

**Actions de fin de sprint :**
- Compléter le sprint
- Déplacer les stories non terminées vers le prochain sprint ou le backlog

### 4. Les Rapports (Reports)

Jira propose de nombreux rapports prêts à l'emploi :

**Pour Scrum :**
- **Burndown Chart** : Travail restant par jour
- **Burnup Chart** : Travail complété
- **Velocity Chart** : Story points par sprint (historique)
- **Sprint Report** : Résumé du sprint (complété vs non complété)
- **Epic Burndown** : Progression sur un epic

**Pour Kanban :**
- **Cumulative Flow Diagram (CFD)**
- **Control Chart** : Lead time et cycle time
- **Throughput** : Items complétés par période

**Exemple de Burndown Chart :**
```
Points
  ↑
30│ ╲
  │   ╲___
20│       ╲___
  │           ╲___  ← Réalité
10│               ╲___
  │  ← Idéal         ╲___
 0└──────────────────────→ Jours
  0  2  4  6  8  10  12  14
```

---

## Création et gestion des issues

### Créer une issue

**Champs obligatoires :**
- **Type** : Story, Task, Bug, Epic...
- **Summary** : Titre court et descriptif
- **Project** : Projet concerné

**Champs recommandés :**
- **Description** : Détails, contexte (supporte Markdown)
- **Assignee** : Personne responsable
- **Priority** : Highest, High, Medium, Low, Lowest
- **Story Points** : Estimation (si Scrum)
- **Epic Link** : Rattachement à un epic
- **Labels** : Tags libres (ex: frontend, backend, urgent)
- **Sprint** : Sprint concerné

**Exemple de User Story dans Jira :**
```
Type: Story
Summary: En tant qu'utilisateur, je veux réinitialiser mon mot de passe

Description:
En tant qu'utilisateur ayant oublié mon mot de passe
Je veux recevoir un email de réinitialisation
Afin de retrouver l'accès à mon compte

Critères d'acceptation :
- [ ] Bouton "Mot de passe oublié" sur la page de login
- [ ] Email envoyé avec un lien unique valide 24h
- [ ] Formulaire de nouveau mot de passe sécurisé
- [ ] Confirmation visuelle après réinitialisation

Story Points: 5
Epic Link: Authentification
Priority: High
```

### Workflow des issues

**États par défaut :**
1. **To Do** : Pas encore démarré
2. **In Progress** : En cours de développement
3. **Done** : Terminé

**Workflow personnalisable :**
```
To Do → In Dev → Code Review → QA → Done
         ↓
      Blocked (en cas de problème)
```

**Transitions :**
- Cliquer sur une issue → boutons d'actions (Start Progress, Done)
- Drag & drop sur le board

---

## Fonctionnalités avancées

### 1. Automation (règles automatiques)

**Exemples d'automations :**
- "Quand une issue passe en Code Review → assigner à Alice"
- "Quand un bug est marqué High Priority → notifier sur Slack"
- "Quand toutes les subtasks sont Done → passer la story en Done"

**Configuration :** No-code (interface graphique)

**Déclencheurs (Triggers) :**
- Issue created
- Status changed
- Field value changed
- Comment added
- Scheduled (cron)

**Actions :**
- Edit issue
- Transition issue
- Send notification
- Create issue
- Comment

### 2. Filtres et JQL (Jira Query Language)

**JQL = langage de requête SQL-like**

**Exemples :**
```sql
-- Mes issues en cours
assignee = currentUser() AND status = "In Progress"

-- Bugs critiques non résolus
type = Bug AND priority = Highest AND status != Done

-- Stories du sprint actif
sprint in openSprints() AND type = Story

-- Issues créées cette semaine
created >= -1w

-- Issues avec "frontend" en label et non assignées
labels = frontend AND assignee is EMPTY
```

**Utilité :**
- Créer des dashboards personnalisés
- Filtrer le backlog
- Swimlanes personnalisées
- Notifications ciblées

### 3. Roadmaps (Epics)

**Vue timeline des Epics**
```
Q1 2024          Q2 2024         Q3 2024
|────────────────|───────────────|
[Epic: Auth     ]
                [Epic: Dashboard      ]
                                [Epic: Mobile App]
```

**Bénéfice :** Vision d'ensemble pour stakeholders

### 4. Intégrations

**Jira s'intègre avec 3000+ outils :**

**Développement :**
- **GitHub / GitLab / Bitbucket** : Lier commits et PRs aux issues
- **Slack / Teams** : Notifications
- **Confluence** : Documentation
- **Figma** : Liens vers designs

**CI/CD :**
- Jenkins, CircleCI, GitHub Actions
- Affiche les builds et déploiements dans Jira

**Exemple d'intégration GitHub :**
```bash
git commit -m "USER-123 Fix password reset bug"
# → Le commit apparaît automatiquement dans USER-123
```

---

## Scrum avec Jira : Workflow complet

### Sprint Planning
1. Aller dans le Backlog
2. Créer un nouveau sprint (bouton "Create Sprint")
3. Glisser les stories du backlog vers le sprint
4. Vérifier la vélocité (capacité de l'équipe)
5. Démarrer le sprint (bouton "Start Sprint")

### Pendant le sprint
- Daily : Consulter le Board, déplacer les cartes
- Ajouter des commentaires, logs de travail
- Créer des subtasks si nécessaire
- Marquer les issues bloquées (flag)

### Sprint Review
- Aller dans Reports → Sprint Report
- Voir les issues complétées vs non complétées
- Démontrer les fonctionnalités

### Sprint Retrospective
- Analyser le Velocity Chart
- Voir les patterns (bloquages fréquents, etc.)

### Clôture du sprint
- Bouton "Complete Sprint"
- Choisir : déplacer les stories non terminées au prochain sprint ou au backlog

---

## Kanban avec Jira : Workflow

### Configuration initiale
1. Créer un projet Kanban
2. Configurer les colonnes
3. Définir les WIP limits par colonne
4. Paramétrer les swimlanes

### Utilisation quotidienne
- Ajouter des issues dans "To Do"
- Tirer (pull) les issues quand on a de la capacité
- Respecter les WIP limits
- Analyser le CFD pour détecter les goulots

---

## Bonnes pratiques Jira

### 1. Nommage des issues
✅ **Bon :** "USER-123 : Login par email avec validation 2FA"
❌ **Mauvais :** "Login"

### 2. Descriptions détaillées
- Utiliser les templates de User Stories
- Ajouter des critères d'acceptation
- Lier des mockups/documents

### 3. Estimation
- Estimer toutes les stories du haut du backlog
- Utiliser une échelle cohérente (Fibonacci)
- Ré-estimer si besoin lors du refinement

### 4. Utiliser les Epics
- Regrouper les stories liées
- Facilite le suivi et la roadmap

### 5. Labels et composants
- **Labels** : tags libres (ex: urgent, tech-debt, frontend)
- **Components** : parties du système (ex: API, Web, Mobile)

### 6. Garder le backlog propre
- Supprimer/archiver les issues obsolètes
- Backlog grooming régulier

### 7. Commentaires et mentions
- @mention pour notifier quelqu'un
- Logger les décisions importantes

---

## Pièges courants

❌ **Too many fields** : N'ajoutez que les champs nécessaires
❌ **Workflows trop complexes** : Gardez-le simple au début
❌ **Trop de projets** : Consolider si possible
❌ **Pas de DoD** : Définissez ce que "Done" signifie
❌ **Issues trop grosses** : Découpez en subtasks
❌ **Micro-management** : Jira est un outil, pas une surveillance

---

## Jira Cloud vs Jira Server/Data Center

| Critère | Jira Cloud | Jira Server/Data Center |
|---------|------------|-------------------------|
| **Hébergement** | Atlassian (SaaS) | On-premise (vos serveurs) |
| **Mise à jour** | Automatique | Manuelle |
| **Prix** | Abonnement mensuel | Licence perpétuelle |
| **Customisation** | Limitée | Totale (accès serveur) |
| **Sécurité** | Gérée par Atlassian | Votre responsabilité |
| **Scalabilité** | Automatique | Manuelle |

**Tendance :** Atlassian pousse vers le Cloud (fin de vente des licences Server en 2024)

---

## Alternatives à Jira

| Outil | Points forts | Points faibles |
|-------|--------------|----------------|
| **Azure DevOps** | Intégration Microsoft, CI/CD intégré | Moins user-friendly |
| **GitHub Projects** | Gratuit, intégré à GitHub | Moins de fonctionnalités |
| **Linear** | Moderne, rapide, UX excellente | Jeune, moins d'intégrations |
| **Monday.com** | Visuel, polyvalent | Cher, moins orienté dev |
| **ClickUp** | Tout-en-un, personnalisable | Peut être overwhelming |
| **Asana** | Simple, collaboratif | Moins orienté développement |

**Pourquoi Jira reste leader ?**
- Écosystème riche (Atlassian suite)
- Personnalisation extrême
- Adapté aux grosses organisations
- Reporting et métriques avancées

---

## Démonstration pratique (à faire en cours)

**Scénario :** Créer un projet Scrum pour une application de todo list

**Étapes :**
1. Créer un projet Jira Scrum
2. Créer 3 Epics : Authentification, Gestion des tâches, Notifications
3. Créer 5-6 User Stories
4. Estimer les stories (Planning Poker)
5. Créer un sprint de 2 semaines
6. Glisser des stories dans le sprint
7. Démarrer le sprint
8. Faire évoluer des issues sur le board
9. Consulter le Burndown Chart
10. Compléter le sprint

**Accès démo :** https://www.atlassian.com/try/cloud/signup?bundle=jira-software

---

## Exercice pratique (à faire après le cours)

**Mission :** Configurez Jira pour le projet EduTask (app de gestion de tâches étudiantes)

**Tâches :**
1. Créer un projet Scrum "EduTask"
2. Créer 3 Epics : "Authentification", "CRUD Tâches", "Partage et collaboration"
3. Importer les User Stories de l'exercice Backlog Gardening
4. Estimer les stories
5. Créer un sprint de 2 semaines
6. Planifier le sprint avec les stories prioritaires
7. Prendre une capture d'écran du Board
8. Configurer une automation : "Quand une issue passe en Done → commenter 'Bravo !'"

**Bonus :** Créer un filtre JQL pour afficher uniquement les bugs de haute priorité

---

## Ressources

**Documentation officielle :**
- https://www.atlassian.com/software/jira/guides

**Formations gratuites :**
- Atlassian University (certifications)
- Tutoriels vidéo YouTube

**Communauté :**
- Atlassian Community Forum
- Stack Overflow (tag: jira)

---

**Transition :** Jira est l'outil de référence pour les grosses équipes et projets complexes. Mais pour les équipes qui utilisent déjà GitHub ou GitLab pour le code, pourquoi ne pas aussi gérer les projets dans ces outils ? Voyons maintenant **GitHub Projects** et **GitLab Boards**.
