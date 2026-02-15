# Exercice pratique : Backlog Gardening 🌱

**Durée :** 20-30 minutes
**Format :** Groupes de 3-4 personnes
**Objectif :** Pratiquer le refinement d'un Product Backlog en appliquant les principes du "jardinage"

---

## Contexte

Vous êtes l'équipe Scrum d'**EduTask**, une startup qui développe une application mobile de gestion de tâches pour étudiants.

Votre Product Owner vient de partir en congé maladie pour 2 semaines. Il vous a laissé le Product Backlog ci-dessous, mais celui-ci n'a pas été entretenu depuis 2 mois...

**Votre mission :** Préparer ce backlog pour les 2 prochains sprints !

---

## Product Backlog actuel (dans le désordre)

| ID | User Story | Priorité | Story Points |
|----|-----------|----------|--------------|
| 1 | En tant qu'étudiant, je veux créer une tâche avec un titre et une description | Haute | 3 |
| 2 | En tant qu'étudiant, je veux pouvoir partager mes tâches avec mes amis sur Facebook | Moyenne | ? |
| 3 | Refactoring de la base de données pour améliorer les performances | Basse | 13 |
| 4 | En tant qu'étudiant, je veux voir mes tâches classées par date d'échéance | Haute | 5 |
| 5 | En tant qu'étudiant, je veux synchroniser mes tâches avec Google Calendar | Haute | ? |
| 6 | En tant qu'étudiant, je veux créer une tâche | Haute | 3 |
| 7 | En tant qu'utilisateur premium, je veux créer des listes de tâches personnalisées | Moyenne | ? |
| 8 | En tant qu'étudiant, je veux recevoir une notification push 1h avant une échéance | Haute | ? |
| 9 | Implémenter l'algorithme de machine learning pour prédire le temps nécessaire par tâche | Moyenne | ? |
| 10 | En tant qu'étudiant, je veux marquer une tâche comme terminée | Haute | ? |
| 11 | En tant qu'étudiant, je veux pouvoir imprimer mes tâches de la semaine | Basse | ? |
| 12 | Corriger le bug : l'app crash quand on crée une tâche sans titre | ? | 1 |
| 13 | En tant qu'étudiant, je veux voir toutes mes tâches dans une liste | ? | ? |
| 14 | Support du Metaverse pour visualiser les tâches en VR | ? | 34 |
| 15 | En tant qu'étudiant, je veux modifier une tâche existante | ? | 3 |
| 16 | En tant qu'étudiant, je veux supprimer une tâche | ? | 2 |
| 17 | En tant qu'étudiant, je veux ajouter des sous-tâches à une tâche | Moyenne | 8 |
| 18 | En tant qu'étudiant, je veux filtrer mes tâches par matière (Maths, Anglais, etc.) | Moyenne | 5 |
| 19 | Mise à jour vers la dernière version de React Native | Moyenne | 5 |

**Informations complémentaires :**
- Votre vélocité moyenne : **15 story points par sprint**
- Durée du sprint : **2 semaines**
- Contexte business : Vous lancez une version beta publique dans 1 mois
- L'item #6 est identique au #1 (doublon créé par erreur)
- Facebook n'est plus utilisé par votre cible (étudiants de 18-25 ans)
- Le Product Owner avait mentionné que le Metaverse était une "idée jetée en brainstorming à revoir plus tard"

---

## Mission 1 : Désherber 🌿 (5 minutes)

**Identifiez les items à supprimer ou mettre en "icebox" (parking)**

Questions à vous poser :
- Y a-t-il des doublons ?
- Certaines stories sont-elles obsolètes ou sans valeur ?
- Y a-t-il des "nice to have" qui ne sont pas prioritaires pour la beta ?

**Listez les IDs des stories à retirer et justifiez :**

```
À supprimer/mettre en icebox :
- ID __ : raison
- ID __ : raison
...
```

---

