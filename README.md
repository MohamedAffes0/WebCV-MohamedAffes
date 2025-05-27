# 🌐 WebCV – Mohamed Affes

> **CV en ligne** réalisé avec **[Astro](https://astro.build/)**, prêt pour un déploiement statique rapide (Netlify, Vercel, GitHub Pages, etc.).

# Screenshot
<p align="center">
    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/MohamedAffes0/WebCV-MohamedAffes/blob/main/docs/images/preview-dark.png">
    <source media="(prefers-color-scheme: light)" srcset="https://github.com/MohamedAffes0/WebCV-MohamedAffes/blob/main/docs/images/preview-light.png">
</p>

---

## Sommaire
1. [Fonctionnalités](#fonctionnalités)
2. [Architecture du projet](#architecture-du-projet)
3. [Prérequis](#prérequis)
4. [Installation locale](#installation-locale)
5. [Commandes fondamentales](#commandes-fondamentales)
6. [Déploiement](#déploiement)
7. [Personnalisation](#personnalisation)
8. [Contribuer](#contribuer)

---

## Fonctionnalités

- ⚡ **Statique & ultra‐rapide** : rendu pré‑compilé par Astro.  
- 📱 **Responsive** : design mobile‑first et adaptatif.  
- 🌑 **Dark mode** (activé par défaut) inspiré d’Appwrite.  
- 🚀 **Déploiement 1‑clic** sur Netlify.  
- ✍️ **Facile à éditer** : un simple fichier `.astro` pour vos infos.  

---

## Architecture du projet

```text
.
├── public/               # Fichiers statiques (images, icônes…)
├── src/
│   ├── components/       # Composants Astro/JSX réutilisables
│   ├── layouts/          # Gabarits de pages (Layout.astro)
│   └── pages/            # Pages du site (index.astro, 404.astro…)
├── .netlify/             # Config Netlify (op­tion­nel)
├── astro.config.mjs      # Config globale Astro
├── package.json          # Dépendances & scripts npm
├── tsconfig.json         # Config TypeScript (facultatif)
└── README.md             # Ce fichier
```

> **Astuce :** pour voir la structure complète, exécute `tree -I "node_modules|dist"` ou `npm run list:files` si tu as le script.

---

## Prérequis

| Outil | Version minimale | Installation |
|-------|------------------|--------------|
| Node.js | **18.0.0** | <https://nodejs.org/> |
| npm     | **9.0.0** (ou supérieur) | livré avec Node.js |

---

## Installation locale

1. **Cloner le dépôt :**
   ```bash
   git clone https://github.com/MohamedAffes0/WebCV-MohamedAffes.git
   cd WebCV-MohamedAffes
   ```

2. **Installer les dépendances (dont Astro) :**
   ```bash
   npm install
   ```

   > Astro est référencé dans `package.json`; aucune commande supplémentaire n’est nécessaire.

3. **Lancer le serveur de développement :**
   ```bash
   npm run dev
   ```
   Accède ensuite à **<http://localhost:3000>**.

---

## Commandes fondamentales

| Action | Commande |
|--------|----------|
| Installer Astro dans un _nouveau_ projet | `npm create astro@latest` |
| Lancer le serveur de dev (hot reload) | `npm run dev` |
| Construire la version production | `npm run build` |
| Aperçu de la build locale | `npm run preview` |
| Nettoyer le cache | `npm run astro -- cleanup` |

---

## Déploiement

### Netlify

1. Crée un compte sur <https://app.netlify.com/> puis **« New Site from Git »**.  
2. Renseigne :
   - **Build command :** `npm run build`
   - **Publish directory :** `dist`
3. Clique **Deploy Site** – Netlify gère tout !  
   Les déploiements suivants se feront automatiquement à chaque `git push`.

### Autres plateformes

Le dossier **`dist/`** est 100 % statique ; tu peux l’héberger sur Vercel, GitHub Pages, Cloudflare Pages, etc.

---

## Personnalisation

| Élément | Fichier à modifier |
|---------|--------------------|
| Contenu du CV | `src/pages/index.astro` |
| Mise en page globale | `src/layouts/Main.astro`, `src/layouts/Blog.astro` |
| Style / thèmes | `src/styles/` ou Tailwind CSS (si installé) |
| Images | `public/` |

---

## Contribuer

Les _pull requests_ sont les bienvenues !  
1. Fork → feature branch → commit → PR.  
2. Assure‑toi que le linter et la build passent (`npm test` si défini).

---

> ⭐️ Si ce projet t’a aidé, n’oublie pas de laisser une _star_ !

