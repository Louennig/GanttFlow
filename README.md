# 🎯 GanttFlow

**GanttFlow** est une application web de gestion de projets et de planification avancée inspirée d’outils comme Microsoft Project ou OpenProject.
Elle fonctionne entièrement côté client, sans backend, et permet de gérer des projets complexes directement dans le navigateur.

Lien vers l'outil : https://louennig.github.io/GanttFlow/gantt_patched.html

---

# 🚀 Fonctionnalités principales

## 📊 Gestion de projet complète

* Création, modification et suppression de projets
* Support multi-projets
* Sauvegarde automatique locale (localStorage)
* Import / export JSON

---

## 📌 Gestion avancée des tâches

* Création de tâches avec :

  * dates début / fin
  * progression
  * couleur personnalisée
  * jalons
  * priorité
  * tags
* Sous-tâches illimitées (structure WBS)
* Hiérarchie complète avec regroupement
* Historique et commentaires par tâche

---

## 📅 Diagramme de Gantt interactif

* Timeline dynamique basée sur les jours ouvrés
* Exclusion automatique week-ends et jours non travaillés
* Barres Gantt interactives :

  * drag & drop horizontal
  * redimensionnement (début / fin)
  * affichage progression intégré
* Zoom multi-échelles (jour → année)
* Mini-map de navigation pour grands projets

---

## 🔗 Dépendances avancées

* Liaisons entre tâches avec SVG
* Types de dépendances :

  * FS (Finish → Start)
  * SS (Start → Start)
  * FF (Finish → Finish)
  * SF (Start → Finish)
* Gestion des délais (lag)
* Recalcul automatique des positions

---

## 🧠 Moteur de planification

* Recalcul automatique global du projet
* Mode manuel / automatique
* Détection d’incohérences
* Calcul du chemin critique
* Gestion des marges (flottants)

---

## 👥 Ressources & charge

* Affectation de ressources (humaines / matérielles)
* Calcul de charge par jour / semaine / mois
* Détection de surcharge
* Estimation des coûts :

  * coût tâche
  * coût projet global

---

## 📈 Suivi et analyse

* Dashboard de projet :

  * progression globale
  * tâches terminées / en retard
  * budget consommé
  * tâches critiques
* Baseline (référence projet)
* Comparaison planning réel vs initial

---

## 🔎 Organisation & filtres

* Recherche de tâches
* Filtres avancés :

  * statut
  * priorité
  * tags
  * ressources
* Multi-sélection et actions groupées

---

## 🧭 Vues multiples

* Vue Gantt
* Vue tableau
* Vue Kanban
* Vue calendrier
* Vue charge des ressources

---

## 📦 Import / Export

* JSON (complet projet)
* CSV / XLSX (données)
* PDF (rapport Gantt propre)
* PNG (export visuel)
* Compatible structure type Microsoft Project (XML simplifié)

---

## ⚙️ Interactions utilisateur

* Drag & drop des tâches
* Resize interactif
* Double-clic édition
* Modales dynamiques
* Undo / Redo
* Raccourcis clavier (Ctrl+Z, Ctrl+Y, etc.)

---

## 🎨 Interface

* Design moderne type SaaS
* UI inspirée Notion / Microsoft Project
* Mode clair / sombre
* Animations fluides CSS
* Interface optimisée pour projets complexes

---

# 🧱 Architecture technique

Projet 100% **frontend vanilla** :

```
index.html
style.css
app.js
ganttEngine.js
taskManager.js
timeline.js
dependencyManager.js
storage.js
exportPdf.js
```

Même dans un fichier unique HTML, le code est structuré en modules logiques simulés.

---

# 💾 Stockage

Aucune base de données.

* localStorage pour sauvegarde rapide
* export/import JSON pour persistance complète

---

# 📄 Export PDF

* Format A4 paysage
* Rendu fidèle du Gantt
* Inclut :

  * tâches
  * timeline
  * dépendances
  * progression

---

# 🧠 Objectif du projet

GanttFlow vise à reproduire un outil de gestion de projet complet utilisable en production légère, capable de gérer :

* plusieurs centaines de tâches
* dépendances complexes
* planification automatique
* suivi budgétaire et ressources

Tout cela **sans backend**, directement dans le navigateur.

---

# ⚠️ Contraintes techniques

* HTML / CSS / JavaScript vanilla uniquement
* Aucun framework
* Aucun serveur
* Données locales uniquement
* Librairie autorisée : html2pdf.js (export PDF)

---

# 🏁 Vision

Un outil de gestion de projet complet, léger, autonome, capable de rivaliser avec des solutions professionnelles tout en restant simple à lancer :
👉 ouvrir un fichier HTML suffit pour travailler.

