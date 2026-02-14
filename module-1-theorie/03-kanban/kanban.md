# Kanban - 30 minutes

## Qu'est-ce que Kanban ?

### Origines
- **Années 1940** : Toyota Production System (TPS)
- **Kanban** (看板) = "panneau" ou "carte" en japonais
- Système visuel de gestion de production
- **2007** : Adapté au développement logiciel par David J. Anderson

### Définition
- **Méthode de gestion de flux** basée sur la visualisation
- Approche **pull** (tiré par la demande) vs push
- Amélioration continue (Kaizen)
- Pas de sprints ni d'itérations fixes

### Philosophie
> "Commencez avec ce que vous faites maintenant"
- Évolutif, non disruptif
- Changement incrémental
- Respect des rôles existants

---

## Les principes de Kanban

### Principes de gestion du changement
1. **Commencer par ce que vous faites actuellement**
   - Pas de réorganisation radicale
   - Comprendre le flux actuel

2. **Accepter de poursuivre avec des changements incrémentaux et évolutifs**
   - Amélioration continue
   - Résistance au changement minimale

3. **Encourager les actes de leadership à tous les niveaux**
   - Pas de rôles imposés
   - Responsabilisation collective

### Principes de livraison de service
1. **Comprendre et se concentrer sur les besoins du client**
2. **Gérer le travail, pas les personnes**
3. **Évoluer les politiques pour améliorer les résultats**

---

## Les 4 pratiques fondamentales

### 1. Visualiser le flux de travail

**Le tableau Kanban**
```
| Backlog | À faire | En cours | En test | Terminé |
|---------|---------|----------|---------|---------|
|  Story  |  Task   |   Task   |  Task   |  Task   |
|  Story  |  Task   |   Task   |         |  Task   |
|  Story  |         |          |         |  Task   |
```

**Éléments visuels :**
- **Colonnes** : étapes du processus
- **Cartes** : items de travail
- **Swimlanes** : catégories (priorité, type, équipe...)
- **Couleurs** : urgence, type de tâche

**Bénéfices :**
- Transparence totale
- Identification rapide des blocages
- Compréhension partagée

### 2. Limiter le travail en cours (WIP Limits)

**Principe :** Limiter le nombre d'items dans chaque colonne

**Exemple :**
```
| À faire | En cours (WIP: 3) | En test (WIP: 2) | Terminé |
|---------|-------------------|------------------|---------|
|  Task   |   Task            |    Task          |  Task   |
|  Task   |   Task            |    Task          |  Task   |
|  Task   |   Task            |                  |  Task   |
|         |   ❌ FULL         |    ❌ FULL       |         |
```

**Objectifs :**
- Réduire le multitasking
- Identifier les goulots d'étranglement
- Augmenter le débit (throughput)
- Améliorer la qualité

**Loi de Little :**
```
Lead Time = WIP / Throughput
```
→ Moins de WIP = Délai plus court

**Comment fixer les WIP ?**
- Commencer par WIP = nombre de personnes × 1,5
- Ajuster expérimentalement
- Observer le flux

### 3. Gérer le flux

**Objectif :** Fluidifier le travail du début à la fin

**Métriques clés :**

**Lead Time**
- Temps total de la demande à la livraison
- Inclut le temps d'attente

**Cycle Time**
- Temps de travail actif
- De "En cours" à "Terminé"

**Throughput**
- Nombre d'items livrés par unité de temps
- Ex : 10 tâches/semaine

**Flow Efficiency**
```
Flow Efficiency = Temps de travail actif / Lead Time × 100
```
- Industrie logicielle : souvent 10-15% !
- Objectif : augmenter

**Actions d'amélioration :**
- Supprimer les blocages
- Réduire les temps d'attente
- Améliorer la collaboration
- Automatiser

### 4. Rendre les règles explicites

**Politiques explicites :**
- **Definition of Ready (DoR)** : Quand peut-on commencer une tâche ?
- **Definition of Done (DoD)** : Quand une tâche est-elle finie ?
- **Règles de priorisation** : FIFO ? Par valeur ? Urgence ?
- **Critères de blocage** : Quand escalader ?

**Affichage :**
- Sur le tableau physique
- Dans l'outil numérique
- Accessible et visible

**Exemple de politique :**
```
DoR pour "En cours" :
- Critères d'acceptation définis
- Estimation réalisée
- Dépendances identifiées
```

---

## Les pratiques avancées

### 1. Boucles de feedback

**Kanban Meetings**

**Daily Standup (optionnel)**
- Focus sur le board, pas les personnes
- "Que peut-on faire pour faire avancer les tâches ?"

