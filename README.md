# TSX Rocket Tracker 🚀

Tracker personnel de penny stocks TSX / TSXV basé sur l'analyse de **3 514 fusées historiques** (2000–2026).

## Fonctionnalités

- 🔍 Recherche de n'importe quel ticker TSX/TSXV
- 📊 Graphique live via TradingView
- 💰 Prix en temps réel via Yahoo Finance
- ⭐ Watchlist personnelle (sauvegardée dans ton navigateur)
- 🎯 Score algorithmique basé sur les patterns historiques
- 📱 Responsive (fonctionne sur mobile)

## Déploiement sur GitHub Pages (5 minutes)

### Étape 1 — Créer le dépôt

1. Va sur [github.com](https://github.com) et connecte-toi
2. Clique **New repository**
3. Nom : `tsx-tracker` (ou ce que tu veux)
4. Coche **Public**
5. Clique **Create repository**

### Étape 2 — Uploader les fichiers

1. Dans ton nouveau dépôt, clique **uploading an existing file**
2. Glisse-dépose ces 2 fichiers :
   - `index.html`
   - `stock.html`
3. Clique **Commit changes**

### Étape 3 — Activer GitHub Pages

1. Va dans **Settings** → **Pages** (dans le menu de gauche)
2. Source : **Deploy from a branch**
3. Branch : **main** / **(root)**
4. Clique **Save**

### Étape 4 — Accéder au site

Après 1-2 minutes, ton site sera accessible à :
```
https://TON-USERNAME.github.io/tsx-tracker/
```

## Utilisation

### Rechercher un titre
- Entre le ticker dans la barre de recherche : `RPX.V`, `MN.V`, `GOLD.TO`
- Appuie sur Entrée ou clique ANALYSER

### Format des tickers
- TSXV : `RPX.V`, `MN.V`, `MINE.V`
- TSX principale : `ABX.TO`, `CNQ.TO`

### Watchlist
- Depuis la fiche d'un titre, clique **+ Ajouter à ma watchlist**
- La watchlist est sauvegardée localement dans ton navigateur
- Pour retirer un titre : survole la carte et clique ✕

## Mettre à jour les données

Le top 20 est basé sur l'analyse du 10 mai 2026.
Pour mettre à jour avec de nouvelles données :
1. Relance `tsx_analyzer.py` sur ta machine
2. Copie les nouvelles données dans `stock.html` (objet `TOP20_DATA`)

## Structure

```
tsx-tracker/
├── index.html    ← Page principale (watchlist + top 20 + recherche)
├── stock.html    ← Fiche détaillée d'un titre
└── README.md     ← Ce fichier
```

## Avertissement

⚠️ Ce tracker est à titre informatif uniquement. Les penny stocks sont des investissements à très haut risque. Les patterns historiques ne garantissent aucun rendement futur. Ne jamais investir plus que ce qu'on est prêt à perdre entièrement.

---

*Généré avec Claude · Données: Yahoo Finance + TradingView + EODHD*
