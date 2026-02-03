# Contribuer au Projet BTS

Merci de votre intérêt pour **ce projet**.
Les contributions sont les bienvenues, qu’il s’agisse de corrections de bugs, d’améliorations, de nouveaux templates ou de documentation.

Ce document décrit les règles et bonnes pratiques pour contribuer au projet.

---

## Prérequis

* Python **≥ 3.10**
* `pip`
* Un environnement Linux, macOS ou Windows
* Connaissances de base en Python et Git

---

## Installation pour le développement

1. Forker le dépôt sur GitHub
2. Cloner le fork localement :

```bash
git clone https://github.com/boudjelaba/projet_bts_ciel.git
cd projet_bts
```

---

## Bonnes pratiques de code

* Python clair et lisible
* Fonctions courtes et bien nommées
* Commentaires utiles (pas redondants)
* Pas de dépendances inutiles
* Compatibilité Linux / macOS / Windows

---

## Soumettre une contribution

1. Créer une branche à partir de `main` :

```bash
git checkout -b feature/ma-fonctionnalite
```

2. Faire vos modifications
3. Vérifier que tout fonctionne
4. Commit avec un message clair :

```bash
git commit -m "feat: Ajout du template xyz"
```

5. Push la branche et ouvrir une **Pull Request**

### Format recommandé

```
[BTS-XX] <type> : <description courte>
```

### Exemples

```
[BTS-01] feature : analyse des logs
[BTS-02] bug : erreur de comptage des ERROR
[BTS-03] docs : compléter le README
[BTS-04] ci : ajouter semantic-release
[BTS-05] test : tests unitaires ping_check
```

### Mapping type → semantic-release

| Type issue | Label         | Commit   |
| ---------- | ------------- | -------- |
| feature    | type: feature | `feat:`  |
| bug        | type: bug     | `fix:`   |
| docs       | type: docs    | `docs:`  |
| ci         | type: chore   | `chore:` |
| test       | type: chore   | `chore:` |

---

## Types de contributions appréciées

* Corrections de bugs
* Amélioration de la documentation
* Simplification ou refactorisation du code
* Suggestions d’amélioration (via issues)

---

## Style des commits (Conventional Commits)

Les messages de commit doivent respecter la forme :

<type>: <description courte>

**Exemples :**

- `feat: ajouter un nouveau test sur ping_check`
- `fix: corriger l'affichage des logs`
- `docs: compléter le README`
- `chore: mettre à jour .gitignore`
- `ci: modifier le workflow GitHub`

### Types standards

| Type               | Impact    |
| ------------------ | --------- |
| `feat:`            | minor     |
| `fix:`             | patch     |
| `perf:`            | patch     |
| `refactor:`        | patch     |
| `docs:`            | aucun     |
| `test:`            | aucun     |
| `chore:`           | aucun     |
| `feat!:`           | **major** |
| `BREAKING CHANGE:` | **major** |

Exemple valide :

```text
feat(cli): ajout de l'option --dry-run
```

Une issue est considérée comme terminée si :
- [ ] code fonctionnel
- [ ] tests passent
- [ ] CI verte
- [ ] documentation mise à jour si nécessaire

---

### Changements cassants

Pour une rupture de compatibilité :

```text
feat!: refonte du projet
````

ou

```text
feat: refonte du projet

BREAKING CHANGE: changement de structure
```

---

## Intégration continue

Chaque Pull Request déclenche automatiquement :

* Les tests
* La validation du CHANGELOG
* La vérification du format des commits

Une PR ne respectant pas ces règles ne pourra pas être mergée.

---

## Signaler un bug ou proposer une idée

* Ouvrir une **issue GitHub**
* Décrire :

  * ce que vous faites
  * ce que vous attendez
  * ce qui se passe réellement
  * votre OS et la version de Python

---

## Code de conduite

Soyez pros.

---

Merci pour vos contributions.
Chaque amélioration aide à rendre **pygen** plus utile et plus robuste.

---

