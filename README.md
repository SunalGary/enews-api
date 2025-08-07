# E-News API - Guide d'utilisation

## 🚀 Déploiement sur Vercel

### Étape 1 : Créer un repository GitHub
1. Allez sur [github.com](https://github.com)
2. Cliquez "New repository"
3. Nommez-le `enews-api`
4. Cliquez "Create repository"

### Étape 2 : Uploader les fichiers
1. Dans votre nouveau repository, cliquez "uploading an existing file"
2. Glissez-déposez ces fichiers :
   - `articles.json`
   - `api/articles.js`
   - `vercel.json`
   - `README.md`
3. Cliquez "Commit changes"

### Étape 3 : Déployer sur Vercel
1. Allez sur [vercel.com](https://vercel.com)
2. Cliquez "New Project"
3. Importez votre repository `enews-api`
4. Cliquez "Deploy"

### Étape 4 : Récupérer l'URL
- Vercel vous donnera une URL comme : `https://enews-api-xxx.vercel.app`
- Votre API sera accessible à : `https://enews-api-xxx.vercel.app/api/articles`

## 📝 Modifier les articles

### Pour ajouter/modifier des articles :
1. Allez dans votre repository GitHub
2. Cliquez sur `articles.json`
3. Cliquez l'icône crayon (Edit)
4. Modifiez le contenu
5. Cliquez "Commit changes"
6. **Vercel déploie automatiquement !**

### Structure d'un article :
```json
{
  "title": "🚀 Titre avec emoji",
  "summary": "Description de l'article",
  "url": "https://votre-lien.com",
  "category": "tech"
}
```

## 🔧 Utilisation dans l'extension

L'URL de votre API sera utilisée dans `background.js` :
```javascript
const API_URL = 'https://votre-api.vercel.app/api/articles';
```

## ✅ Test

Testez votre API en visitant : `https://votre-api.vercel.app/api/articles`

Vous devriez voir le JSON avec tous vos articles ! 