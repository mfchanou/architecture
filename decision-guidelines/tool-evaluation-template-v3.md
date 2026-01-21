# Template d'Évaluation d'Outils

## Comment utiliser ce template

1. **Copie ce fichier** pour chaque décision (ex: `eval-gitops.md`)
2. **Remplis la section "Contexte"**
3. **Évalue chaque option** avec le même template
4. **Compare** dans le tableau de synthèse
5. **Décide** et documente pourquoi
6. **Crée l'ADR** à partir de cette évaluation

---

## Sources d'information par critère

| Critère | Où chercher |
|---------|-------------|
| Répond au besoin | Doc officielle (features), GitHub README |
| Maturité / CNCF Status | landscape.cncf.io |
| GitHub Stats | GitHub repo (stars, contributors, releases, issues) |
| Adoption / Qui l'utilise | Page "Adopters" sur site officiel, CNCF case studies |
| Learning curve | Doc (getting started), YouTube tutos, faire le quickstart |
| Coût | Site officiel (pricing), GitHub (licence) |
| Scalabilité / Limites | GitHub issues ("scale", "performance"), blog posts |
| Intégration | Doc (integrations), GitHub examples |
| Opérabilité | Doc (troubleshooting, upgrade), GitHub issues |
| Sécurité | GitHub Security tab, CVE databases |
| Réversibilité | Google "migrate from X to Y" |
| Red flags | GitHub activité, issues non répondues, CNCF Slack |
| Retours d'XP | Blog posts, Reddit r/kubernetes, CNCF Slack, KubeCon talks |

### Sources clés

| Source | URL | Ce que tu trouves |
|--------|-----|-------------------|
| CNCF Landscape | https://landscape.cncf.io | Status CNCF, catégorie, alternatives |
| CNCF Radar | https://radar.cncf.io | Ce que les entreprises utilisent vraiment |
| GitHub | https://github.com/[projet] | Stats, activité, issues, roadmap |
| Reddit | https://reddit.com/r/kubernetes | Retours honnêtes, problèmes |
| CNCF Slack | https://slack.cncf.io | Questions directes aux maintainers |
| YouTube | KubeCon talks | Deep dives, retours d'XP |

---

# Évaluation : [Nom de la décision]

**Date :** YYYY-MM-DD  
**Décideur :** [Ton nom]  
**Deadline de décision :** YYYY-MM-DD  
**Temps investi :** Xh

---

## 1. Contexte

### Quel problème je résous ?
[Décris en 2-3 phrases]

### Contraintes
- Budget : 
- Temps dispo :
- Stack existante :
- Compétences équipe :

### Critères de succès
Comment je sais que j'ai fait le bon choix dans 6 mois ?
- [ ] Critère 1
- [ ] Critère 2
- [ ] Critère 3

---

## 2. Options identifiées

| Option | Description courte |
|--------|-------------------|
| A. [Nom] | ... |
| B. [Nom] | ... |
| C. [Nom] | ... |
| D. Ne rien faire | Toujours une option |

---

## 3. Évaluation détaillée

### Option A : [Nom]

#### Fiche d'identité

> **Où chercher :** Site officiel, GitHub repo

| Attribut | Valeur |
|----------|--------|
| Site | |
| GitHub | |
| Licence | |
| CNCF Status | Graduated / Incubating / Sandbox / Non |
| Version actuelle | |
| Dernière release | |

---

#### Besoin

> **Questions :** Ça répond à mon problème ? Quels features manquent ?
> 
> **Où chercher :** Doc officielle (features list), GitHub README

- [ ] ✅ Oui totalement
- [ ] ⚠️ Partiellement
- [ ] ❌ Non

**Features qui matchent :**
- 

**Features manquantes :**
- 

---

#### Maturité

> **Questions :** C'est stable ? En prod où ? CNCF Graduated/Incubating ?
> 
> **Où chercher :** landscape.cncf.io, GitHub releases, CNCF case studies

| Indicateur | Valeur |
|------------|--------|
| CNCF Status | |
| Version stable depuis | |
| Breaking changes récents ? | Oui / Non |
| En prod chez | |

---

#### Communauté

> **Questions :** Actif ? Contributors ? GitHub stars/issues ? Slack actif ?
> 
> **Où chercher :** GitHub repo, CNCF Slack

| Indicateur | Valeur |
|------------|--------|
| GitHub Stars | |
| Contributors | |
| Open Issues | |
| Issues fermées (30 derniers jours) | |
| Slack/Discord actif ? | |
| Dernière release | |

---

#### Adoption

> **Questions :** Qui l'utilise en prod ? Des entreprises similaires à moi ?
> 
> **Où chercher :** Page "Adopters" du site officiel, CNCF case studies, blog posts

| Indicateur | Valeur |
|------------|--------|
| Entreprises connues | |
| Entreprises similaires à moi | |
| Case studies dispos | |

---

#### Learning Curve

> **Questions :** Temps pour être productif ? Doc de qualité ?
> 
> **Où chercher :** Doc (getting started), YouTube, essayer le quickstart toi-même

| Indicateur | Valeur |
|------------|--------|
| Time to "Hello World" | |
| Qualité doc | ⭐⭐⭐⭐⭐ |
| Tutos disponibles | |
| Je connais déjà ? | Oui / Non |

---

#### Coût

