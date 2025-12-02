# 🤝 Guide de Contribution

Merci de vouloir contribuer à ce projet ! 💜

Ce guide vous explique comment proposer de nouvelles ressources ou améliorer celles existantes.

## Table des matières

- [Types de contributions](#types-de-contributions)
- [Comment ajouter une ressource](#comment-ajouter-une-ressource)
- [Critères de qualité](#critères-de-qualité)
- [Process de review](#process-de-review)
- [Style et formatage](#style-et-formatage)

## Types de contributions

### Ajouter une nouvelle ressource

Vous connaissez une ressource de qualité qui manque ? Proposez-la !

### Mettre à jour une ressource existante

- Corriger un lien mort
- Mettre à jour une description
- Corriger une erreur

### Suggérer une amélioration

- Proposer une nouvelle catégorie
- Améliorer l'organisation
- Traduire le contenu

### Signaler un problème

- Lien mort
- Information obsolète
- Erreur de formatage

## Comment ajouter une ressource

### 1. Fork le repo

Cliquez sur le bouton "Fork" en haut à droite de la page GitHub.

### 2. Clone votre fork

```bash
git clone https://github.com/VOTRE-USERNAME/ressources-ml.git
cd ressources-ml
```

### 3. Configurez le repo upstream (optionnel mais recommandé)

Pour garder votre fork synchronisé avec le repo original :

```bash
# Ajoutez le repo original comme "upstream"
git remote add upstream https://github.com/benjamin-svg/ressources-ml.git

# Vérifiez que c'est bien configuré
git remote -v
```

**Pour synchroniser votre fork avant de contribuer :**

```bash
# Récupérez les dernières modifications du repo original
git fetch upstream

# Mettez à jour votre branche main
git checkout main
git merge upstream/main

# Poussez les mises à jour sur votre fork
git push origin main
```

> 💡 **Conseil** : Faites toujours un `git fetch upstream` avant de créer une nouvelle branche pour éviter les conflits.

### 4. Créez une branche

```bash
git checkout -b add/nom-de-la-ressource
```

**Convention de nommage des branches :**
- `add/nom-ressource` - Pour ajouter une ressource
- `fix/description-du-fix` - Pour corriger quelque chose
- `update/nom-ressource` - Pour mettre à jour une ressource

### 5. Ajoutez votre ressource

Éditez le fichier `RESSOURCES.md` en suivant le format existant :

```markdown
| [Nom de la ressource](URL) | Type | Description courte et pertinente. |
```

**Types acceptés :**
- `Vidéo` - Cours vidéo, tutoriels YouTube
- `Livre` - Livres (gratuits ou payants)
- `MOOC` - Cours en ligne structurés
- `Interactif` - Plateformes avec exercices
- `Blog` - Articles de blog
- `Doc` - Documentation officielle
- `Podcast` - Podcasts audio/vidéo
- `Tuto` - Tutoriels écrits
- `Paper` - Articles de recherche
- `Pratique` - Exercices, projets pratiques
- `Framework` / `Lib` - Outils et bibliothèques

### 6. Committez vos changements

```bash
git add RESSOURCES.md
git commit -m "Add: Nom de la ressource (Catégorie)"
```

**Format des commits :**
- `add: Nom ressource (Catégorie)`
- `fix: Description du fix`
- `update: Nom ressource`
- `remove: Nom ressource`

### 7. Push et créez une Pull Request

```bash
git push origin add/nom-de-la-ressource
```

Puis créez une Pull Request sur GitHub en utilisant le template fourni.

## Critères de qualité

Avant de soumettre une ressource, vérifiez qu'elle répond à ces critères :

### Obligatoire

- [ ] **Pertinente** : La ressource est liée au ML/AI
- [ ] **Accessible** : Le lien fonctionne
- [ ] **Qualité** : Le contenu est pédagogique et bien fait
- [ ] **Pas de doublon** : La ressource n'est pas déjà listée

### Bonus

- [ ] **Gratuite** ou avec une version gratuite substantielle
- [ ] **À jour** : Le contenu n'est pas obsolète
- [ ] **Reconnue** : La ressource est recommandée par la communauté
- [ ] **Francophone** : Les ressources en français sont bienvenues (ajoutez 🇫🇷)

### ❌ Ce qu'on n'accepte pas

- Ressources promotionnelles ou spam
- Contenus de faible qualité
- Ressources entièrement payantes sans version gratuite
- Liens vers des contenus piratés
- Contenus offensants ou discriminatoires

## 🔍 Process de review

1. **Vérification automatique** : Le lien fonctionne-t-il ?
2. **Review par un mainteneur** : La ressource répond-elle aux critères ?
3. **Feedback** : Si besoin, on vous demandera des modifications
4. **Merge** : Une fois validée, votre PR sera mergée ! 🎉

## Style et formatage

### Format d'une entrée

```markdown
| [Nom officiel de la ressource](https://url-complete.com) | Type | Description en une phrase. |
```

### Bonnes pratiques

- **Nom** : Utilisez le nom officiel de la ressource
- **URL** : Lien direct vers la ressource (pas de raccourcisseurs)
- **Type** : Un seul type parmi la liste ci-dessus
- **Description** : 
  - Maximum 2 phrases
  - Commencez par un verbe ou un qualificatif
  - Évitez "Très bien", "Super", préférez des descriptions factuelles
  - Indiquez le niveau si pertinent (débutant, avancé, etc.)

### Exemples

✅ **Bon** :
```markdown
| [Fast.ai](https://course.fast.ai/) | MOOC | Approche top-down pragmatique. Idéal pour coder rapidement avant de comprendre la théorie. |
```

❌ **Moins bon** :
```markdown
| [fastai course](https://course.fast.ai/) | Cours | C'est vraiment un super cours que j'ai adoré !! |
```

## Besoin d'aide ?

- Ouvrez une [issue](../../issues/new) pour poser une question
- Rejoignez les [discussions](../../discussions) pour échanger

---

Merci pour votre contribution ! 🙏
