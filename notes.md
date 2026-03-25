# Mes notes - Lab Git 1

## Ce que j'ai appris

### 1. Configurer Git
Avant tout, dire à Git qui on est :
```
git config --global user.name "Serigne Mbaye Thioub"
git config --global user.email "serignembayethioub@esp.sn"
```

### 2. Les 3 zones de Git
- **Répertoire de travail** : mes fichiers sur mon PC
- **Zone de préparation (Staging)** : les fichiers prêts à être sauvegardés (git add)
- **Dépôt local (.git)** : l'historique de tous mes commits (git commit)

### 3. Les commandes de base

| Commande | Ce qu'elle fait |
|---|---|
| `git init` | Crée un nouveau dépôt Git |
| `git status` | Montre l'état des fichiers |
| `git add .` | Prépare tous les fichiers modifiés |
| `git commit -m "message"` | Sauvegarde les changements |
| `git log --oneline` | Affiche l'historique des commits |

### 4. Connecter à GitHub
```
git remote add origin https://github.com/USERNAME/REPO.git
git branch -M main
git push -u origin main
```

### 5. Le cycle complet (à retenir !)
```
modifier fichier → git add . → git commit -m "message" → git push
```

### 6. Ce que j'ai retenu
- `git add` = mettre le fichier dans l'enveloppe
- `git commit` = envoyer l'enveloppe
- `git push` = envoyer sur GitHub
- Ne jamais supprimer le dossier `.git`
- Toujours écrire un message de commit clair

### 7. Erreurs rencontrées et solutions
- **Warning LF/CRLF** : pas grave, juste Windows qui gère les fins de ligne
- **error: src refspec main** : ma branche s'appelait `master` pas `main` → j'ai utilisé `git branch -M main`
- **Typo dans un message de commit** : corrigé avec `git commit --amend -m "nouveau message"`
