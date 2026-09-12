<div align="center">

# 🌞 Oracle Solaire

**🌞 Oracle Directionnel Solaire + Lunaire + Atlas Energetique + Simulateur PV ( Photovoltaique ) + PVGIS vs Modele ... 

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-4.0-blue.svg)](https://github.com/)
[![PWA](https://img.shields.io/badge/PWA-ready-success.svg)](https://web.dev/progressive-web-apps/)
[![Responsive](https://img.shields.io/badge/responsive-mobile%20%7C%20tablet%20%7C%20desktop-green.svg)]()

*44 capitales européennes · 24 communes de La Réunion · Soleil · Lune · Planètes · ISS · PVGIS*

[Fonctionnalités](#-fonctionnalités) · [Installation](#-installation) · [Utilisation](#-utilisation) · [Documentation](#-documentation) · [Licence](#-licence)

</div>

---

## 📖 Présentation

**Oracle Solaire** est une application web progressive (PWA) autonome qui calcule en temps réel la position du Soleil, de la Lune, des planètes et de la Station Spatiale Internationale (ISS). Elle fournit des éphémérides complètes, un simulateur photovoltaïque basé sur PVGIS 5.3, et un atlas d'ensoleillement pour **44 capitales européennes** et **24 communes de La Réunion**.

Aucune clé API requise. Aucun compte. Aucune dépendance serveur. Un seul fichier HTML.

---

## ✨ Fonctionnalités

### 🔮 Mode solo — Éphémérides complètes

- **Position du Soleil** en temps réel (azimut, hauteur, distance)
- **Position de la Lune** (azimut, hauteur, phase, illumination, distance)
- **Boussole solaire et lunaire** avec aiguille directionnelle
- **Éphémérides** : lever, coucher, midi solaire, heures dorées, crépuscules
- **Rose des vents** et projections polaires
- **Course du Soleil et de la Lune** sur 24h
- **Carte solaire** avec trajectoires comparées (solstices, équinoxes)
- **Mode Photographe** : heures idéales pour la photo de paysage
- **Mode AR** (Réalité Augmentée) avec gyroscope du téléphone

### 🌙 Module lunaire détaillé (9 visualisations)

1. Boussole lunaire avec aiguille directionnelle
2. Rose lunaire (azimut/heure)
3. Hauteur lunaire en projection polaire
4. Azimut Lune sur 24h (courbe linéaire)
5. Comparaison azimut Soleil / Lune
6. Rose comparée 16 secteurs
7. Quadrants célestes occupés
8. Tableau des positions horaires (24 lignes)
9. Conseil contextuel selon la phase

### 🪐 Astronomie

- **Planètes visibles** : Mercure, Vénus, Mars, Jupiter, Saturne
- **Pluies de météores** : Perséides, Géminides, Léonides, Quadrantides…
- **ISS** : distance, altitude, vitesse en temps réel
- **Solstices et équinoxes** avec horodatage précis

### 🔋 Simulateur photovoltaïque

- Calcul de production annuelle en kWh
- Ajustement automatique de l'orientation (Sud en Europe, Nord à La Réunion)
- Estimation du retour sur investissement (ROI)
- Calcul du CO₂ évité
- Graphique de production mensuelle

### 📊 Atlas d'ensoleillement

- Comparaison de 4 villes sur 12 mois
- Données **PVGIS 5.3** (Commission Européenne)
- Cumul mensuel ou moyenne quotidienne
- Thermomètre visuel heatmap
- Export PNG du graphique

### 🌍 Couverture géographique

| Région | Villes |
|--------|--------|
| 🇷🇪 **La Réunion** | 24 communes (Saint-Denis, Saint-Paul, Saint-Pierre…) |
| 🇫🇷 **Paris** | Capitale française |
| 🇪🇺 **Europe** | 44 capitales (Paris, Londres, Berlin, Madrid, Rome, Athènes, Oslo, Moscou…) |

### 🌐 Autres fonctionnalités

- **Météo live** (Open-Meteo) avec prévisions 7 jours
- **Calendrier culturel** : fêtes créoles et européennes
- **Export PDF** : éphémérides du jour + graphiques
- **Multilangue** : 🇫🇷 Français · 🇬🇧 English · 🇷🇪 Kréol
- **Favoris** : sauvegarde locale des villes préférées
- **Mode PWA** : installable sur mobile, fonctionne hors-ligne
- **Carte interactive 3D** : relief MapLibre
- **Responsive** : mobile, tablette, desktop

---

## 🎯 Points forts

| Caractéristique | Détail |
|-----------------|--------|
| **Aucune clé API** | Toutes les données sont open-source ou embarquées |
| **PWA offline** | Fonctionne sans connexion après premier chargement |
| **Un seul fichier** | Tout tient dans un seul `index.html` |
| **Responsive** | Barre mobile + hamburger + FAB |
| **PDF intégré** | Éphémérides exportables en un clic |
| **Multilingue** | FR / EN / CR |
| **Calculs précis** | SunCalc + Astronomy Engine |

---

## 📊 Mise à jour des données

Oracle Solaire combine des **calculs astronomiques locaux** (temps réel) et des **données externes** (météo, ISS).

### 🎯 Vue d'ensemble

| Donnée | Mise à jour auto ? | Fréquence | Source |
|--------|:------------------:|-----------|--------|
| ☀️ Position Soleil | ✅ Oui | Temps réel (si animation) | SunCalc (calcul local) |
| 🌙 Position Lune | ✅ Oui | Temps réel (si animation) | SunCalc (calcul local) |
| 🌙 Phase lunaire | ✅ Oui | À chaque refresh | SunCalc |
| 🌅 Heures lever/coucher Soleil | ✅ Oui | À chaque changement de date | SunCalc |
| 🌙 Heures lever/coucher Lune | ✅ Oui | À chaque changement de date | SunCalc |
| 🪐 Planètes | ✅ Oui | À chaque refresh | Astronomy Engine |
| 🌠 Pluies de météores | ✅ Oui | Recaculées selon la date | Formules embarquées |
| 📅 Solstices / Équinoxes | ✅ Oui | Selon l'année affichée | Astronomy Engine |
| 🌤️ Météo live | ✅ Oui | Au chargement + refresh | Open-Meteo |
| 🔮 Prévisions 7 jours | ✅ Oui | Au chargement | Open-Meteo |
| 🛰️ ISS | ✅ Oui | À chaque refresh | wheretheiss.at |
| 📅 Fêtes locales | ⚠️ Non | Dates figées en 2026 | Codées en dur |
| 📊 PVGIS (Atlas) | ⚠️ Non | Valeurs figées | Embarquées v19.0 |
| 📍 Sélection ville | Manuel | À chaque clic | — |
| 📅 Date / heure | Manuel ou ⏱️ | À chaque clic | — |

### ✅ Mise à jour automatique

À l'ouverture :

1. La date est mise à aujourd'hui
2. Toutes les positions astronomiques sont recalculées
3. La météo est rechargée depuis Open-Meteo
4. La position ISS est rechargée

### 🔄 Actualisation manuelle

Pour actualiser : bouton **⏱️ Maintenant**, **🔮 Consulter**, recharger la page (F5), ou lancer l'animation **▶️ Animer**.

### 🔧 Auto-refresh (optionnel)

Ajoutez à la fin de `DOMContentLoaded` :

```javascript
// Rafraîchir les positions toutes les 60 s
setInterval(() => {
  const today = new Date().toISOString().slice(0, 10);
  if ($("dateInput").value === today) {
    refreshAll();
  }
}, 60000);

// Rafraîchir la météo toutes les 10 min
setInterval(() => {
  if (currentMode === "solo") loadWeather(currentLocation);
}, 600000);

// Rafraîchir l'ISS toutes les 30 s
setInterval(() => {
  if (currentMode === "solo") renderISSPasses(currentLocation);
}, 30000);
```

---

## 🚀 Installation

### Option 1 — Utilisation directe

Clonez le dépôt et ouvrez le fichier HTML dans votre navigateur :

```bash
git clone https://github.com/votre-utilisateur/oracle-solaire.git
cd oracle-solaire
```

Puis ouvrez `index.html` dans votre navigateur.

### Option 2 — Serveur local

Pour bénéficier du mode PWA (service worker) et éviter les restrictions CORS :

```bash
# Avec Python 3
python -m http.server 8000

# Avec Node.js (npx)
npx serve

# Avec PHP
php -S localhost:8000
```

Puis ouvrez [http://localhost:8000](http://localhost:8000)

### Option 3 — Déploiement

Oracle Solaire est un fichier statique. Déployez-le sur :

- **GitHub Pages** (recommandé)
- **Netlify**
- **Vercel**
- **Cloudflare Pages**
- N'importe quel serveur HTTP

### Installation PWA (mobile)

1. Ouvrez Oracle Solaire dans **Safari** (iOS) ou **Chrome** (Android)
2. Appuyez sur **Partager** → **Ajouter à l'écran d'accueil**
3. L'application devient installable et fonctionne hors-ligne

---

## 💡 Utilisation

### Sélection de ville

1. Choisissez une région : 🇷🇪 Réunion · 🇫🇷 Paris · 🇪🇺 Europe
2. Cliquez sur une ville dans la grille
3. Les données se recalculent automatiquement

### Modes

- **🔮 Solo** : éphémérides complètes pour une ville
- **🌐 Comparer** : 2 villes côte à côte
- **📊 Atlas** : comparaison annuelle jusqu'à 4 villes
- **🔋 PV** : simulateur photovoltaïque
- **🛰️ PVGIS** : comparaison modèle vs données réelles

### Raccourcis mobiles

- **Barre basse** : Solo · Atlas · Maintenant · PV · Partager
- **Hamburger** ☰ : Mode · Région · Langue · Export
- **FAB** (boutons flottants) : Actualiser · Maintenant · Position · PDF

### Export

- **📄 PDF** : éphémérides du jour (1 page A4)
- **📊 PDF + graphiques** : éphémérides + visualisations (2 pages)
- **📸 PNG** : graphique d'atlas seul

### URL partageable

Vous pouvez partager un lien direct vers une configuration :

```
https://votre-site.com/?city=MADRID&date=2026-06-21&time=12:00&mode=solo
```

Paramètres : `city`, `date`, `time`, `mode`.

---

## 📚 Documentation

### Technologies utilisées

| Bibliothèque | Version | Usage |
|--------------|---------|-------|
| [SunCalc](https://github.com/mourner/suncalc) | 1.9.0 | Position Soleil / Lune |
| [Astronomy Engine](https://github.com/cosinekitty/astronomy) | 2.1.19 | Planètes, solstices, équinoxes |
| [MapLibre GL JS](https://maplibre.org/) | 4.7.1 | Carte interactive 3D |
| [jsPDF](https://github.com/parallax/jsPDF) | 2.5.1 | Génération PDF |
| [html2canvas](https://html2canvas.hertzen.com/) | 1.4.1 | Capture des graphiques |

### APIs externes

| Service | Usage | Clé API |
|---------|-------|---------|
| [Open-Meteo](https://open-meteo.com/) | Météo + prévisions | ❌ Non |
| [wheretheiss.at](https://wheretheiss.at/) | Position ISS | ❌ Non |
| [OpenStreetMap](https://www.openstreetmap.org/) | Tuiles carte | ❌ Non |
| [AWS Terrarium](https://s3.amazonaws.com/elevation-tiles-prod/) | Relief 3D | ❌ Non |

### Structure du fichier

```
index.html
├── <head>
│   ├── Meta tags (SEO, PWA)
│   ├── CDN links (SunCalc, Astronomy, MapLibre, jsPDF)
│   └── <style> (CSS complet responsive)
├── <body>
│   ├── Conteneur principal
│   ├── Modes (solo / compare / atlas / pv / comparePvgis)
│   ├── Éléments AR (vidéo, canvas, overlay)
│   ├── Modales (calibration, PDF)
│   └── Navigation mobile (barre, drawer, FAB)
└── <script>
    ├── Service Worker (PWA offline)
    ├── Base de données (LOCATIONS + EUROPE_LOCATIONS)
    ├── PVGIS embarqué (PVGIS_PRECOMPUTED)
    ├── Utilitaires (formatage, calculs)
    ├── Rendu (solo, lunaire, atlas, PV)
    ├── Graphiques canvas (adaptatifs)
    ├── Mode AR
    └── Export (PDF, PNG)
```

### Architecture des données

```javascript
// Structure d'une ville
{
  name: "Espagne",           // Pays
  city: "Madrid",            // Ville
  lat: 40.4168,              // Latitude
  lon: -3.7038,              // Longitude
  altitude: 667,             // Altitude (m)
  timezone: 1,               // Fuseau UTC
  dst: true,                 // Heure d'été
  hemisphere: "nord",        // Hémisphère
  population: 3223334,       // Population
  region: "Communauté de Madrid",
  sf: 0.65                   // Facteur solaire (0-1)
}
```

### Données PVGIS

Les données PVGIS sont précalculées et embarquées :

```javascript
// Production mensuelle kWh/kWc
MADRID: [85, 105, 148, 175, 195, 205, 215, 200, 165, 120, 90, 75]
```

- **Tilt** : 20° (Réunion) / 35° (Europe)
- **Orientation** : Nord (Réunion) / Sud (Europe)
- **Source** : PVGIS 5.3 (Commission Européenne)

---

## 🎨 Personnalisation

### Ajouter une ville

Ajoutez une entrée dans `EUROPE_LOCATIONS` ou `LOCATIONS` :

```javascript
const NEW_CITY = {
  name: "Pays",
  city: "Nom de la ville",
  lat: 00.0000,
  lon: 00.0000,
  altitude: 000,
  timezone: 1,
  dst: true,
  hemisphere: "nord",
  population: 00000,
  region: "Région",
  sf: 0.60
};
```

Puis ajoutez ses données PVGIS dans `PVGIS_PRECOMPUTED` :

```javascript
NEW_CITY: [00, 00, 00, 00, 00, 00, 00, 00, 00, 00, 00, 00]
```

### Modifier le thème

Les couleurs sont centralisées dans les variables CSS :

```css
:root {
  --bleu: #0055A4;      /* Bleu France */
  --rouge: #EF4135;     /* Rouge France */
  --azur: #5B9BD5;      /* Azur Réunion */
  --moon: #c8d4e8;      /* Argent lunaire */
  --bg: #0d0d12;        /* Fond sombre */
  --panel: #16161f;     /* Panneaux */
}
```

### Auto-refresh

Ajoutez dans `DOMContentLoaded` :

```javascript
setInterval(() => {
  if ($("dateInput").value === new Date().toISOString().slice(0, 10)) {
    refreshAll();
  }
}, 60000);
```

---

## 📋 Roadmap

- [x] Calculs Soleil / Lune / Planètes
- [x] Carte interactive 3D
- [x] Export PDF
- [x] Module lunaire complet
- [x] Responsive mobile
- [x] Aiguille lunaire directionnelle
- [x] Graphiques adaptatifs
- [x] Europe (44 capitales)
- [ ] Notifications push (heure dorée, ISS)
- [ ] Thème clair pour usage en plein soleil
- [ ] Export ICS (calendrier téléphone)
- [ ] Spots photo (Maïdo, Cap Méchant…)
- [ ] Traduction créole complète
- [ ] API publique REST

---

## 🤝 Contribution

Les contributions sont bienvenues ! Pour contribuer :

1. **Fork** le dépôt
2. **Créez** une branche (`git checkout -b feature/ma-fonctionnalite`)
3. **Committez** vos changements (`git commit -m 'Ajout de ma fonctionnalité'`)
4. **Poussez** la branche (`git push origin feature/ma-fonctionnalite`)
5. **Ouvrez** une Pull Request

### Signaler un bug

Ouvrez une [issue](https://github.com/votre-utilisateur/oracle-solaire/issues) avec :

- Description du problème
- Étapes pour reproduire
- Navigateur et OS utilisés
- Captures d'écran si possible

### Suggérer une fonctionnalité

Ouvrez une [issue](https://github.com/votre-utilisateur/oracle-solaire/issues) avec le label `enhancement`.

---

## 📄 Licence

Ce projet est sous licence **MIT**. Voir le fichier [LICENSE](LICENSE) pour plus de détails.

```
MIT License

Copyright (c) 2026 Oracle Solaire

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## 🙏 Remerciements

- [Vladimir Agafonkin](https://github.com/mourner) pour **SunCalc**
- [Don Cross](https://github.com/cosinekitty) pour **Astronomy Engine**
- [MapLibre](https://maplibre.org/) pour la carte 3D
- [Open-Meteo](https://open-meteo.com/) pour la météo gratuite
- [PVGIS](https://re.jrc.ec.europa.eu/pvg_tools/fr/) pour les données solaires
- [OpenStreetMap](https://www.openstreetmap.org/) pour les tuiles

---

## ⭐ Soutenir le projet

Si Oracle Solaire vous est utile :

- ⭐ **Ajoutez une étoile** au dépôt
- 🐛 **Signalez les bugs**
- 💡 **Suggérez des idées**
- 📤 **Partagez** avec votre entourage

---

## LIENS 

    https://gunout.github.io/oracle-solaire-europeens/

<div align="center">

**🌞 Oracle Solaire** — *Voir le ciel autrement*

[⬆ Retour en haut](#-oracle-solaire)

Fait avec ❤️ à La Réunion et en Europe 🇷🇪🇪🇺

</div>