**Replenishment Meeting**
- Régulier (hebdo ou bi-hebdo)
- Remplir le backlog
- Prioriser

**Kanban Review**
- Démonstration des items terminés
- Feedback des stakeholders

**Retrospective**
- Amélioration du processus
- Analyser les métriques

### 2. Service Level Expectation (SLE)

**Définition :**
- Engagement de délai
- Ex : "85% des tâches seront terminées en 5 jours"

**Basé sur les données historiques**

**Permet :**
- Prévisibilité
- Gestion des attentes clients

### 3. Classes de service

**Catégorisation par urgence/importance**

| Classe | Description | WIP | Exemple |
|--------|-------------|-----|---------|
| **Expedite** | Urgent, bloquant | 1 max | Bug critique production |
| **Fixed Date** | Deadline imposée | Limité | Release contractuelle |
| **Standard** | Travail normal | Majorité | Features classiques |
| **Intangible** | Pas de deadline | Flexible | Dette technique, R&D |

**Visualisation :** Swimlanes sur le tableau

---

## Métriques Kanban

### 1. Cumulative Flow Diagram (CFD)

**Graphique empilé :**
- Axe X : Temps
- Axe Y : Nombre d'items
- Zones colorées par colonne du board

**Interprétation :**
- Largeur des bandes = WIP
- Pente = vitesse de flux
- Bandes qui s'élargissent = goulot

### 2. Lead Time & Cycle Time Distribution

**Histogramme ou percentiles**
- P50 (médiane), P85, P95
- Permet SLE

### 3. Throughput

**Nombre d'items livrés**
- Par jour/semaine
- Tendance

### 4. Blockers / Impediments

**Tracking des blocages**
- Nombre
- Durée moyenne
- Causes

---

## Métriques DORA (DevOps Research and Assessment)

### Contexte : Métriques au-delà de l'équipe

Les métriques DORA mesurent la **performance de livraison logicielle** au niveau organisationnel.

**Créées par :** Dr. Nicole Forsgren, Jez Humble, Gene Kim (livre "Accelerate")

**Applicabilité :**
- ✅ **Kanban** : Naturellement aligné (flux continu, focus sur le cycle time)
- ✅ **Scrum** : Applicable mais nécessite mesure au-delà des sprints
- ✅ **DevOps** : Contexte d'origine, fortement lié au CI/CD

---

### Les 4 métriques DORA

#### 1. Deployment Frequency (Fréquence de déploiement)

**Question :** À quelle fréquence déployez-vous en production ?

**Échelle de performance :**
- **Elite** : Multiple déploiements par jour
- **High** : Entre 1 fois par jour et 1 fois par semaine
- **Medium** : Entre 1 fois par semaine et 1 fois par mois
- **Low** : Moins d'une fois par mois

**En pratique :**
```
Kanban : Déploiement continu dès qu'une feature est Done
Scrum : Souvent 1 déploiement par sprint (toutes les 2 semaines)
```

**Lien avec agilité :**
- Kanban favorise le flux continu → déploiements fréquents
- Scrum peut limiter à la fin de sprint (sauf si CI/CD bien intégré)

---

#### 2. Lead Time for Changes (Délai de mise en production)

**Question :** Combien de temps entre le commit du code et son déploiement en production ?

**Échelle de performance :**
- **Elite** : < 1 heure
- **High** : < 1 jour
- **Medium** : 1 jour à 1 semaine
- **Low** : > 1 semaine

**Mesure :**
```
Lead Time = Temps(commit) → Temps(deploy en prod)
```

**Différence avec Kanban Lead Time :**
- **Kanban Lead Time** : Demande → Livraison (plus large, inclut analyse, dev, tests)
- **DORA Lead Time** : Code écrit → En production (focus sur le pipeline technique)

**En pratique :**
```
Kanban : Lead Time naturellement tracké, aligné avec DORA
Scrum : Peut être plus long si déploiement uniquement en fin de sprint
```

---

#### 3. Change Failure Rate (Taux d'échec des changements)

**Question :** Quel pourcentage de déploiements causent un incident en production ?

**Échelle de performance :**
- **Elite** : 0-15%
- **High** : 16-30%
- **Medium** : 16-30% (ancienne catégorie, fusion avec High)
- **Low** : > 30%

**Calcul :**
```
CFR = (Nombre de déploiements avec incident / Total déploiements) × 100
```

**Exemples d'incidents :**
- Rollback nécessaire
- Hotfix d'urgence
- Dégradation de service
- Bug critique en production

