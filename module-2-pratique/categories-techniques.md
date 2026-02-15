# Catégories de critères techniques

Ce document définit les catégories de critères techniques et les bonus qu'elles débloquent dans le jeu.

---

## `[INFRA_TEST]` - Infrastructure de test

### User Stories techniques associées
- Environnement de test isolé
- Données de test automatisées
- Base de données de test dédiée
- Containers de test (Docker)

### 🎁 Bonus débloqué
**🎲 +1 dé** : L'équipe peut lancer **2 dés** au lieu d'1 pour valider les critères d'acceptation

---

## `[CI/CD]` - Intégration Continue / Déploiement Continu

### User Stories techniques associées
- Pipeline CI/CD fonctionnel
- Déploiement automatisé en staging
- Déploiement automatisé en production
- Rollback automatique en cas d'erreur
- Build automatique sur commit

### 🎁 Bonus débloqué
**🔒 Critères permanents** : Les critères marqués `[CI/CD]` une fois validés ne doivent **plus être rejoués** dans les sprints suivants

---

## `[DEVOPS]` - DevOps & Automatisation

### User Stories techniques associées
- Infrastructure as Code (Terraform, Ansible)
- Monitoring et alerting (Prometheus, Grafana)
- Logs centralisés (ELK, Loki)
- Gestion des secrets (Vault)
- Auto-scaling

### 🎁 Bonus débloqué
**🔄 Relance** : L'équipe peut **relancer 1 dé** par sprint (choisir quel dé relancer)

---

## `[TESTS]` - Qualité des tests

### User Stories techniques associées
- Tests unitaires exécutés en < 3 minutes
- Couverture de tests > 80%
- Tests d'intégration automatisés
- Tests end-to-end (E2E)
- Mutation testing

### 🎁 Bonus débloqué
**🔒 Critères permanents** : Les critères marqués `[TESTS]` une fois validés ne doivent **plus être rejoués** dans les sprints suivants

---

## `[ARCHI]` - Architecture & Design

### User Stories techniques associées
- Documentation architecture à jour (C4, ADR)
- Code review systématique (obligatoire)
- Refactoring de la dette technique
- Design patterns documentés
- Diagrammes UML/Architecture

### 🎁 Bonus débloqué
**🔒 Critères permanents** : Les critères marqués `[ARCHI]` une fois validés ne doivent **plus être rejoués** dans les sprints suivants

---

## `[PERF]` - Performance

### User Stories techniques associées
- Temps de réponse API < 200ms
- Optimisation des requêtes BDD
- Cache distribué (Redis)
- Profiling de performance
- Load testing automatisé

### 🎁 Bonus débloqué
**⏱️ Temps supplémentaire** : L'équipe gagne **+30 secondes** de temps de jeu par sprint

---

## `[SECU]` - Sécurité

### User Stories techniques associées
- Scan de vulnérabilités automatisé
- Authentification/Autorisation robuste
- Chiffrement des données sensibles
- HTTPS obligatoire
- Protection CSRF/XSS

### 🎁 Bonus débloqué
**🔒 Critères permanents** : Les critères marqués `[SECU]` une fois validés ne doivent **plus être rejoués** dans les sprints suivants

---

## Règles d'application des bonus

1. **Cumul des bonus** : Les bonus de différentes catégories se cumulent
2. **Activation** : Un bonus s'active dès qu'une US technique de la catégorie est **complètement terminée** (tous ses critères validés)
3. **Permanence** : Les bonus restent actifs pour tous les sprints suivants
4. **Ordre d'acquisition** : Il est stratégique de prioriser `[INFRA_TEST]` pour obtenir le 2ème dé rapidement

---

## Exemple d'évolution d'une équipe

**Sprint 1** : Pas de bonus
→ 1 dé, critères à rejouer à chaque fois

**Sprint 2** : US "Base de données de test" `[INFRA_TEST]` terminée
→ 2 dés, critères toujours à rejouer

**Sprint 3** : US "Pipeline CI/CD" `[CI/CD]` terminée
→ 2 dés + critères `[CI/CD]` permanents

**Sprint 4** : US "Monitoring" `[DEVOPS]` terminée
→ 2 dés + critères `[CI/CD]` permanents + 1 relance par sprint