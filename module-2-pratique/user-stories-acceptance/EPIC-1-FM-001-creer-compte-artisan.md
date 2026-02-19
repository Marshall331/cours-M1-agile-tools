# US-EPIC-1-FM-001 : Créer un compte artisan

## Type
- [x] Fonctionnelle
- [ ] Technique

## Description
En tant qu'**artisan**,
Je veux **créer un compte**,
Afin de **pouvoir vendre mes produits**.

## Complexité estimée
**Story Points** : 3 pts

## Critères d'acceptation

### ☑️ Critère 1 : Formulaire d'inscription fonctionnel
- **Catégorie** : _Aucune_
- **Valeur du dé** : 🎲 **1**
- **Statut** : ⬜ Non validé
- **Permanent** : ❌ Non

**Description** : Le formulaire contient les champs email, nom, prénom, mot de passe et confirmation mot de passe avec validation côté client.

---

### ☑️ Critère 2 : Validation des données
- **Catégorie** : `[SECU]`
- **Valeur du dé** : 🎲 **4**
- **Statut** : ⬜ Non validé
- **Permanent** : ❌ Non (✅ Oui si bonus `[SECU]` actif)

**Description** : L'email est unique en base, le mot de passe respecte les règles (min 8 caractères, 1 majuscule, 1 chiffre). Messages d'erreur clairs affichés.

---

### ☑️ Critère 3 : Compte créé en base de données
- **Catégorie** : _Aucune_
- **Valeur du dé** : 🎲 **3**
- **Statut** : ⬜ Non validé
- **Permanent** : ❌ Non

**Description** : Les données sont enregistrées en base avec mot de passe hashé (bcrypt). L'utilisateur reçoit un message de confirmation.

---

### ☑️ Critère 4 : Email de bienvenue envoyé
- **Catégorie** : _Aucune_
- **Valeur du dé** : 🎲 **5**
- **Statut** : ⬜ Non validé
- **Permanent** : ❌ Non

**Description** : Un email de bienvenue est envoyé automatiquement à l'artisan après création du compte.

---

## Notes

### Dépendances
- Aucune (première story à implémenter)

### Bonus débloqué
_Aucun (US fonctionnelle)_

### Historique des tentatives

# EPIC-1-FM-1

| Sprint | Dés lancés | Critères validés | Statut |
|--------|------------|------------------|--------|
| 0 | 6 | Critère 1 : Formulaire d'inscription fonctionnel | OK |
| 0 | 2 | Critère 2 : Validation des données | OK |
| 0 | 5 | Critère 3 : Compte créé en base de données | OK |
| 0 | 4 | Critère 4 : Email de bienvenue envoyé | OK |

# EPIC-1-FM-2

| Sprint | Dés lancés | Critères validés | Statut |
|--------|------------|------------------|--------|
| 0 | 1 | Critère 1 | OK |
| 0 | 1 | Critère 2 | OK |
| 0 | 4 | Critère 3 | OK |

# EPIC-1-FM-3

| Sprint | Dés lancés | Critères validés | Statut |
|--------|------------|------------------|--------|
| 1 | 2 | Critère 1 | OK |
| 1 | 4 | Critère 2 | OK |
| 1 | 2 | Critère 3 | OK |
| 1 | 4 | Critère 4 | OK |
| 1 | 1 | Critère 5 | OK |


# EPIC-1-FM-4

| Sprint | Dés lancés | Critères validés | Statut |
|--------|------------|------------------|--------|
| 1 | 1 | Critère 1 | OK |
| 1 | 2 | Critère 2 | OK |
| 1 | 3 | Critère 3 | OK |
| 1 | 4 | Critère 4 | OK |
| 1 | 6 | Critère 5 | OK |
| 1 | 5 | Critère 6 | OK |
| 1 | 6 | Critère 7 | OK |
| 1 | 2 | Critère 8 | OK |
| 1 | 3 | Critère 9 | OK |

# EPIC-1-FM-5

| Sprint | Dés lancés | Critères validés | Statut |
|--------|------------|------------------|--------|
| 1 | 3 | Critère 1 | OK |
| 1 | 2 | Critère 2 | OK |
| 1 | 5 | Critère 3 | OK |