**Amélioration :**
- Tests automatisés (unit, integration, E2E)
- Code review systématique
- Feature flags / Progressive rollout
- Monitoring et alertes

---

#### 4. Time to Restore Service (Temps de rétablissement)

**Question :** Combien de temps pour rétablir le service après un incident en production ?

**Échelle de performance :**
- **Elite** : < 1 heure
- **High** : < 1 jour
- **Medium** : 1 jour à 1 semaine
- **Low** : > 1 semaine

**Mesure :**
```
MTTR = Temps(incident détecté) → Temps(service rétabli)
```

**Stratégies :**
- Monitoring et alertes proactives
- Procédures de rollback rapides
- Feature flags pour désactiver une feature
- Équipes on-call bien formées

---

### DORA : Kanban vs Scrum

| Métrique DORA | Kanban | Scrum | Qui gagne ? |
|---------------|--------|-------|-------------|
| **Deployment Frequency** | Continu (plusieurs/jour) | Souvent 1/sprint | ⭐ Kanban |
| **Lead Time for Changes** | Court, flux continu | Peut être plus long (attente fin sprint) | ⭐ Kanban |
| **Change Failure Rate** | Dépend de la qualité (neutre) | Dépend de la qualité (neutre) | ⚖️ Égalité |
| **Time to Restore** | Réactivité continue | Réactivité continue | ⚖️ Égalité |

**Conclusion :**
- **Kanban** est plus naturellement aligné avec DORA (flux continu, déploiement continu)
- **Scrum** peut atteindre les mêmes résultats MAIS nécessite de découpler le rythme de sprint du rythme de déploiement
- Les **équipes Elite** font souvent du **Scrum + CI/CD continu** (déploiement en cours de sprint)

---

### Comment mesurer DORA en pratique ?

**Outils de mesure :**
- **Jira + CI/CD** : Lier les issues aux déploiements
- **GitLab/GitHub** : Intégration native des métriques DORA
- **Datadog, New Relic** : Monitoring et MTTR
- **LinearB, Sleuth** : Plateformes dédiées aux métriques DORA

**Exemple de workflow :**
```
1. Commit code → branche feature
2. Pull Request + CI (tests auto)
3. Merge → main
4. Pipeline CD → deploy staging
5. Deploy production (auto ou manuel)

→ Chaque étape est tracée pour calculer Lead Time
```

**Intégration avec Kanban board :**
- Colonne "Deployed to Production" dans le board
- Lead Time mesuré jusqu'à cette colonne
- Automation : issue passe automatiquement à "Done" quand déployée

---

### DORA et amélioration continue

**Cycle d'amélioration :**

1. **Mesurer** les 4 métriques DORA sur 3 mois
2. **Identifier** la métrique la plus faible
3. **Analyser** les causes racines
4. **Implémenter** des améliorations
5. **Re-mesurer** après 1-2 mois

**Exemple :**
```
Problème : Change Failure Rate = 40% (Low)

Analyse :
- Tests manuels insuffisants
- Pas de staging environment
- Code review superficielle

Actions :
- Ajouter tests E2E automatisés
- Créer environnement de staging
- Checklist de code review

Résultat après 2 mois : CFR = 20% (High) ✅
```

---

### Ressources DORA

**Gratuit :**
- **State of DevOps Report** (rapport annuel) : dora.dev
- **DORA Quick Check** : Évaluation de votre niveau

**Livres :**
- **"Accelerate"** - Nicole Forsgren, Jez Humble, Gene Kim
- **"The DevOps Handbook"** - Gene Kim et al.

---

## Tableau Kanban : Conception

### Colonnes

**Approche simple :**
```
| To Do | Doing | Done |
```

**Approche détaillée :**
```
| Backlog | Ready | Dev | Code Review | Test | Deploy | Done |
```

**Colonnes avec "buffer" :**
```
| Dev - Doing | Dev - Done | Test - Doing | Test - Done |
```
→ Permet de voir où sont les files d'attente

### Swimlanes (lignes)

**Par priorité :**
```
| Expedite  |  ...  |
| High      |  ...  |
| Normal    |  ...  |
| Low       |  ...  |
```

**Par type :**
```
| Features  |  ...  |
| Bugs      |  ...  |
| Tech Debt |  ...  |
```

**Par équipe/personne :**
```
| Team A    |  ...  |
| Team B    |  ...  |
```

---

## Kanban vs Scrum

