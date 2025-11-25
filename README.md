# Widget Dureté de l'Eau Luxembourg

**© 2025 Aqua Purify - Tous droits réservés**

Ce widget est développé et maintenu par **Aqua Purify**.
Il permet de consulter la dureté de l'eau par commune au Luxembourg.

## 📁 Fichiers disponibles

### 1. `index.html` - Version simple
Widget basique qui charge les données depuis l'API publique de data.public.lu et affiche :
- Filtre alphabétique pour sélectionner les communes
- Menu déroulant avec les communes
- Affichage de la dureté et des recommandations

### 2. `widget-durete-eau.html` - Version complète
Widget autonome avec des fonctionnalités avancées :
- Design moderne et responsive
- Barre de recherche avec auto-complétion
- Filtre alphabétique
- Affichage visuel avec codes couleur selon la dureté
- Chargement dynamique depuis l'API

## 🔌 Source des données

Les données proviennent de **data.public.lu** - Administration de la gestion de l'eau :
- **URL de l'API** : https://download.data.public.lu/resources/durete-de-leau/20251111-020330/wasserharte.geojson
- **Format** : GeoJSON
- **Licence** : Creative Commons Zero (CC0)
- **Dernière mise à jour** : 11 novembre 2025

## 📊 Catégories de dureté

| Dureté (°f) | Catégorie | Recommandation |
|-------------|-----------|----------------|
| < 8 | Eau douce | Adoucisseur optionnel |
| 8 - 16 | Eau modérément dure | Adoucisseur recommandé |
| 16 - 32 | Eau dure | Adoucisseur fortement recommandé |
| > 32 | Eau très dure | Adoucisseur indispensable |

**Note :** Pour la ville de Luxembourg, en raison de plusieurs réseaux de distribution différents, le widget renvoie vers le site officiel de la Ville de Luxembourg pour vérifier la qualité de l'eau selon l'adresse spécifique.

## 🚀 Utilisation

### Intégration dans votre site

#### Option 1 : Utiliser le widget complet (recommandé)
```html
<iframe
    src="widget-durete-eau.html"
    style="width: 100%; height: 600px; border: none;"
    title="Widget Dureté de l'Eau">
</iframe>
```

#### Option 2 : Intégrer le code directement
Copiez le contenu de `index.html` et intégrez-le dans votre page.

### Ouvrir directement
Vous pouvez simplement ouvrir les fichiers HTML dans votre navigateur :
- Double-cliquez sur `widget-durete-eau.html` pour la version complète
- Double-cliquez sur `index.html` pour la version simple

## 🛠️ Fonctionnalités

### Version complète (`widget-durete-eau.html`)
- ✅ Recherche en temps réel avec suggestions
- ✅ Filtre alphabétique interactif
- ✅ Affichage avec codes couleur
- ✅ Design moderne et responsive
- ✅ Gestion des erreurs de chargement
- ✅ Message de chargement

### Version simple (`index.html`)
- ✅ Filtre alphabétique
- ✅ Sélection par menu déroulant
- ✅ Affichage simple et clair
- ✅ Léger et rapide

## 🌐 Compatibilité

Les widgets fonctionnent sur tous les navigateurs modernes :
- Chrome / Edge (version 90+)
- Firefox (version 88+)
- Safari (version 14+)
- Opera (version 76+)

**Note** : Une connexion internet est requise pour charger les données depuis l'API.

## 📝 Structure des données

Les données GeoJSON contiennent pour chaque zone :
```json
{
  "properties": {
    "trinkwasser.GISADMIN.DWDnationalReportingDurete.Commune": "Luxembourg",
    "trinkwasser.GISADMIN.DWDnationalReportingDurete.WSZDurete": 27.5
  }
}
```

- `Commune` : Nom de la commune
- `WSZDurete` : Dureté de l'eau en degrés français (°f)

## 🔄 Mise à jour des données

Les données sont chargées directement depuis l'API publique à chaque chargement de page, garantissant que vous avez toujours les informations les plus récentes.

Pour mettre à jour l'URL de l'API si elle change, modifiez la constante `API_URL` dans le code JavaScript.

## 📄 Licence

Ce widget utilise des données publiques sous licence CC0 (Creative Commons Zero).
Le code du widget est libre d'utilisation.

## 🆘 Support

Pour toute question concernant les données, consultez :
- https://data.public.lu/fr/datasets/durete-de-leau/
- Administration de la gestion de l'eau du Luxembourg
