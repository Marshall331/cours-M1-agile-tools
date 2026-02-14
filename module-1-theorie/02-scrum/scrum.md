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
- Priorisé par valeur business
- Items du haut : détaillés et prêts
- Items du bas : moins détaillés
- Refinement continu (grooming)

**Format des items :** User Stories
```
En tant que [rôle]
Je veux [fonctionnalité]
Afin de [bénéfice]
```

### 2. Sprint Backlog
**Définition :**
- Sous-ensemble du Product Backlog sélectionné pour le Sprint
- Plan pour livrer l'incrément
- Décomposé en tâches

**Propriété :** Development Team

**Visibilité :** Tableau Scrum / Kanban

### 3. Incrément
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

#### 3. Autres méthodes (pour information)

**Heures idéales**
- Estimation en heures de travail pur (sans interruptions)
- Moins utilisé car moins agile

**Points = Heures ?**
- ❌ **NON !** Ne jamais dire "1 point = 2 heures"
- Les points sont relatifs et évoluent avec l'équipe

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
