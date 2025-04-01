# 🚀 React-TS

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Electron](https://img.shields.io/badge/Electron-22.x-47848F.svg?logo=electron)
![Vite](https://img.shields.io/badge/vite-4.x-646CFF.svg?logo=vite)
![React](https://img.shields.io/badge/React-18.x-61DAFB.svg?logo=react)
![TypeScript](https://img.shields.io/badge/TypeScript-4.x-3178C6.svg?logo=typescript)

Un'applicazione Electron avanzata con React e TypeScript. Ideale per sviluppare applicazioni desktop robuste e moderne con tipizzazione statica e componenti UI reattivi.

## 📋 Table of Contents
- [Features](#-features)
- [Project Structure](#-project-structure)
- [Recommended IDE Setup](#-recommended-ide-setup)
- [Project Setup](#-project-setup)
- [Package Managers](#-package-managers)
- [Resources](#-resources)

## ✨ Features

- ⚛️ React framework per componenti UI
- 📊 Supporto per dashboard e visualizzazioni statistiche
- 🗓️ Possibilità di implementare timeline e viste calendario
- 💾 Salvataggio dati in localStorage (100% offline)
- 📤 Funzionalità di import/export e backup
- 🔄 Hot Module Replacement (HMR) durante lo sviluppo
- ⚡ Build ultra-veloce con Vite bundler
- 📦 Packaging cross-platform
- 🔒 Type safety con TypeScript
- 🧩 Integrazione nativa con Node.js
- 🔍 Linting TypeScript con ESLint
- 🎨 Formattazione del codice con Prettier
- 🖌️ Architettura basata su componenti

## 🗂️ Project Structure

```
bl-electron-vite-typescript-react/
├── build/              # Build resources and configuration
├── dist/               # Build output directory
├── out/                # Packaged application output
├── src/
│   ├── main/           # Main process code
│   │   └── index.ts    # Main entry point
│   ├── preload/        # Preload scripts
│   │   └── index.ts    # Preload entry point
│   └── renderer/       # Renderer process code (React)
│       ├── App.tsx     # Root React component
│       ├── components/ # React components
│       ├── hooks/      # Custom React hooks
│       ├── utils/      # Utility functions
│       ├── index.html  # HTML template
│       └── index.tsx   # Renderer entry point
├── .eslintrc           # ESLint configuration
├── electron-builder.yml # Electron builder configuration
├── package.json        # Project dependencies and scripts
├── tsconfig.json       # TypeScript configuration
└── vite.config.ts      # Vite configuration
```

## 🛠️ Recommended IDE Setup

- [VSCode](https://code.visualstudio.com/) + [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) + [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)

## 🚀 Project Setup

### 📥 Install

```bash
$ pnpm install
```

### 🔧 Development

```bash
$ pnpm dev
```

### 📦 Build

```bash
# For windows
$ pnpm build:win

# For macOS
$ pnpm build:mac

# For Linux
$ pnpm build:linux
```

## 📦 Package Managers

Questo progetto supporta diversi package manager. Ecco come utilizzare ciascuno:

### NPM

NPM è il package manager predefinito per Node.js.

**Installazione NPM:**
```bash
# Incluso con l'installazione di Node.js
```

**Setup progetto con NPM:**
```bash
# Installazione dipendenze
$ npm install

# Avvio server di sviluppo
$ npm run dev

# Build dell'applicazione
$ npm run build:win
$ npm run build:mac
$ npm run build:linux
```

**Caratteristiche principali:**
- 📚 Vasto ecosistema di pacchetti
- 🔒 Struttura gerarchica di node_modules
- 📋 Package.json per la gestione delle dipendenze

### Yarn

Yarn è un'alternativa rapida, affidabile e sicura a NPM.

**Installazione Yarn:**
```bash
# Installazione tramite NPM
$ npm install -g yarn
```

**Setup progetto con Yarn:**
```bash
# Installazione dipendenze
$ yarn

# Avvio server di sviluppo
$ yarn dev

# Build dell'applicazione
$ yarn build:win
$ yarn build:mac
$ yarn build:linux
```

**Caratteristiche principali:**
- ⚡ Velocità di installazione superiore
- 📦 Caching offline
- 🔒 Maggiore sicurezza con checksum
- 📋 yarn.lock per installazioni deterministiche

### PNPM

PNPM è un package manager efficiente in termini di spazio su disco.

**Installazione PNPM:**
```bash
# Installazione tramite NPM
$ npm install -g pnpm
```

**Setup progetto con PNPM:**
```bash
# Installazione dipendenze
$ pnpm install

# Avvio server di sviluppo
$ pnpm dev

# Build dell'applicazione
$ pnpm build:win
$ pnpm build:mac
$ pnpm build:linux
```

**Caratteristiche principali:**
- 💾 Risparmio di spazio su disco tramite symlink
- 🚀 Velocità di installazione elevata
- 🔄 Storage con indirizzamento basato sul contenuto
- 📋 pnpm-lock.yaml per blocco delle dipendenze

### Confronto

| Funzionalità          | NPM     | Yarn    | PNPM    |
|-----------------------|---------|---------|---------|
| Utilizzo disco        | Alto    | Alto    | Basso   |
| Velocità installazione| Lenta   | Veloce  | Velocissima |
| Installazioni parallele| Limitato| Sì      | Sì      |
| Supporto workspaces   | Limitato| Buono   | Ottimo  |
| Modalità offline      | Limitato| Buono   | Buono   |
| Sicurezza             | Buona   | Migliore| Migliore|

## 📚 Resources

- [Electron Documentation](https://www.electronjs.org/docs)
- [React Documentation](https://reactjs.org/docs/getting-started.html)
- [TypeScript Documentation](https://www.typescriptlang.org/docs/)
- [Vite Documentation](https://vitejs.dev/guide/)
- [NPM Documentation](https://docs.npmjs.com/)
- [Yarn Documentation](https://yarnpkg.com/getting-started)
- [PNPM Documentation](https://pnpm.io/motivation)
