# TRADE ACTIVE CAMEROON S.A. — Plateforme Web Officielle

Site vitrine institutionnel et catalogue technique de **TRADE ACTIVE CAMEROON S.A.**, Société Anonyme agréée par le Ministère du Commerce (Arrêté N° 0096/MINCOMMERCE).

- **Siège social & Showroom :** Yaoundé, Biyem-Assi (Rond-Point Express, BP 1252 Yaoundé - Cameroun)
- **Ligne Directe / WhatsApp Business :** (+237) 655 41 73 42
- **Email Officiel :** info@tradeactivecameroon.com
- **Partenaires Internationaux & Alliances Techniques :** DRAGFLOW (Italie), KLINDEX (Italie), PAVA RESINE / VIRES (Italie), CMAlifts (Italie), THINK BRICK AUSTRALIA (Australie), ICES — Engineering Structures.

---

## 🚀 Déploiement en Production sur Vercel (Recommandé)

Le site est entièrement configuré avec le fichier [`vercel.json`](vercel.json) pour un déploiement instantané et haute performance sur le réseau mondial Edge de **Vercel**.

### Méthode 1 : Via l'interface Vercel & GitHub (En 1 Clic)
1. Poussez votre projet sur votre compte GitHub (ou GitLab / Bitbucket).
2. Rendez-vous sur votre tableau de bord **[Vercel Dashboard](https://vercel.com/new)**.
3. Cliquez sur **Add New...** > **Project** et importez votre dépôt.
4. Dans les paramètres du projet :
   - **Framework Preset :** `Other` *(détecté automatiquement)*
   - **Root Directory :** `./` *(racine)*
   - **Build & Output Settings :** Laisser les commandes vides (site statique pur sans étape de compilation lourde).
5. Cliquez sur **Deploy** : Votre site est en ligne en moins de 15 secondes avec certificat SSL HTTPS gratuit et CDN mondial !

### Méthode 2 : Déploiement Direct via le CLI Vercel
Ouvrez votre terminal dans le dossier du projet et exécutez :
```bash
# Première connexion / initialisation
npx vercel

# Déploiement direct en production
npx vercel --prod
```

---

## ⚡ Optimisations Vercel incluses dans `vercel.json`
- **Clean URLs (`cleanUrls: true`) :** URLs épurées sans extension `.html` (ex: `https://votre-domaine.com/metiers-btp`).
- **Règles de Réécriture (`rewrites`) :** Alias d'accès rapide (`/accueil`, `/btp`, `/marques`, `/academie`, `/a-propos`, `/projets`, `/catalogues`).
- **En-têtes de Sécurité HTTP :** Protection `X-Frame-Options`, `X-Content-Type-Options`, `X-XSS-Protection`, `Referrer-Policy` et `Permissions-Policy`.
- **Mise en cache CDN Edge :** Cache agressif (1 an immuable) pour tous les assets (`/assets/*`) et revalidation immédiate pour les fichiers HTML.
- **Gestion d'erreur 404 :** Routage automatique vers la page sur mesure [`404.html`](404.html).

---

## 🌐 Déploiement Alternatif sur Netlify

Le site est entièrement architecturé, optimisé et prêt pour un déploiement instantané sur **Netlify**.

### Méthode 1 : Déploiement Glisser-Déposer (1 Clic, Sans Ligne de Commande)
1. Rendez-vous sur **[Netlify Drop](https://app.netlify.com/drop)**.
2. Connectez-vous à votre compte Netlify (ou créez-en un gratuitement).
3. Glissez-déposez l'ensemble du dossier `TRADE ACTIVE CAMEROON` dans la zone de téléversement.
4. En quelques secondes, votre site est en ligne avec une URL HTTPS sécurisée (ex: `https://votre-site.netlify.app`).

---

### Méthode 2 : Déploiement via GitHub / Git
1. Initialisez votre dépôt Git et publiez-le sur GitHub :
   ```bash
   git init
   git add .
   git commit -m "Site TRADE ACTIVE CAMEROON S.A. prêt pour Netlify"
   git remote add origin https://github.com/votre-nom/trade-active-cameroon.git
   git push -u origin main
   ```
2. Dans le tableau de bord **Netlify** :
   - Cliquez sur **Add new site** > **Import an existing project**.
   - Choisissez **GitHub** et sélectionnez votre dépôt.
   - Les paramètres de build sont automatiquement détectés grâce au fichier `netlify.toml` :
     - **Publish directory :** `.` (racine)
     - **Build command :** *(laisser vide)*
   - Cliquez sur **Deploy site**.

---

### Méthode 3 : Déploiement via le CLI Netlify
```bash
# Déploiement direct en production
npx netlify-cli deploy --prod --dir=.
```

---

## 📁 Architecture des Fichiers de Déploiement Netlify

| Fichier | Rôle & Fonctionnalité |
| :--- | :--- |
| **`netlify.toml`** | Configuration principale Netlify (répertoire de publication, règles de réécriture d'URL, en-têtes HTTP de sécurité et mise en cache CDN). |
| **`_redirects`** | Règles de redirection pour URLs propres (ex: `/metiers-btp` sans `.html`) et routage automatique vers la page 404. |
| **`_headers`** | En-têtes de sécurité (X-Frame-Options, X-Content-Type-Options, Referrer-Policy) et mise en cache agressive des images/CSS (1 an). |
| **`404.html`** | Page d'erreur 404 sur mesure reprenant l'identité visuelle de l'entreprise et orientant les visiteurs vers les pages clés. |
| **`robots.txt`** | Directives pour les robots d'indexation (Google, Bing) autorisant le crawl et référençant le plan de site. |
| **`sitemap.xml`** | Plan de site XML complet avec les 7 pages officielles et leurs priorités SEO. |
| **`site.webmanifest`** | Manifeste d'application web pour l'affichage sur mobile (PWA, icônes, thème couleur `#0E5A80`). |
| **`.gitignore`** | Exclusion des fichiers locaux, logs et dépendances de développement. |

---

## 📬 Formulaires de Contact & Devis (Netlify Forms)

Tous les formulaires du site intègrent l'attribut natif `data-netlify="true"` :
1. **Double Réception :** 
   - **Netlify Forms :** Chaque soumission est automatiquement archivée dans votre tableau de bord Netlify (avec possibilité de recevoir des notifications par email).
   - **WhatsApp Business Direct :** Le client est simultanément redirigé vers le WhatsApp de l'entreprise (`+237 655 41 73 42`) avec son message pré-rempli pour un traitement commercial immédiat.
2. **Formulaires Actifs :**
   - `devis-express` (sur `index.html`)
   - `devis-btp` (sur `metiers-btp.html`)
   - `partenariat-marques` (sur `marques-partenaires.html`)
   - `inscription-formation` (sur `formation.html`)
   - `contact-direction` (sur `entreprise.html`)
   - `contact-general` (sur `contact.html`)

---

## 🌐 Pages Officielles du Site

- [`index.html`](index.html) : Accueil, Grands Pôles & Catalogue Équipements
- [`metiers-btp.html`](metiers-btp.html) : BTP, Terrassement, Génie Civil & VRD
- [`marques-partenaires.html`](marques-partenaires.html) : DRAGFLOW, KLINDEX, PAVARESINE, VIRES & CMAlifts
- [`formation.html`](formation.html) : Académie Pratique & Sessions Professionnelles
- [`entreprise.html`](entreprise.html) : Gouvernance, Agrément N° 0096 & Équipe
- [`contact.html`](contact.html) : Showroom Yaoundé, Carte & Formulaire Détaillé
- [`galerie.html`](galerie.html) : 24 Réalisations HD au Cameroun
- [`404.html`](404.html) : Page d'erreur personnalisée
