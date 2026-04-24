# Portfolio — Yannick Compaore

Portfolio personnel déployable sur Vercel en 2 minutes.

## Stack
- HTML5 / CSS3 / JavaScript vanilla
- Fonts : Syne (display) + DM Mono (body) + Fraunces (serif accent)
- Aucune dépendance, aucun build step requis

## Structure
```
portfolio-yannick/
├── index.html          # Page principale
├── css/
│   └── style.css       # Tous les styles
├── js/
│   └── main.js         # Interactions & animations
├── vercel.json         # Config Vercel (static)
└── README.md
```

## Déploiement sur Vercel

### Option 1 — Via GitHub (recommandé)
1. Push ce dossier sur un repo GitHub
2. Aller sur [vercel.com](https://vercel.com) → "Add New Project"
3. Importer le repo
4. Vercel détecte automatiquement le site statique
5. Cliquer **Deploy** → c'est en ligne en ~30 secondes

### Option 2 — Via CLI
```bash
npm i -g vercel
cd portfolio-yannick
vercel
```

## Personnalisation

### Changer les liens
Dans `index.html`, remplacer :
- `https://linkedin.com/in/yannick-faical-compaore` → ton URL LinkedIn
- `https://github.com/YannickFaical` → ton GitHub
- `ycompaore48@gmail.com` → ton email
- `+212 690-166935` → ton numéro

### Ajouter ton CV PDF
Placer `CV_YANNICK_COMPAORE.pdf` à la racine du dossier.
Le bouton "Télécharger CV" le récupérera automatiquement.

### Modifier les couleurs
Dans `css/style.css`, section `:root` :
```css
--gold: #d4af37;      /* Couleur principale */
--green: #00e5a0;     /* Accent secondaire */
--bg: #080c10;        /* Fond principal */
```

## Features
- ✅ Cursor personnalisé avec trail doré
- ✅ Animations au scroll (IntersectionObserver)
- ✅ Parallax sur les blobs hero
- ✅ Tilt 3D sur les cartes projet
- ✅ Barre de chargement
- ✅ Menu mobile responsive
- ✅ Navbar sticky avec blur
- ✅ Compteurs animés (stats hero)
- ✅ Entièrement responsive mobile
