# 📌 Instructions pour intégrer le widget (Embed Code)

## Méthode simple : Copier-Coller

Pour intégrer le widget de dureté de l'eau sur votre site web, suivez ces étapes :

### 1️⃣ Ouvrez le fichier `embed-code.html`

Ce fichier contient le code complet à copier.

### 2️⃣ Copiez TOUT le contenu du fichier

Sélectionnez tout le contenu de `embed-code.html` (de la première ligne à la dernière).

### 3️⃣ Collez le code sur votre page

Collez le code complet à l'endroit où vous voulez que le widget apparaisse sur votre site.

**Exemple d'intégration :**

```html
<!DOCTYPE html>
<html>
<head>
    <title>Mon Site</title>
</head>
<body>
    <h1>Bienvenue</h1>
    <p>Consultez la dureté de l'eau de votre commune :</p>

    <!-- COLLEZ LE CODE EMBED ICI -->
    <div id="widget-durete-eau-container">
        ... (tout le code du widget) ...
    </div>
    <!-- FIN DU CODE EMBED -->

    <p>Autres contenus de votre page...</p>
</body>
</html>
```

## ✅ Avantages du code embed

- ✅ **Aucun fichier externe nécessaire** : Tout est inclus (HTML, CSS, JavaScript)
- ✅ **Fonctionne immédiatement** : Pas de configuration requise
- ✅ **Données en temps réel** : Se connecte automatiquement à l'API data.public.lu
- ✅ **Responsive** : S'adapte à tous les écrans
- ✅ **Autonome** : Ne perturbe pas le reste de votre site

## 🔧 Personnalisation

### Modifier la largeur maximale

Par défaut, le widget a une largeur maximale de 700px. Pour la modifier :

```css
#widget-durete-eau-container {
  max-width: 900px; /* Changez cette valeur */
  margin: 0 auto;
}
```

### Modifier les couleurs

Recherchez `#0D7EBC` dans le code et remplacez-le par votre couleur principale.

### Modifier le titre

Recherchez `<h2 class="wde-title">Dureté de l'Eau par Commune</h2>` et changez le texte.

## 🌐 Compatibilité

Le widget fonctionne sur tous les navigateurs modernes :
- Chrome / Edge (90+)
- Firefox (88+)
- Safari (14+)
- Opera (76+)

**Important :** Une connexion internet est requise pour charger les données depuis l'API.

## 🚨 Dépannage

### Le widget ne s'affiche pas
1. Vérifiez que vous avez bien copié TOUT le code
2. Assurez-vous qu'il n'y a pas de conflits de CSS avec votre site
3. Vérifiez la console du navigateur (F12) pour les erreurs

### "Erreur de chargement des données"
1. Vérifiez votre connexion internet
2. L'API data.public.lu peut être temporairement indisponible
3. Vérifiez que l'URL de l'API est toujours valide

### Conflits de style avec votre site
Toutes les classes CSS du widget commencent par `wde-` pour éviter les conflits. Si vous avez quand même des problèmes, vous pouvez ajouter `!important` aux styles du widget.

## 📞 Support

Pour toute question sur les données :
- https://data.public.lu/fr/datasets/durete-de-leau/
