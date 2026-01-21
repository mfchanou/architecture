# 📋 Index des Décisions d'Architecture

## Structure des dossiers

```
/decisions
├── evaluations/           # Comparaisons d'outils
│   ├── eval-gitops.md
│   ├── eval-cni.md
│   └── ...
├── adrs/                  # Décisions finales
│   ├── ADR-001-gitops.md
│   ├── ADR-002-cni.md
│   └── ...
└── adr-index.md           # Ce fichier
```

---

## Comment utiliser

### Nouvelle décision à prendre ?

1. **Créer l'évaluation** → `evaluations/eval-[sujet].md` (utilise `tool-evaluation-template-v3.md`)
2. **Remplir et comparer** les options
3. **Décider**
4. **Créer l'ADR** → `adrs/ADR-XXX-[sujet].md` (utilise `adr-template-v2.md`)
5. **Mettre à jour cet index**

### Décision rapide (pas besoin d'évaluation formelle) ?

1. **Créer l'ADR** directement
2. **Documenter le raisonnement** même si court
3. **Mettre à jour cet index**

---

## Évaluations en cours

| Sujet | Fichier | Options comparées | Statut | Date |
|-------|---------|-------------------|--------|------|
| GitOps | `eval-gitops.md` | Argo CD, Flux, Fleet | 🟡 En cours | 2026-01-XX |
| CNI | `eval-cni.md` | Cilium, Calico | ⬜ À faire | |
| Secrets | `eval-secrets.md` | SOPS, Sealed Secrets, Vault | ⬜ À faire | |
| Policies | `eval-policies.md` | Kyverno, OPA/Gatekeeper | ⬜ À faire | |
| Cluster provisioning | `eval-cluster-provisioning.md` | Crossplane, Cluster API | ⬜ À faire | |
| Monitoring | `eval-monitoring.md` | Prometheus, Victoria Metrics | ⬜ À faire | |
| Ingress | `eval-ingress.md` | Nginx, Traefik, Contour | ⬜ À faire | |
| Backup | `eval-backup.md` | Velero, autres | ⬜ À faire | |

---

## ADRs - Décisions acceptées

| ID | Titre | Date | Évaluation | Lien |
|----|-------|------|------------|------|
| ADR-001 | GitOps : Argo CD | 2026-XX-XX | `eval-gitops.md` | [lien](adrs/ADR-001-gitops.md) |

---

## ADRs - Décisions en cours de validation

| ID | Titre | Statut | Date | Lien |
|----|-------|--------|------|------|
| - | - | - | - | - |

---

## ADRs - Décisions rejetées

| ID | Titre | Raison | Date | Lien |
|----|-------|--------|------|------|
| - | - | - | - | - |

---

## ADRs - Décisions supersédées

| ID | Titre | Supersédé par | Date | Lien |
|----|-------|---------------|------|------|
| - | - | - | - | - |

---

## Quick Log

Pour noter rapidement une décision (5 min) avant de faire l'ADR formel :

```markdown
### YYYY-MM-DD - [Titre]
- **Problème:** ...
- **Options:** A, B, C
- **Choix:** X parce que ...
- **Qui convaincu:** ...
- **TODO:** ⬜ Évaluation formelle | ⬜ ADR complet
```

---

### 2026-01-XX - GitOps tool
- **Problème:** Besoin d'un outil GitOps pour la plateforme
- **Options:** Argo CD, Flux, Fleet
- **Choix:** En cours d'évaluation
- **TODO:** 🟡 Évaluation formelle | ⬜ ADR complet

---

## Statistiques

| Métrique | Valeur |
|----------|--------|
| Total évaluations | 1 |
| Total ADRs | 0 |
| Acceptées | 0 |
| Rejetées | 0 |
| En cours | 1 |

---

## Prochaines décisions à prendre

| Priorité | Sujet | Pourquoi maintenant |
|----------|-------|---------------------|
| 🔴 Haute | GitOps | Besoin pour déployer tout le reste |
| 🔴 Haute | Cluster local | Besoin d'un cluster pour commencer |
| 🟠 Moyenne | CNI | Après le cluster |
| 🟠 Moyenne | Secrets | Avant de déployer des apps |
| 🟡 Basse | Monitoring | Peut venir après |

---

## Templates disponibles

| Template | Usage | Fichier |
|----------|-------|---------|
| Évaluation complète | Comparer des outils (~1-2h) | `tool-evaluation-template-v3.md` |
| Évaluation rapide | Décision rapide (~30min) | `tool-evaluation-quick-v3.md` |
| ADR | Documenter une décision | `adr-template-v2.md` |

---

## Tags fréquents

`#gitops` `#networking` `#cni` `#security` `#secrets` `#monitoring` `#observability` `#storage` `#backup` `#policies` `#ingress` `#cluster-management`
