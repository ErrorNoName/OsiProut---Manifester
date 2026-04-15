<div align="center">

<!-- ═══════════════════════════════════════════════════════════
     OsiProut Manifester — README
     ═══════════════════════════════════════════════════════════ -->

# OsiProut Manifester

**Steam Manifest Manager — OsiProut edition**

[![Version](https://img.shields.io/badge/version-1.1.1-7c5cbf?style=for-the-badge&labelColor=0e0e17)](https://github.com/osiprout/manifester)
[![Electron](https://img.shields.io/badge/Electron-41-956ee0?style=for-the-badge&logo=electron&logoColor=white&labelColor=0e0e17)](https://www.electronjs.org/)
[![Platform](https://img.shields.io/badge/Windows-x64-58a8f0?style=for-the-badge&logo=windows&logoColor=white&labelColor=0e0e17)](.)
[![License](https://img.shields.io/badge/Portable-.exe-50c87e?style=for-the-badge&labelColor=0e0e17)](.)

<br/>

<samp>Browse · Download · Install · Play</samp>

<br/>

</div>

<br/>

---

<br/>

<div align="center">

## 🎮 &ensp; À propos

</div>

<table>
<tr>
<td width="100%" align="center">

**OsiProut Manifester** est un gestionnaire de manifests Steam tout-en-un,
conçu pour parcourir, télécharger et installer des manifests et fichiers `.lua` directement dans votre installation Steam.
<br/><br/>
L'application intègre un système de **patch Online-Fix / Goldberg** pour le multijoueur,
une bibliothèque locale avec lancement de jeux, et un **mode BigPicture** immersif avec shader WebGL volumétrique.
<br/><br/>
Interface sombre haut de gamme, glassmorphisme, accents violets — pensé pour les passionnés.

</td>
</tr>
</table>

<br/>

---

<br/>

<div align="center">

## ✨ &ensp; Fonctionnalités

</div>

<br/>

<table>
<thead>
<tr>
<th width="50%">🔍 &ensp; Catalogue</th>
<th width="50%">📦 &ensp; Manifest</th>
</tr>
</thead>
<tbody>
<tr>
<td>

- Catalogue distant avec **cache 24h**
- Recherche par nom ou AppID (debounce)
- Filtre par type : game, DLC, music, video, demo
- Quick-pills : **All** · **DRM-free** · **NSFW**
- **Scroll infini** (batches de 50)
- Panneau détail : cover, branches, dépôts, fichiers, DLC

</td>
<td>

- Téléchargement de fichiers **`.lua`** et **`.manifest`**
- Détection auto des archives **ZIP** (PK magic bytes)
- Installation directe dans `stplug-in` et `depotcache`
- Barre de progression en temps réel
- **Quota journalier** (50/jour) avec compteur visuel
- Sélection de **branche** et type de fichiers

</td>
</tr>
</tbody>
</table>

<br/>

<table>
<thead>
<tr>
<th width="50%">📚 &ensp; Bibliothèque</th>
<th width="50%">🔧 &ensp; Online-Fix / Goldberg</th>
</tr>
</thead>
<tbody>
<tr>
<td>

- Bibliothèque locale persistante (`library.json`)
- Fiche détaillée : cover, type, AppID, branche, date
- Liste des fichiers installés avec chemins
- **Lancer** / **Arrêter** un jeu depuis l'app
- **Exe personnalisé** par jeu (sauvegardé)
- Suppression de jeu / réinstallation

</td>
<td>

- Détection auto du chemin du jeu via `libraryfolders.vdf`
- Vérification du statut Online-Fix
- Scan du dossier jeu pour patchs existants
- **Appliquer** le patch Goldberg multijoueur
- **Retirer** le patch (restauration)
- Barre de progression + logs en direct

</td>
</tr>
</tbody>
</table>

<br/>

<table>
<thead>
<tr>
<th width="50%">⚡ &ensp; Install en masse</th>
<th width="50%">♻️ &ensp; Steam</th>
</tr>
</thead>
<tbody>
<tr>
<td>

- Zone de texte **bulk** : coller URLs ou AppIDs
- **Auto-paste** depuis le presse-papiers (toggle)
- Choix du type de fichier (`.lua` + `.manifest`)
- File d'attente avec statut par jeu
- Lancement batch en un clic

</td>
<td>

- Détection auto des chemins Steam (Registre + VDF)
- **Redémarrage de Steam** (shutdown → relaunch)
- Détection & lancement de **SteamTools**
- Protocole `steam://install` pour jeux manquants
- Détection du port debug CEF (WMI, cache 60s)

</td>
</tr>
</tbody>
</table>

<br/>

<table>
<thead>
<tr>
<th width="50%">🖥️ &ensp; Interface</th>
<th width="50%">🔐 &ensp; Auth & Système</th>
</tr>
</thead>
<tbody>
<tr>
<td>

- **Barre de titre custom** (frameless, drag natif)
- Splash screen anti-flashbang
- **Mode BigPicture** avec carousel GSAP
- Shader WebGL2 volumétrique (Three.js)
- Toasts de notification
- Thème sombre glassmorphisme

</td>
<td>

- Connexion via **Discord OAuth**
- Gate d'authentification obligatoire
- Session cookies persistantes
- Indicateur de statut auth (titlebar)
- **Auto-updater** avec progression
- Logs applicatifs (`app.log`)

</td>
</tr>
</tbody>
</table>

<br/>

---

<br/>

<div align="center">

## 🛠️ &ensp; Stack technique

</div>

<br/>

<div align="center">

| Composant | Technologie |
|:---|:---|
| **Runtime** | Electron 41 |
| **Build** | electron-builder · Portable `.exe` x64 |
| **Polices** | Syne (Google Fonts) |
| **Icônes** | Font Awesome 6.4.0 |
| **Animation** | GSAP 3.12.5 |
| **3D** | Three.js 0.160.0 (WebGL2) |
| **Archives** | adm-zip · 7zip-min |
| **Backend** | `generator.ryuu.lol` (API distante) |

</div>

<br/>

---

<br/>

<div align="center">

## 🎨 &ensp; Palette

</div>

<br/>

<div align="center">

| Token | Couleur | Aperçu |
|:---|:---|:---:|
| `--accent` | `#7c5cbf` | ![#7c5cbf](https://img.shields.io/badge/-%20-7c5cbf?style=flat-square) |
| `--accent-h` | `#956ee0` | ![#956ee0](https://img.shields.io/badge/-%20-956ee0?style=flat-square) |
| `--bg-1` | `#0e0e17` | ![#0e0e17](https://img.shields.io/badge/-%20-0e0e17?style=flat-square) |
| `--bg-2` | `#13131e` | ![#13131e](https://img.shields.io/badge/-%20-13131e?style=flat-square) |
| `--tx-1` | `#e8e8f4` | ![#e8e8f4](https://img.shields.io/badge/-%20-e8e8f4?style=flat-square) |
| `--tx-2` | `#9898b8` | ![#9898b8](https://img.shields.io/badge/-%20-9898b8?style=flat-square) |
| `--success` | `#50c87e` | ![#50c87e](https://img.shields.io/badge/-%20-50c87e?style=flat-square) |
| `--error` | `#f05858` | ![#f05858](https://img.shields.io/badge/-%20-f05858?style=flat-square) |
| `--warn` | `#e0962e` | ![#e0962e](https://img.shields.io/badge/-%20-e0962e?style=flat-square) |
| `--info` | `#58a8f0` | ![#58a8f0](https://img.shields.io/badge/-%20-58a8f0?style=flat-square) |

</div>

<br/>

---

<br/>

<div align="center">

## 🚀 &ensp; Installation

</div>

<br/>

### Utilisation rapide

> Téléchargez le `.exe` portable depuis la page **Releases** — aucune installation nécessaire.

```
OsiProut-Manifester.exe
```

Double-cliquez pour lancer. L'application détecte automatiquement vos chemins Steam.

<br/>

### Build depuis les sources

```bash
# Cloner le dépôt
git clone https://github.com/osiprout/manifester.git
cd manifester

# Installer les dépendances
npm install

# Lancer en dev
npm run dev

# Build portable (.exe)
npm run build
```

<br/>

### Structure du projet

```
OsiProut-Manifester/
├── main.js              # Process principal Electron (IPC, downloads, Steam)
├── preload.js           # Bridge sécurisé (contextBridge)
├── src/
│   ├── index.html       # Interface (titlebar, sidebar, panels)
│   ├── renderer.js      # Logique UI (carousel, search, detail, library)
│   └── styles.css       # Thème sombre glassmorphisme
├── data/
│   ├── games.json       # Cache catalogue (24h)
│   └── library.json     # Bibliothèque locale
├── config.json          # Configuration utilisateur
├── icon.png             # Icône application
├── Build.bat            # Script de build interactif
└── package.json         # Métadonnées & electron-builder config
```

<br/>

---

<br/>

<div align="center">

## ⌨️ &ensp; Raccourcis

</div>

<br/>

<div align="center">

| Raccourci | Action |
|:---|:---|
| `Ctrl + Shift + I` | Ouvrir / Fermer les DevTools |
| `Mode BigPicture` | Toggle via l'icône gamepad dans la titlebar |

</div>

<br/>

---

<br/>

<div align="center">

## 📡 &ensp; Architecture IPC

</div>

<br/>

<details>
<summary>&ensp; <b>Channels — Main ↔ Renderer</b> &ensp; (cliquer pour développer)</summary>

<br/>

#### `ipcMain.handle` — Requêtes (invoke / return)

| Channel | Rôle |
|:---|:---|
| `get-config` / `save-config` | Lire / écrire la configuration |
| `fetch-games` | Catalogue distant (avec cache) |
| `get-manifest-info` | Infos manifest par AppID |
| `download-install` | Télécharger & installer les fichiers |
| `get-download-stats` | Compteur quota du jour |
| `detect-steam-paths` | Détection auto chemins Steam |
| `browse-path` | Dialogue natif fichier/dossier |
| `check-auth` / `open-auth-window` / `logout` | Authentification Discord |
| `get-library` / `remove-from-library` | Gestion bibliothèque |
| `launch-game` / `stop-game` | Lancer / arrêter un jeu |
| `detect-game-path` | Détecter le chemin du jeu |
| `check-online-fix` / `scan-game-for-patch` | Vérifier patches |
| `apply-online-fix` / `remove-online-fix` | Appliquer / retirer Goldberg |
| `save-custom-exe` / `get-custom-exe` | Exe personnalisé par jeu |
| `restart-steam` | Redémarrer Steam + SteamTools |
| `detect-steamtools` / `check-steamtools-running` | Gestion SteamTools |
| `check-update-now` / `download-update` | Auto-updater |
| `get-app-version` | Version de l'app |
| `open-folder` / `open-external` / `read-clipboard` | Utilitaires système |

#### `ipcMain.on` — Événements (fire-and-forget)

| Channel | Rôle |
|:---|:---|
| `splash-ready` | Splash screen chargé |
| `win-minimize` / `win-maximize` / `win-close` | Contrôles fenêtre |
| `toggle-devtools` | Basculer DevTools |
| `overlay-close` / `overlay-download` | Overlay in-game |

#### Main → Renderer — Événements push

| Channel | Rôle |
|:---|:---|
| `auth-changed` | Statut auth mis à jour |
| `dl-progress` | Progression téléchargement |
| `restart-progress` | Progression redémarrage Steam |
| `update-available` / `update-dl-progress` | Mises à jour |
| `game-exited` | Jeu terminé |
| `fix-progress` | Progression patch Online-Fix |
| `open-game` | Ouvrir un jeu (overlay) |

</details>

<br/>

---

<br/>

<div align="center">

## 📋 &ensp; Configuration

</div>

<br/>

Le fichier `config.json` à la racine stocke les chemins détectés et préférences :

```jsonc
{
  "steam_config_path": "C:\\Program Files (x86)\\Steam\\config",
  "depot_cache_path": "C:\\Program Files (x86)\\Steam\\depotcache",
  "steam_exe_path": "C:\\Program Files (x86)\\Steam\\steam.exe",
  "steamtools_path": "..."
}
```

> Les chemins sont **auto-détectés** au premier lancement via le Registre Windows et le parsing de `libraryfolders.vdf`.

<br/>

---

<br/>

<div align="center">

<br/>

<br/><br/>

<samp>OsiProut Manifester v1.1.1</samp>

<br/>

[![Made with Electron](https://img.shields.io/badge/Made%20with-Electron-7c5cbf?style=flat-square&logo=electron&logoColor=white&labelColor=0e0e17)](https://www.electronjs.org/)
&nbsp;
[![Windows](https://img.shields.io/badge/Windows-x64-956ee0?style=flat-square&logo=windows&logoColor=white&labelColor=0e0e17)](.)

<br/><br/>

</div>