## Mission 2 : Estimer l'effort avec Planning Poker 🔢 (10-15 minutes)

**Objectif :** Estimer les stories prioritaires avec Planning Poker

### Rappel des méthodes d'estimation

**Méthode : Story Points (Fibonacci)**
- Échelle : **1, 2, 3, 5, 8, 13, 21**
- Estimation **relative** (comparer à la story de référence)
- Prendre en compte : **Complexité + Effort + Incertitude**

**Référence :** ID #1 = 3 points (créer une tâche avec titre et description)

**Méthode alternative : T-Shirt Sizing**
- Échelle : **XS, S, M, L, XL**
- Plus rapide pour un premier tri
- Conversion : XS=1, S=2-3, M=5, L=8, XL=13

### Processus de Planning Poker

**Pour chaque story avec "?" :**
1. Lecture de la story
2. Questions/clarifications (2 min max)
3. Estimation secrète (chacun choisit une carte Fibonacci)
4. Révélation simultanée
5. Discussion si écarts > 2 points
6. Nouvelle estimation jusqu'à consensus

### Stories à estimer en priorité

**Commencez par les stories de haute priorité :**
- ID 5, 7, 8, 9, 10, 13, 15, 16

**Remplissez le tableau d'estimation :**

| ID | Story résumée | Fibonacci | Justification |
|----|---------------|-----------|---------------|
| 5 | Sync Google Calendar | ___ | OAuth + API complexe ? |
| 7 | Listes personnalisées | ___ | Groupement logique ? |
| 8 | Notif push 1h avant | ___ | Service externe ? |
| 9 | ML prédiction temps | ___ | Probablement > 13 |
| 10 | Marquer terminée | ___ | Plus simple que créer ? |
| 13 | Voir liste tâches | ___ | Similaire à #1 ? |
| 15 | Modifier tâche | ___ | Même que créer ? |
| 16 | Supprimer tâche | ___ | Très simple ? |

**Continuez avec les autres stories si le temps le permet.**

---

## Mission 3 : Estimer la valeur métier 💰 (15-20 minutes)

**Objectif :** Estimer la **valeur business** de chaque story avec une méthode structurée


### Critères de valeur

- **Impact utilisateur :** Combien d'utilisateurs en bénéficient ?
- **Fréquence d'utilisation :** Quotidienne ? Hebdomadaire ? Rare ?
- **Différenciation :** Feature unique vs standard ?
- **Impact business :** Revenu ? Rétention ? Acquisition ?


### Étape 1 : Choisir une méthode (5 min)

Votre équipe doit choisir UNE méthode parmi :

**Option A : Business Value Points (Fibonacci) - Recommandé pour débutants**
- Échelle 1, 2, 3, 5, 8, 13, 21
- Estimation relative basée sur des critères

**Option B : MoSCoW + Value Points**
- D'abord catégoriser (Must/Should/Could/Won't)
- Puis affiner avec des points dans chaque catégorie

**Option C : WSJF (Weighted Shortest Job First) - Pour avancés**
- Calcul : (User Value + Time Criticality + Risk) / Effort
- Plus complexe mais plus complet

---

### Étape 2 : Si vous choisissez Business Value Points (recommandé)

**Échelle de valeur métier (Fibonacci) :**
- **1-2 points :** Nice to have (faible valeur)
- **3-5 points :** Amélioration notable
- **8-13 points :** Fonctionnalité clé
- **21+ points :** Critique pour le lancement

**Critères d'évaluation (utilisez au moins 4) :**

| Critère | Question à se poser | Poids |
|---------|---------------------|-------|
| 💰 **Revenu** | Génère des revenus directs ? | 0-5 |
| 👥 **Impact utilisateur** | % d'utilisateurs concernés ? | 0-5 |
| 📈 **Rétention** | Fidélise-t-il les utilisateurs ? | 0-5 |
| 🚀 **Acquisition** | Attire nouveaux utilisateurs ? | 0-5 |
| 🔥 **Fréquence** | Usage quotidien/hebdo/rare ? | 0-3 |
| 🏆 **Différenciation** | Feature unique vs standard ? | 0-5 |
| ⚖️ **Risque** | Que se passe-t-il si on ne le fait pas ? | 0-5 |