# EPIC-1-FM-6

| Sprint | Dés lancés | Critères validés | Statut |
|--------|------------|------------------|--------|
| 1 | 1 | Critère 1 | OK |
| 1 | 1 | Critère 2 | OK |
| 1 | 5 | Critère 3 | OK |

# Bonus CI CD

| Sprint | Dés lancés | Critères validés | Statut |
|--------|------------|------------------|--------|
| 1 | 1 | Critère 1 | OK |
| 1 | 1 | Critère 2 | OK |
| 1 | 2 | Critère 3 | OK |
| 1 | 4 | Critère 4 | OK |
| 1 | 3 | Critère 5 | OK |

# EPIC-1-FM-7

| Sprint | Dés lancés | Critères validés | Statut |
|--------|------------|------------------|--------|
| 2 | 1 | Critère 1 | OK |
| 2 | 4 | Critère 2 | OK |
| 2 | 1 | Critère 3 | OK |
| 2 | 5 | Critère 4 | OK |
| 2 | 5 | Critère 5 | OK |

# BUG 001

| Sprint | Dés lancés | Critères validés | Statut |
|--------|------------|------------------|--------|
| 2 | 6 | Critère 1 | OK |
| 2 | 6 | Critère 2 | OK |
| 2 | 9 | Critère 3 | OK |
| 2 | 1 | Critère 4 | OK |
| 2 | 3 | Critère 5 | OK ||

# EPIC-1-FM-8

| Sprint | Dés lancés | Critères validés | Statut |
|--------|------------|------------------|--------|
| 2 | 2 | Critère 1 | OK |
| 2 | 2 | Critère 2 | OK |
| 2 | 2 | Critère 3 | OK |
| 2 | 2 | Critère 4 | OK |
| 2 | 3 | Critère 4 | OK |

# Bonus infa test

| Sprint | Dés lancés | Critères validés | Statut |
|--------|------------|------------------|--------|
| 2 | 1 | Critère 1 | OK |
| 2 | 1 | Critère 2 | OK |
| 2 | 1 | Critère 3 | OK |
| 2 | 4 | Critère 4 | OK |
| 2 | 1 | Critère 4 | OK |

# BUG 02

| Sprint | Dés lancés | Critères validés | Statut |
|--------|------------|------------------|--------|
| 3 | 3 | Critère 1 | OK |
| 3 | 1 | Critère 2 | OK |
| 3 | 3 | Critère 3 | OK |
| 3 | 4 | Critère 4 | OK |
| 3 | 2 | Critère 4 | OK |

# EPIC-2-FM-9

| Sprint | Dés lancés | Critères validés | Statut |
|--------|------------|------------------|--------|
| 3 | 3 | Critère 1 | OK |
| 3 | 3 | Critère 2 | OK |
| 3 | 3 | Critère 3 | OK |
| 3 | 5 | Critère 4 | OK |
| 3 | 5 | Critère 4 | OK |

# EPIC-2-FM-10

| Sprint | Dés lancés | Critères validés | Statut |
|--------|------------|------------------|--------|
| 3 | 3 | Critère 1 | OK |
| 3 | 2 | Critère 2 | OK |
| 3 | 3 | Critère 3 | OK |
| 3 | 8 | Critère 4 | OK |
| 3 | 10 | Critère 4 | OK |
| 3 | 1 | Critère 2 | OK |
| 3 | 3 | Critère 3 | OK |
| 3 | 3 | Critère 4 | OK |
| 3 | 2 | Critère 4 | OK |

# EPIC-2-FM-11

| Sprint | Dés lancés | Critères validés | Statut |
|--------|------------|------------------|--------|
| 3 | 5 | Critère 1 | OK |
| 3 | 1 | Critère 2 | OK |
| 3 | 8 | Critère 3 | OK |
| 3 | 3 | Critère 4 | OK |
| 3 | 1 | Critère 4 | OK |

---

## Définition of Done (DoD)
- [ ] Tous les critères d'acceptation sont validés (4/4)
- [ ] Code reviewé et mergé
- [ ] Tests unitaires passent
- [ ] Démo préparée pour la revue de sprint