> **Questions :** Open source ? Licence ? Coût opérationnel (ressources, maintenance) ?
> 
> **Où chercher :** Site officiel (pricing), GitHub (fichier LICENSE)

| Type | Estimation |
|------|------------|
| Licence | Gratuit / Payant (€X/mois) |
| Ressources (CPU/RAM) | |
| Temps de maintenance estimé | |
| Coût total estimé | |

---

#### Scalabilité

> **Questions :** Tient la charge ? Limites connues ?
> 
> **Où chercher :** GitHub issues (cherche "scale", "performance", "limit"), blog posts retours d'XP

| Question | Réponse |
|----------|---------|
| Limites connues ? | |
| Tient la charge pour mon use case ? | |
| Utilisé à grande échelle par ? | |

---

#### Intégration

> **Questions :** S'intègre avec ma stack existante ?
> 
> **Où chercher :** Doc officielle (integrations), GitHub examples/

| Composant de ma stack | Compatible ? | Notes |
|-----------------------|--------------|-------|
| | Oui / Non / Partiel | |
| | Oui / Non / Partiel | |
| | Oui / Non / Partiel | |

---

#### Support

> **Questions :** Commercial dispo ? Communauté réactive ?
> 
> **Où chercher :** Site officiel, GitHub issues response time, Slack

| Type | Disponible ? | Détails |
|------|--------------|---------|
| Support commercial | Oui / Non | |
| Support communautaire | Oui / Non | |
| Temps de réponse moyen (issues) | | |

---

#### Réversibilité

> **Questions :** Je peux changer si ça marche pas ? Lock-in ?
> 
> **Où chercher :** Google "migrate from X to Y", ton jugement

| Critère | Évaluation |
|---------|------------|
| Lock-in | Faible / Moyen / Fort |
| Migration possible vers | |
| Effort de migration | |
| Standards ouverts utilisés ? | |

---

#### Sécurité

> **Questions :** CVEs ? Audit ? Maintenu activement ?
> 
> **Où chercher :** GitHub Security tab, CVE databases, doc (security section)

| Critère | Évaluation |
|---------|------------|
| CVEs récentes critiques ? | |
| Audit de sécu ? | |
| Activement maintenu ? | |
| Security policy ? | |

---

#### Opérabilité

> **Questions :** Facile à debug ? Observabilité ? Upgrade path ?
> 
> **Où chercher :** Doc (troubleshooting, upgrade guide), GitHub issues

| Critère | Évaluation |
|---------|------------|
| Facile à debug ? | |
| Observabilité native (metrics, logs) ? | |
| Upgrade path clair ? | |
| Backup/Restore ? | |
| Rollback possible ? | |

---

#### Red Flags 🚩

> **Où chercher :** GitHub (activité commits, issues non répondues), CNCF Slack

- [ ] Projet dormant (pas de commit depuis 6 mois)
- [ ] Peu de contributors (bus factor)
- [ ] Breaking changes fréquents
- [ ] Pas de roadmap claire
- [ ] Company-driven sans communauté
- [ ] Issues ignorées
- [ ] Autre : 

---

#### Score global : X/10

**Forces :**
- 

**Faiblesses :**
- 

---

### Option B : [Nom]

*(Copie la même structure que Option A)*

---

### Option C : [Nom]

*(Copie la même structure que Option A)*

---

## 4. Tableau de synthèse

| Critère | Poids (1-5) | Option A | Option B | Option C |
|---------|-------------|----------|----------|----------|
| Besoin | 5 | /10 | /10 | /10 |
| Maturité | 3 | /10 | /10 | /10 |
| Communauté | 3 | /10 | /10 | /10 |
| Adoption | 2 | /10 | /10 | /10 |
| Learning curve | 4 | /10 | /10 | /10 |
| Coût | 3 | /10 | /10 | /10 |
| Scalabilité | 3 | /10 | /10 | /10 |
| Intégration | 4 | /10 | /10 | /10 |
| Support | 2 | /10 | /10 | /10 |
| Réversibilité | 2 | /10 | /10 | /10 |
| Sécurité | 3 | /10 | /10 | /10 |
| Opérabilité | 4 | /10 | /10 | /10 |
| **SCORE PONDÉRÉ** | | **X** | **X** | **X** |

---

## 5. Décision

### Je choisis : [Option X]

### Pourquoi ?
1. 
2. 
3. 

### Pourquoi pas les autres ?

**Option Y rejetée :**
- 

**Option Z rejetée :**
- 

### Trade-offs acceptés
- Je perds : 
- Je gagne : 

### Risques identifiés
| Risque | Probabilité | Mitigation |
|--------|-------------|------------|
| | | |

### Conditions de remise en question
Je reconsidère ce choix si :
- 
- 

---

## 6. Validation

### Sources consultées
- [ ] Doc officielle
- [ ] GitHub (issues, PRs, roadmap)
- [ ] Blog posts / Retours d'XP
- [ ] CNCF Landscape / Radar
- [ ] Reddit / HackerNews
- [ ] Slack communautaire
- [ ] Talk KubeCon
- [ ] Autre : 

### Personnes consultées
| Qui | Leur avis |
|-----|-----------|
| | |

---

## 7. Next Steps

- [ ] Créer l'ADR à partir de cette évaluation
- [ ] POC rapide pour valider
- [ ] Implémenter
- [ ] Review dans X semaines

---

## Historique

| Date | Action |
|------|--------|
| YYYY-MM-DD | Évaluation initiale |
| | |