**Exemple pour ID 8 (Notifications push) :**

| Critère | Score | Justification |
|---------|-------|---------------|
| Revenu | 1 | Pas de revenu direct |
| Impact utilisateur | 5 | 100% des utilisateurs concernés |
| Rétention | 5 | Critiq ue pour ne pas oublier tâches |
| Acquisition | 2 | Feature standard (concurrents l'ont) |
| Fréquence | 3 | Usage quotidien |
| Différenciation | 2 | Standard |
| Risque | 5 | Sans ça, app peu utile |
| **TOTAL** | **23** → **13 pts** (Fibonacci) | Valeur HAUTE |

**Grille d'estimation rapide :**
- Total < 10 → 1-3 pts
- Total 10-15 → 5 pts
- Total 16-25 → 8 pts
- Total 26-35 → 13 pts
- Total > 35 → 21 pts

**Estimez VOS stories prioritaires :**

| ID | Story | Rev | Impact | Ret | Acq | Freq | Diff | Risk | Total | Value (Fib) |
|----|-------|-----|--------|-----|-----|------|------|------|-------|-------------|
| 1 | Créer tâche | 0 | 5 | 5 | ___ | ___ | ___ | 5 | ___ | ___ |
| 10 | Marquer terminée | ___ | ___ | ___ | ___ | ___ | ___ | ___ | ___ | ___ |
| 13 | Voir liste | ___ | ___ | ___ | ___ | ___ | ___ | ___ | ___ | ___ |
| 15 | Modifier | ___ | ___ | ___ | ___ | ___ | ___ | ___ | ___ | ___ |
| 16 | Supprimer | ___ | ___ | ___ | ___ | ___ | ___ | ___ | ___ | ___ |
| 8 | Notif push | 1 | 5 | 5 | 2 | 3 | 2 | 5 | 23 | 13 |
| 5 | Sync Google Cal | ___ | ___ | ___ | ___ | ___ | ___ | ___ | ___ | ___ |
| 7 | Listes perso | ___ | ___ | ___ | ___ | ___ | ___ | ___ | ___ | ___ |
| 17 | Sous-tâches | ___ | ___ | ___ | ___ | ___ | ___ | ___ | ___ | ___ |

---

### Étape 2 bis : Si vous choisissez MoSCoW (alternative rapide)

**Classez d'abord les stories :**

**Must have (MVP) :**
- Sans ces features, le produit est inutilisable
- Ex : _______________

**Should have (important) :**
- Importantes mais contournables temporairement
- Ex : _______________

**Could have (nice to have) :**
- Améliorent l'expérience mais pas critiques
- Ex : _______________

**Won't have (pas cette version) :**
- Bonnes idées mais pas pour la beta
- Ex : _______________

**Puis affinez avec des points :**
- Must : 13-21 pts par défaut
- Should : 5-8 pts
- Could : 2-3 pts
- Won't : 0-1 pt

---

### Étape 2 ter : Si vous choisissez WSJF (avancé)

**Méthode WSJF (Weighted Shortest Job First) du framework SAFe**

> **Philosophie :** "Faire d'abord ce qui coûte le plus cher si on attend"

**Formule :**
```
WSJF = Cost of Delay (CoD) / Job Size

Où CoD = User-Business Value + Time Criticality + Risk Reduction/Opportunity
```

---

**Pour chaque story, estimez 3 dimensions (échelle 1-10) :**

#### 1. User-Business Value (1-10)

**Question :** Quelle valeur pour les utilisateurs ET le business ?

| Score | Signification |
|-------|---------------|
| 1-2 | Très peu d'utilisateurs, aucun impact business |
| 3-4 | Quelques utilisateurs, impact business faible |
| 5-6 | Usage moyen, impact business moyen |
| 7-8 | Beaucoup d'utilisateurs, impact business fort |
| 9-10 | Tous les utilisateurs, impact business critique |

**Exemples EduTask :**
```
ID 1 (Créer tâche) : 10 (sans ça, app inutile)
ID 8 (Notif push) : 9 (tous utilisateurs, usage quotidien)
ID 28 (Thème sombre) : 3 (confort visuel, pas essentiel)
```

---

#### 2. Time Criticality (1-10)

**Question :** Quelle valeur perd-on si on retarde ?

| Score | Urgence |
|-------|---------|
| 1-2 | Pas urgent (6 mois OK) |
| 3-4 | Peu urgent (3 mois OK) |
| 5-6 | Moyennement urgent (1 mois max) |
| 7-8 | Urgent (2 semaines max) |
| 9-10 | Très urgent (deadline fixe, perte immédiate) |

**Questions à se poser :**
- Y a-t-il une deadline contractuelle ou légale ?
- La concurrence va-t-elle nous devancer ?
- Lance-t-on une beta publique dans 1 mois ?

**Exemples EduTask :**
```
ID 12 (Bug crash) : 10 (bloque le lancement beta)
ID 1 (Créer tâche) : 10 (MVP pour beta dans 1 mois)
ID 5 (Sync Google Cal) : 2 (nice to have, pas urgent)
ID 28 (Thème sombre) : 1 (aucune urgence)
```

---

#### 3. Risk Reduction / Opportunity Enablement (1-10)

**Deux sous-dimensions :**

**A. Risk Reduction (Réduction de risque)**
- Réduit-on un risque technique, sécurité, ou business ?

| Score | Type de risque |
|-------|----------------|
| 1-2 | Aucun risque |
| 3-4 | Risque mineur (workaround possible) |
| 5-6 | Dette technique moyenne |
| 7-8 | Risque significatif (architecture, sécurité) |
| 9-10 | Risque critique |

**B. Opportunity Enablement (Opportunités débloquées)**
- Cette feature débloque-t-elle d'autres features importantes ?

| Score | Opportunités |
|-------|--------------|
| 1-2 | Feature isolée, aucune dépendance |
| 3-4 | Facilite 1-2 features mineures |
| 5-6 | Débloque plusieurs features |
| 7-8 | Fondation pour roadmap entière |
| 9-10 | Change de paradigme |

**Combinaison :** Prendre le **maximum** des deux

**Exemples EduTask :**
```
ID 12 (Bug crash) : 8 (risque de perdre utilisateurs, mauvaise réputation)
ID 20 (Ajouter échéance) : 5 (débloque ID 4 "Trier par date", ID 8 "Notif")
ID 28 (Thème sombre) : 0 (feature isolée)
```

---

**Tableau d'estimation WSJF :**

| ID | Story | User-Biz (1-10) | Time Crit (1-10) | Risk/Opp (1-10) | CoD (sum) | Effort | WSJF | Rang |
|----|-------|-----------------|------------------|-----------------|-----------|--------|------|------|
| 1 | Créer tâche | 10 | 10 | 5 | **25** | 3 | **8.3** | 🥇 |
| 12 | Bug crash | 5 | 10 | 8 | **23** | 1 | **23.0** | 🥇 |
| 8 | Notif push | 9 | 8 | 3 | **20** | 5 | **4.0** | 🥈 |
| 13 | Voir liste | 10 | 10 | 5 | **25** | 3 | **8.3** | 🥇 |
| 20 | Échéance | 8 | 7 | 5 | **20** | 2 | **10.0** | 🥇 |
| 5 | Sync Google | 5 | 2 | 2 | **9** | 8 | **1.1** | 4 |
| 28 | Thème sombre | 3 | 1 | 0 | **4** | 2 | **2.0** | 3 |

**Interprétation du WSJF :**
- **WSJF > 5** : Priorité TRÈS HAUTE (quick wins avec urgence)
- **WSJF 2-5** : Priorité HAUTE
- **WSJF 1-2** : Priorité MOYENNE
- **WSJF < 1** : Faible priorité (reporter)

**Votre tableau à remplir :**

| ID | Story résumée | User-Biz | Time Crit | Risk/Opp | CoD | Effort | WSJF |
|----|---------------|----------|-----------|----------|-----|--------|------|
| 1 | Créer | ___ | ___ | ___ | =sum | 3 | =CoD/Effort |
| 10 | Marquer done | ___ | ___ | ___ | ___ | 2 | ___ |
| 13 | Voir liste | ___ | ___ | ___ | ___ | 3 | ___ |
| 15 | Modifier | ___ | ___ | ___ | ___ | 3 | ___ |
| 16 | Supprimer | ___ | ___ | ___ | ___ | 1 | ___ |
| 8 | Notif push | ___ | ___ | ___ | ___ | 5 | ___ |
| 5 | Sync Google | ___ | ___ | ___ | ___ | 8 | ___ |

**Astuce :** Utilisez un tableur (Excel/Google Sheets) pour calculer automatiquement WSJF et trier !

---

### Étape 3 : Calculer le ratio Valeur/Effort (5 min)

**Pour CHAQUE story estimée, calculez :**

```
Ratio V/E = Valeur (points) / Effort (points)
```

**Grille d'interprétation :**
- **Ratio > 3.0** : ⭐⭐⭐ EXCELLENT (Quick win, à faire en priorité)
- **Ratio 1.5-3.0** : ⭐⭐ BON (Valeur intéressante)
- **Ratio 0.5-1.5** : ⭐ MOYEN (À évaluer selon contexte)
- **Ratio < 0.5** : ❌ FAIBLE (Reporter ou abandonner)

**Remplissez votre matrice :**

| ID | Story | Valeur | Effort | Ratio V/E | Catégorie | Action |
|----|-------|--------|--------|-----------|-----------|--------|
| 16 | Supprimer | 5 | 1 | **5.0** | ⭐⭐⭐ | Sprint 1 |
| 10 | Marquer terminée | 13 | 2 | **6.5** | ⭐⭐⭐ | Sprint 1 |
| 1 | Créer tâche | 21 | 3 | **7.0** | ⭐⭐⭐ | Sprint 1 |
| 13 | Voir liste | 21 | 3 | **7.0** | ⭐⭐⭐ | Sprint 1 |
| 15 | Modifier | 8 | 3 | **2.7** | ⭐⭐ | Sprint 1-2 |
| 8 | Notif push | 13 | 5 | **2.6** | ⭐⭐ | Sprint 2 |
| 17 | Sous-tâches | 8 | 8 | **1.0** | ⭐ | Sprint 3+ |
| 5 | Sync Google | 5 | 8 | **0.6** | ⭐ | v2 |
| ... | ... | ... | ... | ... | ... | ... |

---

### Étape 4 : Matrice de priorisation visuelle (optionnel, 5 min)

**Placez vos stories sur cette matrice :**

```
Valeur ↑
   │
21 │  [1] [13]
   │
13 │  [10] [8]
   │
 8 │  [15]      [17]
   │
 5 │  [16]            [5]
   │
 1 │
   └────────────────────────→ Effort
     1    2    3    5    8   13

Quadrants :
- Haut-Gauche = PRIORITÉ MAX (forte valeur, faible effort)
- Haut-Droit = À ÉVALUER (forte valeur, fort effort)
- Bas-Gauche = Quick wins secondaires
- Bas-Droit = À ÉVITER ou REPORTER
```

**Leçons à tirer :**
- Stories dans le quadrant haut-gauche → Sprint 1
- Stories dans le quadrant haut-droit → Découper si possible, sinon Sprint 2-3
- Stories dans le quadrant bas-droit → v2 ou abandonner

---

### Questions de débriefing

1. Quelle méthode avez-vous choisie ? Pourquoi ?
2. Quelles stories ont la valeur la plus élevée ? Correspond-elle à votre intuition initiale ?
3. Y a-t-il des surprises (stories que vous pensiez importantes mais avec faible ratio) ?
4. En situation réelle, qui devrait faire cette estimation de valeur ? (PO seul ? Avec stakeholders ?)
5. Combien de temps cela prendrait en vrai ? (estimation : 1-2h pour 20-30 stories)

---

## Mission 4 : Tailler ✂️ (5 minutes)

**Identifiez les stories trop grosses (epics) à découper**

Maintenant que vous avez les estimations, identifiez les epics :
- Règle : Une story > 13 points est trop grosse pour un sprint et doit être découpée

**Pour chaque epic identifié, proposez un découpage :**

Exemple :
```
ID 9 (21+ pts) → À découper en :
  - Story 9.1 : Recherche et spike sur les algos ML (5 pts)
  - Story 9.2 : Collecte des données utilisateur (3 pts)
  - Story 9.3 : Implémentation du modèle (8 pts)
  - Story 9.4 : Intégration dans l'app (5 pts)
```

---

## Mission 5 : Fertiliser 💧 (5 minutes)

**Enrichissez 2-3 stories du haut du backlog**

Choisissez 2-3 stories prioritaires qui manquent d'informations :
- Ajoutez des **critères d'acceptation**
- Précisez les **dépendances techniques**
- Posez des **questions au PO** (à simuler)

**Exemple pour l'ID 5 (Sync Google Calendar) :**

**Critères d'acceptation :**
- [ ] L'utilisateur peut connecter son compte Google
- [ ] Les tâches créées dans l'app apparaissent dans Google Calendar
- [ ] Les modifications dans l'app sont synchronisées
- [ ] Un indicateur de synchro est visible

**Questions au PO :**
- La synchro doit-elle être bidirectionnelle (Google → App aussi) ?
- Faut-il supporter d'autres calendriers (Outlook, Apple) ?

**Dépendances techniques :**
- API Google Calendar
- OAuth 2.0 pour l'authentification

---

## Mission 6 : Réorganiser / Prioriser 🔄 (5 minutes)

**Re-priorisez le backlog en utilisant les estimations d'effort ET de valeur**

### Critères de priorisation

1. **Bugs critiques** (bloquants) → Toujours en premier
2. **Ratio Valeur/Effort élevé** → Quick wins 🎯
3. **MVP / Fonctionnalités de base** (CRUD)
4. **Fonctionnalités à forte valeur**
5. **Améliorations techniques**
6. **Nice to have** (faible valeur ou fort effort)

### Matrice de priorisation (optionnel mais recommandé)

```
Valeur ↑
   │
13 │  [13]        [5]
   │
 8 │  [10] [1]
   │  [16]
 5 │              [8]
   │
 3 │  [15]
   │
 1 │         [ML:9]
   └──────────────────→ Effort
     1  2  3  5  8  13

Légende :
- Quadrant haut-gauche = Priorité MAX (forte valeur, faible effort)
- Quadrant haut-droit = À évaluer (forte valeur, fort effort)
- Quadrant bas-gauche = Quick wins secondaires
- Quadrant bas-droit = À éviter/reporter
```

**Créez le backlog réorganisé (top 15 minimum) :**

| Rang | ID | Story | Valeur | Effort | Ratio | Justification |
|------|----|-------|--------|--------|-------|---------------|
| 1 | 12 | Bug crash | - | 1 | ∞ | Bug critique |
| 2 | __ | ______ | __ | __ | __ | ___________ |
| 3 | __ | ______ | __ | __ | __ | ___________ |
| ... | | | | | | |

---

## Mission 7 : Sprint Planning (5-10 minutes)

**Sélectionnez les stories pour le prochain sprint**

Contraintes :
- Vélocité = 15 points max
- Stories doivent être "Ready" (DoR)

**Definition of Ready :**
- [ ] Story claire et détaillée
- [ ] Critères d'acceptation définis
- [ ] Estimée
- [ ] Pas de dépendances bloquantes

**Votre Sprint Backlog :**
```
Sprint Goal : ___________

Stories sélectionnées :
- ID __ (__ pts)
- ID __ (__ pts)
- ID __ (__ pts)

Total : __ points
```

---

## Débriefing collectif (10 minutes)

**Questions de réflexion :**

1. **Sur l'estimation :**
   - Quelles stories ont généré le plus de débat ? Pourquoi ?
   - Avez-vous eu des écarts importants lors du Planning Poker ? Comment les avez-vous résolus ?
   - Fibonacci vs T-Shirt : quelle méthode préférez-vous ?

2. **Sur le Backlog Gardening :**
   - Combien de stories avez-vous supprimées/mises en icebox ?
   - Comment avez-vous géré les stories sans estimation ?
   - Avez-vous été tentés de garder trop de stories "au cas où" ?

3. **Sur le processus :**
   - Comment le backlog gardening améliore-t-il le Sprint Planning ?
   - En situation réelle, qui prend ces décisions ? (PO ? Équipe ? Ensemble ?)
   - Combien de temps faudrait-il pour ce refinement en vrai ? (estimation : 1h-1h30)

---

## Corrigé suggéré

### Désherber 🌿
**À supprimer/icebox :**
- **ID 6** : Doublon de ID 1
- **ID 2** : Obsolète (Facebook non utilisé par la cible)
- **ID 14** : Metaverse = icebox (pas prioritaire pour beta)
- **ID 11** : Impression = faible valeur ajoutée pour une app mobile

### Tailler ✂️
**Epics à découper :**
- **ID 9 (21 pts)** : ML trop complexe → à découper ou reporter
- **ID 3 (13 pts)** : Refactoring BDD → acceptable mais à détailler

### Réorganiser 🔄
**Backlog priorisé :**
1. **ID 12** (Bug critique)
2. **ID 1** (Créer tâche - MVP)
3. **ID 13** (Voir toutes les tâches - MVP)
4. **ID 10** (Marquer terminée - MVP)
5. **ID 15** (Modifier tâche - MVP)
6. **ID 16** (Supprimer tâche - MVP)
7. **ID 4** (Tri par date)
8. **ID 8** (Notifications)
9. **ID 18** (Filtres par matière)
10. **ID 7** (Listes personnalisées)
11. **ID 17** (Sous-tâches)
12. **ID 5** (Sync Google Calendar)
13. **ID 19** (Update React Native)
14. **ID 3** (Refactoring BDD)

### Estimation Effort (Fibonacci)

**Stories prioritaires :**
- **ID 5** (Sync Google Calendar) : **8 pts** - OAuth + API Google complexe
- **ID 7** (Listes personnalisées) : **5 pts** - Groupement logique + UI
- **ID 8** (Notif push) : **5 pts** - Service externe (Firebase/OneSignal)
- **ID 10** (Marquer terminée) : **2 pts** - Toggle simple
- **ID 13** (Voir liste) : **3 pts** - Affichage similaire à #1
- **ID 15** (Modifier) : **3 pts** - Formulaire similaire à #1
- **ID 16** (Supprimer) : **1 pt** - Très simple (DELETE)

**Stories secondaires :**
- **ID 2** (Facebook) : **5 pts** - API externe → mais à supprimer
- **ID 9** (ML) : **21+ pts** - Trop complexe, à découper
- **ID 11** (Imprimer) : **3 pts** - Génération PDF basique
- **ID 17** (Sous-tâches) : **8 pts** - Hiérarchie BDD + UI arbre
- **ID 18** (Filtrer matière) : **5 pts** - Filtres + catégories
- **ID 19** (Update React Native) : **5 pts** - Risques breaking changes

### Estimation Valeur Métier (Fibonacci)

**Stories MVP (haute valeur) :**
- **ID 1** (Créer tâche) : **21 pts** - Sans ça, pas d'app
- **ID 13** (Voir liste) : **21 pts** - Essentiel
- **ID 10** (Marquer terminée) : **13 pts** - Fonctionnalité de base
- **ID 15** (Modifier) : **8 pts** - Corriger erreurs fréquent
- **ID 16** (Supprimer) : **5 pts** - Nettoyage utile
- **ID 12** (Bug crash) : **∞** - Bloquant

**Stories différenciation (valeur moyenne-haute) :**
- **ID 8** (Notif push) : **13 pts** - Forte valeur ajoutée, usage quotidien
- **ID 5** (Sync Google Calendar) : **8 pts** - Différenciation mais niche
- **ID 17** (Sous-tâches) : **8 pts** - Améliore organisation
- **ID 18** (Filtrer matière) : **5 pts** - Utile pour étudiants

**Stories nice-to-have (valeur faible) :**
- **ID 7** (Listes premium) : **3 pts** - Feature payante, petit segment
- **ID 11** (Imprimer) : **1 pt** - Faible usage
- **ID 19** (Update RN) : **2 pts** - Technique, pas user-facing

### Priorisation par Ratio Valeur/Effort

| ID | Story | Valeur | Effort | Ratio | Priorité |
|----|-------|--------|--------|-------|----------|
| 16 | Supprimer | 5 | 1 | **5.0** | ⭐⭐⭐ |
| 10 | Marquer terminée | 13 | 2 | **6.5** | ⭐⭐⭐ |
| 1 | Créer tâche | 21 | 3 | **7.0** | ⭐⭐⭐ |
| 13 | Voir liste | 21 | 3 | **7.0** | ⭐⭐⭐ |
| 15 | Modifier | 8 | 3 | **2.7** | ⭐⭐ |
| 8 | Notif push | 13 | 5 | **2.6** | ⭐⭐ |
| 18 | Filtrer matière | 5 | 5 | **1.0** | ⭐ |
| 5 | Sync Google Cal | 8 | 8 | **1.0** | ⭐ |
| 17 | Sous-tâches | 8 | 8 | **1.0** | ⭐ |

**Conclusion priorisation :**
1. Bug critique (#12)
2. Quick wins MVP : #1, #13, #10, #16 (ratio élevé)
3. Compléter CRUD : #15
4. Valeur ajoutée : #8 (notifications)
5. Reporter : #5, #17 (fort effort, ratio moyen)

### Sprint Backlog suggéré
**Sprint Goal :** *Livrer le CRUD complet des tâches*

**Stories sélectionnées :**
- ID 12 : Bug crash (1 pt)
- ID 1 : Créer tâche (3 pts)
- ID 13 : Voir liste (3 pts)
- ID 10 : Marquer terminée (2 pts)
- ID 15 : Modifier (3 pts)
- ID 16 : Supprimer (1 pt)

**Total : 13 points / 15** ✅

**Alternative (si équipe expérimentée) :**
Ajouter ID 20 (Ajouter échéance - 2pts estimés) → Total 15 points

---

## Variante pour aller plus loin

**Après avoir fait l'exercice une fois, ajoutez cette contrainte :**

> "Le CEO annonce que Google vous propose un partenariat si vous intégrez Google Calendar dans le mois. Cela peut débloquer un financement de 100k€."

**Question :** Comment re-priorisez-vous le backlog ? Quelles stories sacrifiez-vous pour intégrer l'ID 5 ?

→ Cet exercice montre l'importance de l'**agilité** et de la **re-priorisation continue** !
