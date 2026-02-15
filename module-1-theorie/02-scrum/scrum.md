# Scrum - 40 minutes

## Qu'est-ce que Scrum ?

### Définition
- **Framework agile** le plus populaire (70% des équipes agiles)
- Structure basée sur des **itérations courtes** appelées Sprints
- Équipe auto-organisée et pluridisciplinaire
- Focus sur la **livraison incrémentale de valeur**

### Les 3 piliers de Scrum
1. **Transparence** : visibilité totale pour tous les membres
2. **Inspection** : vérification régulière du progrès
3. **Adaptation** : ajustement basé sur les retours

---

## Les rôles Scrum

### 1. Product Owner (PO)
**Responsabilités :**
- Définir la vision du produit
- Gérer et prioriser le Product Backlog
- Maximiser la valeur livrée
- Interface avec les parties prenantes
- Accepter ou refuser les incréments

**Compétences clés :**
- Connaissance métier
- Capacité de décision
- Communication

### 2. Scrum Master (SM)
**Responsabilités :**
- Garant du processus Scrum
- Faciliter les événements
- Supprimer les obstacles (impediments)
- Coach de l'équipe
- Protéger l'équipe des perturbations

**Posture :**
- Servant leader
- Facilitateur, pas manager
- Agent du changement

### 3. Development Team (Équipe de développement)
**Caractéristiques :**
- 3 à 9 personnes
- Pluridisciplinaire (développeurs, testeurs, designers...)
- Auto-organisée
- Responsable de la qualité
- Engage la vélocité

**Principe :** Pas de hiérarchie interne, responsabilité collective

---

## Les événements Scrum

### Le Sprint (1-4 semaines, généralement 2 semaines)
- **Durée fixe** : timebox non modifiable
- Objectif : livrer un incrément de produit potentiellement déployable
- Démarre par le Sprint Planning
- Se termine par Sprint Review et Retrospective

### 1. Sprint Planning (2-4h pour un sprint de 2 semaines)
**Question 1 : QUOI ?**
- Définir le Sprint Goal (objectif)
- Sélectionner les User Stories du Product Backlog

**Question 2 : COMMENT ?**
- Décomposer les stories en tâches
- Estimer l'effort
- S'engager sur un périmètre réalisable

**Résultat :** Sprint Backlog

### Backlog Refinement / Grooming (1-2h par sprint)

**Qu'est-ce que c'est ?**
- Activité continue (pas un événement officiel Scrum)
- Généralement 10% du temps du sprint
- Préparation des User Stories pour les prochains sprints

**Objectifs : le "Backlog Gardening" 🌱**

Le **Product Backlog** est comme un jardin qu'il faut entretenir régulièrement :

1. **Désherber** 🌿
   - Supprimer les items obsolètes
   - Retirer ce qui n'apporte plus de valeur
   - Éliminer les doublons

2. **Tailler** ✂️
   - Découper les grosses stories (epics) en plus petites
   - Clarifier les critères d'acceptation
   - Décomposer en tâches réalisables en un sprint

3. **Fertiliser** 💧
   - Ajouter des détails aux stories du haut du backlog
   - Enrichir avec mockups, specs techniques
   - Répondre aux questions de l'équipe

4. **Réorganiser** 🔄
   - Re-prioriser selon la valeur business
   - Adapter aux nouveaux besoins
   - Grouper les items liés

5. **Estimer** 🔢
   - Planning poker pour les nouvelles stories
   - Ré-estimation si nécessaire

**Participants :**
- Product Owner (anime)
- Development Team
- Scrum Master (facilite, optionnel)

**"Ready" stories (Definition of Ready) :**
- [ ] Suffisamment détaillée
- [ ] Estimée
- [ ] Critères d'acceptation définis
- [ ] Dépendances identifiées
- [ ] Réalisable en un sprint

**Bénéfices :**
- Sprint Planning plus rapide et efficace
- Moins de surprises en cours de sprint
- Équipe alignée sur les prochaines priorités

---

### 2. Daily Scrum / Stand-up (15 min max)
**Format :** Chaque membre répond à 3 questions
1. Qu'ai-je fait hier ?
2. Que vais-je faire aujourd'hui ?
3. Ai-je des obstacles ?

**Règles :**
- Même heure, même lieu
- Debout (pour rester concis)
- Focus sur synchronisation, pas reporting
- Scrum Master note les impediments

### 3. Sprint Review (1-2h)
**Objectifs :**
- Démonstration de l'incrément
- Feedback des parties prenantes
- Adaptation du Product Backlog si nécessaire

**Participants :** Équipe Scrum + stakeholders

**Ce n'est PAS :**
- Une réunion de validation formelle
- Un reporting de statut

### 4. Sprint Retrospective (1-2h)
**But :** Amélioration continue du processus

**Questions typiques :**
- Qu'est-ce qui s'est bien passé ?
- Qu'est-ce qui pourrait être amélioré ?
- Quelles actions concrètes pour le prochain sprint ?