| Critère | Kanban | Scrum |
|---------|--------|-------|
| **Itérations** | Flux continu | Sprints fixes (1-4 sem) |
| **Rôles** | Optionnels | PO, SM, Dev Team |
| **WIP** | Limité par colonne | Limité par sprint |
| **Changements** | Anytime | Entre sprints |
| **Engagement** | Aucun | Sprint backlog |
| **Estimation** | Optionnelle | Story points |
| **Cérémonies** | Flexibles | 4 événements fixes |
| **Métriques** | Lead/Cycle Time | Vélocité, Burndown |
| **Planning** | Continu | Sprint Planning |

### Quand utiliser Kanban ?

**✅ Idéal pour :**
- Support / maintenance
- Flux de demandes continues
- Équipes matures
- Temps de cycle variables
- Priorités changeantes fréquemment

**✅ Exemples :**
- Support technique (tickets)
- Ops / DevOps
- Marketing (campagnes)
- Corrections de bugs

### Quand utiliser Scrum ?

**✅ Idéal pour :**
- Développement de nouvelles features
- Équipes qui démarrent l'agilité
- Besoin de cadre structuré
- Projets avec releases planifiées

---

## Scrumban : Le meilleur des deux mondes

### Concept
- Hybride Scrum + Kanban
- Structure de Scrum + Flexibilité de Kanban

### Caractéristiques
- **Sprints** (comme Scrum) OU flux continu (Kanban)
- **WIP limits** (Kanban)
- **Retrospectives** (Scrum)
- **Tableau Kanban** avec pratiques Scrum
- Planning à la demande (trigger quand backlog faible)

### Cas d'usage
- Transition Scrum → Kanban
- Équipes avec mix développement + support
- Souhait de garder certaines cérémonies Scrum

---

## Mise en place de Kanban

### Étapes

**1. Cartographier le flux actuel**
- Observer le processus existant
- Identifier les étapes

**2. Créer le tableau**
- Colonnes = étapes
- Physique OU numérique

**3. Définir les politiques**
- DoD pour chaque colonne
- Critères de transition

**4. Limiter le WIP**
- Commencer prudemment
- Ajuster progressivement

**5. Mesurer**
- Lead Time, Cycle Time
- CFD

**6. Améliorer**
- Retrospectives régulières
- Kaizen

### Erreurs à éviter

❌ **Pas de WIP limits** → retour au chaos
❌ **Trop de colonnes** → complexité
❌ **Pas de métriques** → pas d'amélioration
❌ **Ignorer les blocages** → goulots
❌ **WIP trop stricte** → frustration

---

## Kanban et amélioration continue

### Kaizen (改善)
- **Kai** = changement
- **Zen** = bon

**Principe :** Petites améliorations continues > grands changements

**Cycle PDCA :**
1. **Plan** : Identifier un problème
2. **Do** : Tester une solution
3. **Check** : Mesurer l'impact
4. **Act** : Standardiser ou ajuster

### A3 Thinking
- Résolution de problème sur une feuille A3
- Structuré : contexte, analyse, solution, plan

---

## Outils Kanban

### Physiques
- **Tableau blanc + post-its**
  - ✅ Visibilité immédiate
  - ✅ Engagement tactile
  - ❌ Équipes distribuées

### Numériques
- **Trello** : Simple, visuel
- **Jira** : Puissant, configurable
- **Azure DevOps** : Intégré Microsoft
- **Asana** : User-friendly
- **Notion / Monday** : Polyvalents

---

## Exercice pratique

**Contexte :** Vous gérez le support technique d'une application web. Vous recevez 20-30 tickets par semaine.

**Questions :**
1. Concevez un tableau Kanban adapté (colonnes, swimlanes)
2. Quelles WIP limits proposeriez-vous ?
3. Quelles métriques suivre ?
4. Proposez 2 politiques explicites (DoD, DoR, priorisation...)

**Exemple de réponse attendue :**
```
Colonnes : Backlog | Triage | In Progress (WIP:3) | Review | Done
Swimlanes : Critical / High / Normal / Low
Métriques : Lead Time, Throughput, % tickets < 48h
```

---

## Ressources

### Livres
- **"Kanban"** - David J. Anderson (LA référence)
- **"Kanban from the Inside"** - Mike Burrows

### En ligne
- **kanban.university** : Formations et certifications
- **LeanKanban.com** : Communauté

### Certifications
- **TKP** (Team Kanban Practitioner)
- **KMP** (Kanban Management Professional)

---

**Transition :** Maintenant que nous connaissons les méthodes Scrum et Kanban, voyons comment les outils comme **Jira** et **GitHub/GitLab** permettent de les mettre en pratique.
