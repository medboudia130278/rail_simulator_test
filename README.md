# Rail Simulator

Application web React/Vite pour simuler l'usure du rail, les interventions de meulage et les coûts de remplacement.

## Lancer en local

```bash
npm install
npm run dev
```

## Build de production

```bash
npm run build
```

Le build est généré dans `dist/`.

## Structure

- `rail_simulator_Vtest.jsx` : composant principal du simulateur
- `src/main.jsx` : point d'entrée React
- `src/styles.css` : styles globaux minimaux

## Push vers GitHub

```bash
git init -b main
git add .
git commit -m "Initial web app setup"
git remote add origin https://github.com/<ton-compte>/<ton-repo>.git
git push -u origin main
```

## Déploiement Vercel

1. Créer ou ouvrir le repository GitHub.
2. Aller sur Vercel et choisir `Add New Project`.
3. Importer le repository GitHub.
4. Laisser Vercel détecter `Vite`.
5. Build command : `npm run build`
6. Output directory : `dist`
7. Lancer `Deploy`

## Remarque

Le bundle actuel est relativement volumineux car le simulateur est concentré dans un seul composant et embarque `recharts`. Ce n'est pas bloquant pour un premier déploiement, mais on pourra optimiser ensuite si nécessaire.