**Format possible :** Start / Stop / Continue

**Résultat :** Plan d'actions d'amélioration

---

## Les artefacts Scrum

### 1. Product Backlog
**Définition :**
- Liste ordonnée de tout ce qui pourrait être nécessaire dans le produit
- Unique source de vérité pour les besoins
- Vivant : évolue en permanence

**Caractéristiques :**
- **Priorisé par valeur business** (critère #1)
- Items du haut : détaillés et prêts
- Items du bas : moins détaillés
- Refinement continu (grooming)

**Format des items :** User Stories

---

## Estimation de la valeur métier

### Pourquoi estimer la valeur ?

**On estime l'effort (story points), mais aussi la VALEUR !**

**Sans estimation de valeur :**
- Risque de faire des features inutiles
- Priorisation subjective ou politique
- Pas de ROI mesurable

**Avec estimation de valeur :**
- Priorisation objective (ratio Valeur/Effort)
- Maximisation du ROI
- Alignement équipe/business

**Règle d'or :** Faire d'abord les stories à **forte valeur + faible effort** (quick wins) 🎯

---

### Méthodes d'estimation de la valeur

#### 1. Business Value Points (Fibonacci)

**Principe :** Estimer la valeur en points, comme pour l'effort

**Échelle Fibonacci :**
- **1-2** : Nice to have (faible valeur)
- **3-5** : Amélioration notable
- **8-13** : Fonctionnalité clé
- **21+** : Critique pour le business

**Critères à considérer :**
- 💰 **Revenu** : Génère-t-il des revenus directs ?
- 👥 **Impact utilisateur** : Combien d'utilisateurs concernés ?
- 📈 **Rétention** : Fidélise-t-il les utilisateurs ?
- 🚀 **Acquisition** : Attire-t-il de nouveaux utilisateurs ?
- 🔥 **Fréquence d'usage** : Quotidien ? Hebdo ? Rare ?
- 🏆 **Différenciation** : Feature unique vs standard ?
- ⚖️ **Risque** : Que se passe-t-il si on ne le fait pas ?

**Exemple :**
```
Story A : Sync Google Calendar
- Revenu : 0 (pas de monétisation directe)
- Impact : 30% des utilisateurs (étudiants qui utilisent Google)
- Rétention : Moyenne
- Acquisition : Faible
- Fréquence : Hebdomadaire
- Différenciation : Moyenne (concurrents l'ont)
→ Valeur estimée : 5 points
```

---

#### 2. WSJF (Weighted Shortest Job First)

**Origine :** Framework SAFe (Scaled Agile Framework)

**Philosophie :**
Prioriser les jobs qui ont le **plus grand coût du retard** (COD : Cost of Delay) par rapport à leur **durée**.

> "Faire d'abord ce qui coûte le plus cher si on attend"

**Formule :**
```
WSJF = Cost of Delay (CoD) / Job Duration

Où Cost of Delay = User-Business Value + Time Criticality + Risk Reduction/Opportunity
```

---

**Composantes en détail :**

### 1. User-Business Value (1-10)

**Question :** Quelle est la valeur pour les utilisateurs ET pour le business ?

**Critères d'évaluation :**

| Score | User Value | Business Value |
|-------|------------|----------------|
| **1-2** | Très peu d'utilisateurs, usage rare | Aucun impact business |
| **3-4** | Quelques utilisateurs, usage occasionnel | Impact business faible |
| **5-6** | Utilisateurs moyens, usage régulier | Impact business moyen |
| **7-8** | Beaucoup d'utilisateurs, usage fréquent | Impact business significatif |
| **9-10** | Tous les utilisateurs, usage quotidien | Impact business critique |

**Exemple :**
```
Story : "Système de notifications push"
- User Value : 9 (tous les utilisateurs, quotidien)
- Business Value : 8 (améliore rétention de 20%)
→ User-Business Value : 8-9 (on peut moyenner ou prendre le max)
```

---

### 2. Time Criticality (1-10)

**Question :** Quelle valeur perd-on si on retarde cette feature ?

**Critères d'évaluation :**

| Score | Urgence | Perte de valeur |
|-------|---------|-----------------|
| **1-2** | Pas urgent | Aucune perte si on attend 6 mois |
| **3-4** | Peu urgent | Perte mineure si on attend 3 mois |
| **5-6** | Moyennement urgent | Perte notable si on attend 1 mois |
| **7-8** | Urgent | Forte perte si on attend 2 semaines |
| **9-10** | Très urgent | Perte massive immédiate, deadline fixe |

**Exemples :**

```
Story A : "Conformité RGPD" (deadline légale 31/12)
→ Time Criticality : 10 (deadline fixe, amende si retard)

Story B : "Thème sombre"
→ Time Criticality : 2 (aucune urgence, nice to have)

Story C : "Intégration Stripe" (concurrence lance son produit dans 1 mois)
→ Time Criticality : 8 (perte d'opportunité si retard)
```

**Questions à se poser :**
- Y a-t-il une deadline contractuelle ou légale ?
- La concurrence va-t-elle nous devancer ?
- Perdons-nous des clients chaque jour sans cette feature ?
- Y a-t-il un événement (salon, lancement) qui impose une date ?

---

### 3. Risk Reduction / Opportunity Enablement (1-10)

**Question :** Cette feature réduit-elle un risque OU débloque-t-elle d'autres opportunités ?

**Deux dimensions :**

**A. Risk Reduction (Réduction de risque)**

| Score | Type de risque |
|-------|----------------|
| **1-2** | Aucun risque technique ou business |
| **3-4** | Risque mineur (workaround possible) |
| **5-6** | Risque moyen (dette technique) |
| **7-8** | Risque significatif (architecture fragile) |
| **9-10** | Risque critique (sécurité, stabilité) |

**Exemples :**
```
Story : "Refactoring du système d'authentification"
→ Risk Reduction : 8 (faille de sécurité potentielle)

Story : "Migration vers React 18"
→ Risk Reduction : 5 (dette technique, mais pas bloquant)
```

**B. Opportunity Enablement (Opportunités débloquées)**

| Score | Opportunités débloquées |
|-------|-------------------------|
| **1-2** | Aucune autre feature ne dépend de celle-ci |
| **3-4** | Facilite 1-2 features mineures |
| **5-6** | Débloque plusieurs features importantes |
| **7-8** | Fondation pour une roadmap entière |
| **9-10** | Change de paradigme, ouvre un marché |

**Exemples :**
```
Story : "API REST pour partenaires"
→ Opportunity : 9 (débloque 10+ intégrations partenaires)

Story : "Export PDF"
→ Opportunity : 2 (feature isolée, pas de dépendances)
```

**Combinaison Risk + Opportunity :**
- Prendre le **maximum** des deux
- Ou faire la **moyenne** si les deux sont significatifs

---

### 4. Job Size / Job Duration (Story Points)

**C'est simplement l'estimation d'effort** que vous avez déjà faite en Fibonacci.

**Attention :** Plus le Job Size est **petit**, plus le WSJF est **élevé** (division).

---

### Calcul WSJF complet

**Formule :**
```
WSJF = (User-Business Value + Time Criticality + Risk Reduction) / Job Size
```

**Exemple complet : EduTask**

| ID | Story | User-Biz | Time Crit | Risk/Opp | CoD (sum) | Job Size | WSJF | Rang |
|----|-------|----------|-----------|----------|-----------|----------|------|------|
| 1 | Créer tâche | 10 | 10 | 5 | **25** | 3 | **8.33** | 🥇 1 |
| 12 | Bug crash | 5 | 10 | 8 | **23** | 1 | **23.0** | 🥇 1 |
| 8 | Notif push | 9 | 8 | 3 | **20** | 5 | **4.0** | 🥈 2 |
| 13 | Voir liste | 10 | 10 | 5 | **25** | 3 | **8.33** | 🥇 1 |
| 5 | Sync Google Cal | 5 | 2 | 2 | **9** | 8 | **1.13** | 4 |
| 9 | ML prédiction | 4 | 1 | 3 | **8** | 21 | **0.38** | 5 |
| 28 | Thème sombre | 3 | 1 | 0 | **4** | 2 | **2.0** | 3 |

**Interprétation :**
- **ID 12 (Bug)** : WSJF = 23 → **PRIORITÉ ABSOLUE** (CoD énorme, effort minimal)
- **ID 1, 13** : WSJF = 8.33 → **Très haute priorité** (MVP avec bon ratio)
- **ID 8** : WSJF = 4.0 → **Haute priorité** (forte valeur, urgence)
- **ID 5** : WSJF = 1.13 → **Priorité moyenne** (effort élevé, peu urgent)
- **ID 9** : WSJF = 0.38 → **Faible priorité** (effort énorme, peu urgent)

---

### Processus d'estimation WSJF en équipe

**1. Préparation (avant la session)**
- Product Owner prépare les stories
- Équipe a déjà estimé les Job Size (story points)

**2. Estimation des 3 dimensions CoD (1h-1h30)**

**Pour chaque story :**
1. PO présente la story et le contexte business
2. **User-Business Value :** Discussion + vote (Planning Poker 1-10)
3. **Time Criticality :** PO explique urgence + équipe challenge
4. **Risk/Opportunity :** Discussion technique + vote
5. Calcul automatique du WSJF

**3. Priorisation**
- Trier par WSJF décroissant
- Valider les anomalies (stories avec WSJF très élevé ou très bas)

**Outils :**
- **Excel / Google Sheets** : Calcul automatique
- **Jira + plugin WSJF** : Champs personnalisés
- **Miro / Mural** : Workshop collaboratif

---

### Exemple de tableau Excel WSJF

```
| Story | User-Biz | Time Crit | Risk | CoD      | Size | WSJF | Rank    |
|-------|----------|-----------|------|----------|------|------|----------|
| A     | 8        | 5         | 3    | =B+C+D   | 3.   | =E/F | =RANK(G) |
```

Formules automatiques → gain de temps

---

### Quand utiliser WSJF ?

**✅ Contextes adaptés :**
- Grandes organisations (50+ personnes)
- Framework SAFe déjà en place
- Backlog avec beaucoup de dépendances techniques
- Besoin de justifier les priorités au management
- Projets avec deadlines contractuelles

**❌ Contextes moins adaptés :**
- Petites équipes (< 10 personnes) → trop complexe
- Équipes débutantes → commencer par Business Value Points
- Backlogs simples sans urgence

---

### WSJF vs Business Value Points

| Critère | Business Value Points | WSJF |
|---------|----------------------|------|
| **Complexité** | Moyenne | Haute |
| **Temps** | 30-45 min | 60-90 min |
| **Dimensions** | 1 (valeur globale) | 3 (valeur + urgence + risque) |
| **Précision** | Bonne | Excellente |
| **Idéal pour** | Équipes Scrum/Kanban | SAFe, grandes orga |
| **Participation PO** | Moyenne | Forte |
| **Prise en compte urgence** | Non (sauf manuellement) | Oui (Time Criticality) |
| **Prise en compte risque tech** | Non | Oui (Risk Reduction) |

---

### Erreurs courantes avec WSJF

❌ **Confondre User Value et Time Criticality**
- User Value = importance intrinsèque
- Time Criticality = urgence temporelle

❌ **Surestimer tous les Risk Reduction**
- Pas toutes les stories réduisent un risque
- Beaucoup sont à 0-2

❌ **Ignorer le Job Size**
- Un WSJF élevé ne veut rien dire si le Job Size est énorme
- Toujours regarder les deux

❌ **Ne pas réévaluer régulièrement**
- Time Criticality évolue avec le temps
- Recalculer tous les 1-2 mois

---

### Ressources WSJF

**Articles :**
- SAFe Framework : scaledagileframework.com/wsjf
- Don Reinertsen : "Principles of Product Development Flow" (livre de référence)

**Templates :**
- Template Excel WSJF (rechercher "WSJF calculator template")
- Jira Cloud app : "WSJF Calculator"

**Formation :**
- SAFe Product Owner/Product Manager (certification officielle)

---

---

#### 3. MoSCoW (Priorisation simple)

**Principe :** Catégoriser les stories en 4 groupes

- **M**ust have : Indispensable pour le MVP
- **S**hould have : Important mais pas bloquant
- **C**ould have : Nice to have
- **W**on't have (this time) : Pas pour cette release

**Exemple pour EduTask :**
```
Must have :
- Créer une tâche
- Voir la liste des tâches
- Marquer comme terminée

Should have :
- Modifier une tâche
- Supprimer une tâche
- Ajouter une échéance

Could have :
- Notifications push
- Filtres par matière

Won't have :
- Sync Google Calendar (v2)
- Machine Learning
```

**Avantages :** Simple, rapide, accessible aux non-tech

**Inconvénients :** Pas de granularité fine, tout devient "Must have" facilement

---

#### 4. Modèle de Kano

**Principe :** Classifier les features selon leur impact sur la satisfaction client

**3 catégories :**

1. **Basic Needs (Besoins de base)**
   - Si absent → insatisfaction
   - Si présent → satisfaction neutre
   - Ex : "Créer une tâche" dans une todo app

2. **Performance Needs (Performance)**
   - Plus c'est développé → plus de satisfaction
   - Relation linéaire
   - Ex : "Vitesse de chargement", "Nombre de filtres"

3. **Excitement Needs (Enchantement)**
   - Si absent → pas d'impact
   - Si présent → forte satisfaction (effet WOW)
   - Ex : "Suggestions intelligentes", "Gamification"

**Représentation graphique :**
```
Satisfaction ↑
                │     Excitement
                │       ╱
                │      ╱
             ───┼─────╱────────── Performance
                │    ╱
                │   ╱ Basic
                │  ╱
                └─────────────→ Fonctionnalité développée
```

**Application à la priorisation :**
- **V1/MVP** : Basic Needs en priorité
- **V2** : Performance Needs
- **V3+** : Excitement Needs

**Exemple EduTask :**
```
Basic :
- CRUD tâches
- Échéances

Performance :
- Rapidité de l'app
- Filtres avancés
- Organisation (sous-tâches, tags)

Excitement :
- Suggestions IA
- Gamification (badges, streaks)
- Collaboration temps réel
```

---

#### 5. Buy a Feature (Jeu collaboratif)

**Principe :** Jeu où les stakeholders "achètent" des features avec un budget limité

**Déroulement :**
1. Donner 100€ (fictifs) à chaque participant
2. Afficher les features avec leur "prix" (= effort)
3. Les participants achètent ce qu'ils veulent
4. Features les plus achetées = prioritaires

**Exemple :**
```
Budget : 100€ par personne

Features disponibles :
- Créer tâche : 10€
- Modifier tâche : 10€
- Supprimer tâche : 5€
- Notifications : 20€
- Sync Google Calendar : 30€
- Machine Learning : 80€

Résultat :
- Créer tâche : 5 acheteurs → Priorité 1
- Notifications : 4 acheteurs → Priorité 2
- Sync Google : 2 acheteurs → Priorité 3
- ML : 0 acheteur → Rejeté
```

**Avantages :** Ludique, engage les stakeholders, révèle les vrais besoins

**Inconvénients :** Nécessite présence des stakeholders, peut prendre du temps

---

#### 6. Impact Mapping

**Principe :** Relier les features aux objectifs business

**Structure :**
```
POURQUOI ? (Goal) → QUI ? (Actor) → COMMENT ? (Impact) → QUOI ? (Deliverable)
```

**Exemple EduTask :**
```
POURQUOI ? Augmenter la rétention à 60% en 6 mois

QUI ? Étudiants universitaires (18-25 ans)

COMMENT ?
- Les aider à ne pas oublier leurs devoirs
- Réduire leur stress lié à l'organisation

QUOI ?
→ Notifications push avant échéance (Impact fort)
→ Vue calendrier mensuel (Impact moyen)
→ Rappels quotidiens (Impact fort)
```

**Bénéfice :** Élimine les features non alignées avec l'objectif

---

### Quelle méthode choisir ?

| Méthode | Complexité | Temps | Idéal pour |
|---------|-----------|-------|------------|
| **Business Value Points** | Moyenne | 30-60 min | Équipes Scrum/Kanban classiques |
| **WSJF** | Haute | 60-90 min | Grandes organisations, SAFe |
| **MoSCoW** | Faible | 15-30 min | Kick-off projet, MVP |
| **Kano** | Moyenne | Workshop 2-3h | Définition produit, roadmap |
| **Buy a Feature** | Faible | 45-60 min | Engagement stakeholders |
| **Impact Mapping** | Moyenne | 1-2h | Stratégie produit, OKRs |

**Notre recommandation pour débutants :**
1. **MoSCoW** pour un premier tri rapide
2. **Business Value Points (Fibonacci)** pour affiner
3. **Calcul du ratio Valeur/Effort** pour prioriser

**Pour équipes matures :**
- **WSJF** si contexte SAFe ou grandes organisations
- **Impact Mapping** pour aligner stratégie et backlog


---



---

### Qui estime la valeur ?

**Product Owner** (rôle principal)
- C'est SA responsabilité
- Connaît le business et les utilisateurs

**Avec input de :**
- Stakeholders / clients
- Équipe marketing
- Sales / support client
- Data analysts (si données disponibles)

**L'équipe Dev ?**
- Généralement NON pour la valeur business
- Mais OUI pour la valeur technique (dette technique, refactoring)

---

### Exemple pratique complet

**Story :** "En tant qu'étudiant, je veux synchroniser mes tâches avec Google Calendar"

**Estimation d'effort :** 8 points (OAuth + API complexe)

**Estimation de valeur (Business Value Points) :**

| Critère | Score | Justification |
|---------|-------|---------------|
| Revenu | 0 | Pas de monétisation directe |
| Impact utilisateurs | 3 | 30% utilisent Google Calendar |
| Rétention | 2 | Améliore légèrement |
| Acquisition | 1 | Peu différenciant |
| Fréquence | 2 | Hebdomadaire |
| Différenciation | 2 | Concurrents l'ont déjà |
| **TOTAL** | **5** | Valeur moyenne |

**Ratio Valeur/Effort :** 5/8 = **0.625** (moyen, pas prioritaire)

**Décision :** Reporter à v2, faire d'abord les quick wins (forte valeur, faible effort)

---
```
En tant que [rôle]
Je veux [fonctionnalité]
Afin de [bénéfice]
```

# Sprint Backlog
**Définition :**
- Sous-ensemble du Product Backlog sélectionné pour le Sprint
- Plan pour livrer l'incrément
- Décomposé en tâches

**Propriété :** Development Team

**Visibilité :** Tableau Scrum / Kanban

# Incrément
**Définition :**
- Somme de tous les items du Product Backlog complétés durant le Sprint
- **+ tous les incréments des sprints précédents**
- Doit être potentiellement déployable

**Condition :** Respecter la **Definition of Done (DoD)**

---

## Definition of Done (DoD)

### Concept
- Accord d'équipe sur ce que "terminé" signifie
- Garantit la qualité
- Évite la dette technique

### Exemple de DoD
- [ ] Code écrit et respectant les standards
- [ ] Tests unitaires passent (couverture > 80%)
- [ ] Tests d'intégration passent
- [ ] Code review effectué
- [ ] Documentation mise à jour
- [ ] Déployé en environnement de staging
- [ ] Validé par le PO

---

## Estimation en Scrum

### Pourquoi estimer ?

**Objectifs de l'estimation :**
- **Planification** : Combien de stories dans le sprint ?
- **Prédictibilité** : Quand sera livré la feature X ?
- **Conversation** : Partager la compréhension
- **Détecter les risques** : Stories trop complexes

⚠️ **L'estimation n'est PAS :**
- Un engagement contractuel
- Une mesure de performance individuelle
- Une estimation en heures exactes

---

### Estimation relative vs absolue

**Estimation absolue (heures/jours) :**
- ❌ Difficile et imprécise
- ❌ Varie selon les personnes
- ❌ Pression sur l'équipe

**Estimation relative (points) :**
- ✅ Plus rapide et simple
- ✅ Compare les stories entre elles
- ✅ Focus sur la complexité, pas le temps

**Exemple :**
```
Story A (référence) = 3 points
Story B est 2x plus complexe → 5 points (pas 6, voir Fibonacci)
Story C est plus simple → 2 points
```

---

### Méthodes d'estimation

# Autres ressources

1. T-Shirt Sizing 👕
 2. Sprint Poker 🃏
3. Three-Point Method 🎲
4. Affinity Estimation 🤝
5. Relative Mass Evaluation ⚖️
6. Dot voting 🗳️
7. Maximum allowable size (MAS) ⛔
8. Big, Uncertain, Small 🤔
9. Weighted Shortest Job First (WSJF) 🏋️‍♀️
10. Bucket System Estimation 🪣
11. Story Counting 📊
12. #NoEstimates 🚫
🏆️ Honorable mentions

 https://www.parabol.co/blog/agile-estimation-techniques/



#### 1. Story Points (Fibonacci)

**Suite de Fibonacci : 1, 2, 3, 5, 8, 13, 21...**

**Pourquoi Fibonacci ?**
- Reflète l'**incertitude croissante**
- Évite les fausses précisions (pas de 6, 7, 9...)
- Force à faire des choix

**Échelle et signification :**

| Points | Signification | Exemple |
|--------|---------------|---------|
| **1** | Trivial, très simple | Corriger une typo |
| **2** | Simple, bien connu | Ajouter un champ dans un formulaire |
| **3** | Modéré, classique | Créer une page de login simple |
| **5** | Moyen, quelques incertitudes | Intégration d'une API externe |
| **8** | Complexe, plusieurs parties | Système de notifications push |
| **13** | Très complexe, à découper | Moteur de recherche avancé |
| **21+** | Epic, TROP GROS | → À découper absolument |

**Facteurs à considérer :**
- **Complexité technique** : Algorithme compliqué ?
- **Effort** : Beaucoup de code ?
- **Incertitude** : Technologies inconnues ?
- **Dépendances** : Beaucoup d'intégrations ?

**Exemple pratique :**
```
Référence : "Créer une tâche avec titre et description" = 3 points

→ "Créer une tâche" (juste le titre) = 2 points (plus simple)
→ "Modifier une tâche existante" = 3 points (similaire)
→ "Supprimer une tâche" = 1 point (très simple)
→ "Synchroniser avec Google Calendar" = 8 points (complexe, API externe)
→ "Système de notifications personnalisables" = 13 points (très complexe)
```

#### 2. T-Shirt Sizing

**Échelle : XS, S, M, L, XL, XXL**

**Idéal pour :**
- Débutants (plus intuitif)
- Estimation rapide / grossière
- Roadmap long terme

**Correspondance avec Fibonacci :**
| T-Shirt | Fibonacci | Signification |
|---------|-----------|---------------|
| **XS** | 1 | Très simple |
| **S** | 2-3 | Simple |
| **M** | 5 | Moyen |
| **L** | 8 | Complexe |
| **XL** | 13 | Très complexe |
| **XXL** | 21+ | Epic (à découper) |

**Exemple :**
```
"Login avec email/password" → M
"Ajouter un bouton" → XS
"Refonte du dashboard" → XL
```

**Conversion :** Une fois les stories en T-shirt, on peut convertir en Fibonacci pour le sprint planning.



---

### Planning Poker

**Le Planning Poker** est la méthode collaborative la plus utilisée pour estimer.

**Matériel :**
- Cartes avec les valeurs Fibonacci : 1, 2, 3, 5, 8, 13, 21
- Cartes spéciales :
  - **?** (pas assez d'infos)
  - **☕** (pause café !)
  - **∞** (trop gros, à découper)

**Déroulement (5-10 min par story) :**

1. **Le PO présente la User Story**
   - Lit la description
   - Explique le contexte et la valeur

2. **Questions / Clarifications**
   - Équipe pose des questions
   - PO précise les critères d'acceptation
   - Discussion technique si besoin

3. **Estimation secrète**
   - Chaque membre choisit une carte
   - **En secret** (pas d'influence)

4. **Révélation simultanée**
   - Tous montrent leur carte en même temps
   - Ex : Alice=3, Bob=5, Carol=8, David=5

5. **Discussion**
   - **Si consensus (±1 point)** → estimation retenue
   - **Si écarts importants** :
     - La personne avec l'estimation la + haute explique
     - La personne avec l'estimation la + basse explique
     - Souvent : l'un a vu une complexité que l'autre n'a pas vue

6. **Nouvelle estimation**
   - Retour à l'étape 3 avec les nouvelles infos
   - Généralement converge en 2-3 tours

**Exemple de discussion :**
```
PO : "En tant qu'utilisateur, je veux réinitialiser mon mot de passe"

Révélation : Alice=3, Bob=8, Carol=3, David=8

PO : "Bob et David, pourquoi 8 ?"
Bob : "Il faut envoyer un email sécurisé, générer un token unique, gérer l'expiration..."
Carol : "Ah oui, j'avais oublié l'email ! Je pensais juste au formulaire."

Nouvelle estimation : Alice=5, Bob=8, Carol=5, David=5
→ Consensus à 5 points
```

**Règles d'or :**
- ⏱️ **Timebox** : max 5-10 min par story (sinon passer à "?" et clarifier plus tard)
- 🎯 **Viser le consensus, pas l'unanimité** (écart de ±1 acceptable)
- 🚫 **Pas de hiérarchie** : chaque voix compte pareil
- 🤝 **Bienveillance** : pas de "ta estimation est nulle"

---

### Vélocité

**Définition :**
- Nombre de Story Points complétés par sprint
- Se stabilise après 3-4 sprints

**Utilité :**
- Prévisibilité
- Planification des releases
- Ne JAMAIS utiliser comme objectif de performance !

---

## #NoEstimates : Peut-on se passer d'estimation ?

### Le mouvement #NoEstimates

**Principe :** Certaines équipes choisissent de ne plus estimer en story points.

**Philosophie :**
- "Les estimations sont souvent fausses et coûteuses en temps"
- "Découpons plutôt toutes les stories en petits morceaux de taille similaire"
- "Comptons le nombre d'items livrés, pas les points"

**Exemple :**
```
Au lieu de :
- Story A : 8 points
- Story B : 3 points
- Story C : 13 points

On découpe tout en stories de ~1-2 jours max :
- Story A.1, A.2, A.3, A.4
- Story B
- Story C.1, C.2, C.3, C.4, C.5
```

### Approches #NoEstimates

**1. Throughput (débit)**
- Compter le nombre de stories complétées par sprint
- Moyenne : 10 stories/sprint → prédictibilité

**2. Cycle Time**
- Mesurer le temps moyen d'une story (ex: 2 jours)
- 20 stories → environ 4 semaines

**3. Story Slicing strict**
- TOUTES les stories doivent faire < 2 jours
- Si > 2 jours → découper
- Simplicité : 1 story = 1 unité de travail

### Conditions de succès du #NoEstimates

✅ **Équipe mature**
- Excellente maîtrise du découpage de stories
- Expérience suffisante du domaine

✅ **Stories homogènes**
- Discipline pour découper finement
- Accepter de ne pas tout planifier à l'avance

✅ **Flux continu**
- Fonctionne mieux en Kanban
- Moins adapté aux sprints Scrum

✅ **Stakeholders compréhensifs**
- Acceptent la variabilité
- Font confiance au débit moyen

### Quand utiliser #NoEstimates ?

**✅ Bon candidat si :**
- Équipe très expérimentée (> 1 an ensemble)
- Domaine bien maîtrisé
- Flux de travail stable et prévisible
- Stories naturellement petites
- Culture de confiance établie

**❌ À éviter si :**
- Équipe débutante en agile
- Nouveau domaine / technologie
- Besoin de prévisibilité forte (contrats, deadlines fixes)
- Stories de tailles très variables
- Management demande des engagements précis

### #NoEstimates vs Story Points

| Critère | Story Points | #NoEstimates |
|---------|--------------|--------------|
| **Temps d'estimation** | 1-2h/sprint | 0 (mais temps de slicing) |
| **Prévisibilité** | Bonne après 3-4 sprints | Bonne si stories homogènes |
| **Complexité** | Moyenne | Faible (compter) |
| **Maturité requise** | Moyenne | Haute |
| **Découpage stories** | Important | **Critique** |
| **Adaptation** | Oui (ré-estimation) | Oui (re-découpage) |

### Notre recommandation

**Pour débutants et équipes en formation :** ⭐ **Story Points**
- Apprentissage de l'estimation relative
- Conversation et partage de connaissance
- Détecter les complexités cachées

**Pour équipes très matures :** ⭐ **#NoEstimates + Throughput**
- Gain de temps
- Focus sur la livraison
- Mais nécessite discipline de slicing

**Hybride (recommandé pour équipes intermédiaires) :**
- T-Shirt sizing rapide (XS/S/M/L)
- Si > M → découper
- Compter le throughput

---

## Le tableau Scrum

### Colonnes classiques
```
| To Do | In Progress | Review | Done |
```

### Informations affichées
- **Tâches** avec assignation
- **Burndown chart** : reste à faire
- **Sprint Goal**
- **Impediments**

---

## Métriques Scrum

### 1. Burndown Chart
- **Axe X :** Jours du sprint
- **Axe Y :** Points restants
- Ligne idéale vs réalité
- Détecte les dérives tôt

### 2. Burnup Chart
- Affiche le travail complété (cumul)
- Permet de voir l'ajout de scope

### 3. Velocity Chart
- Vélocité par sprint
- Tendance sur plusieurs sprints

### 4. Cumulative Flow Diagram
- Visualise le flux de travail
- Détecte les goulots d'étranglement

---

## Métriques DORA et Scrum

### Les 4 métriques DORA (DevOps Research and Assessment)

Les **métriques DORA** mesurent la performance de livraison au niveau organisationnel, au-delà des sprints.

**Les 4 métriques :**

1. **Deployment Frequency** (Fréquence de déploiement)
   - Elite : Plusieurs fois par jour
   - Scrum typique : 1 fois par sprint (toutes les 2 semaines)

2. **Lead Time for Changes** (Temps commit → production)
   - Elite : < 1 heure
   - Scrum : Variable (peut être limité au rythme des sprints)

3. **Change Failure Rate** (% de déploiements causant un incident)
   - Elite : 0-15%
   - Indépendant de la méthodologie (qualité du code + tests)

4. **Time to Restore Service** (Temps de rétablissement après incident)
   - Elite : < 1 heure
   - Dépend de la maturité DevOps

### Scrum et DORA : Compatibilité

**✅ Compatible :**
- Scrum n'empêche PAS de déployer en continu
- Équipes Elite font Scrum + CI/CD (déploiement en cours de sprint)

**⚠️ Attention :**
- Ne pas confondre "fin de sprint" avec "déploiement"
- "Done" = potentiellement déployable ≠ déployé

**Recommandation :**
- **Découpler** le rythme des sprints du rythme de déploiement
- Déployer dès qu'une story est "Done" (pas attendre la fin du sprint)
- Mesurer DORA pour améliorer le flow global

**Pour aller plus loin :** Voir section DORA détaillée dans le cours Kanban (naturellement plus aligné avec ces métriques).

---

## Avantages et limites de Scrum

### ✅ Avantages
- Cadre structuré et éprouvé
- Feedback rapide
- Transparence totale
- Adaptabilité
- Engagement d'équipe
- Livraisons régulières

### ⚠️ Limites / Défis
- Nécessite un changement culturel
- Rôles exigeants (surtout PO et SM)
- Overhead des cérémonies
- Peut être rigide pour certains contextes
- Nécessite implication forte du client

---

## Scrum vs autres approches

### Scrum vs Cascade
| Critère | Scrum | Cascade |
|---------|-------|---------|
| Planning | Sprint par sprint | Tout au début |
| Changement | Accueilli | Coûteux |
| Risques | Réduits tôt | Découverts tard |

### Scrum vs Kanban
| Critère | Scrum | Kanban |
|---------|-------|--------|
| Itérations | Sprints fixes | Flux continu |
| Rôles | Définis (PO, SM, Dev) | Flexibles |
| Changements | Fin de sprint | Tout moment |
| Estimation | Story points | Optionnel |

---

## Cas d'usage de Scrum

**Idéal pour :**
- ✅ Développement logiciel
- ✅ Projets complexes avec incertitude
- ✅ Équipes co-localisées ou bien distribuées
- ✅ Besoins évolutifs

**Moins adapté pour :**
- ❌ Projets très courts (< 1 mois)
- ❌ Besoins 100% définis et stables
- ❌ Équipes < 3 personnes
- ❌ Contraintes réglementaires lourdes

---

## Erreurs courantes (anti-patterns)

1. **Scrum-but** : "On fait Scrum, mais..."
   - Sauter les retrospectives
   - PO absent
   - Sprints de durée variable

2. **Mini-Waterfall** : Tout concevoir au début du sprint

3. **Daily = reporting** : Stand-up devient compte-rendu au manager

4. **Vélocité comme KPI** : Pression sur les points

5. **Pas de DoD claire** : Dette technique s'accumule

6. **PO = proxy** : PO n'a pas le vrai pouvoir de décision

---

## Ressources et certifications

### Ressources gratuites
- **Scrum Guide** (scrum.org) - 13 pages, LA référence
- **Scrum Guides en français** (scrumguides.org)

### Certifications populaires
- **PSM I** (Professional Scrum Master) - Scrum.org
- **CSM** (Certified Scrum Master) - Scrum Alliance
- **PSPO** (Professional Scrum Product Owner)

---

## Exercice pratique

**Contexte :** Vous devez développer une application mobile de gestion de tâches pour étudiants.

**Questions :**
1. Qui serait votre Product Owner ?
2. Donnez 3 exemples de User Stories pour le Product Backlog
3. Quelle durée de sprint choisiriez-vous ?
4. Quels items pourrait contenir votre Definition of Done ?

---

**Transition :** Maintenant que nous maîtrisons Scrum avec ses sprints et rôles définis, explorons **Kanban**, une approche plus fluide basée sur le flux continu.
