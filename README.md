# 🐓 Mastermind — Le Coq Francis

Jeu de **Mastermind** (casse-code) aux couleurs de **Le Coq Francis**, jouable dans le navigateur et lançable comme **Mini App Telegram**.

- 🌐 **En ligne :** https://franclecoq.github.io/Mastermind
- 🤖 **Telegram :** https://t.me/FrancisLeCoqBot/Mastermind

---

## 🎮 Le jeu en bref

Devine la combinaison secrète de couleurs choisie par Francis. À chaque proposition, tu reçois des indices :

| Indice | Signification |
|--------|---------------|
| ⚪ **Blanc** | Bonne couleur, **bonne** place |
| 🟣 **Violet** | Bonne couleur, **mauvaise** place |

Casse le code avant d'épuiser tes essais !

### Deux modes

- **🎯 Jeu Libre** — Choisis ta difficulté et joue sans pression. Les 2 premiers niveaux sont ouverts à tous ; les 3 niveaux supérieurs sont **réservés aux holders $FRANC**.
- **🏆 Compétition** — **Réservé aux holders $FRANC**. Enchaîne les niveaux avec 3 vies, gagne des **$FRANC virtuels** et grimpe dans le TOP 3.

### Difficultés

| Niveau | Cases | Couleurs | Essais | Doublons | Accès |
|--------|:-----:|:--------:|:------:|:--------:|-------|
| ⭐ Très Facile | 4 | 6 | 12 | non | Tous |
| ⭐⭐ Facile | 4 | 6 | 10 | oui | Tous |
| ⭐⭐⭐ Moyen | 5 | 7 | 10 | oui | 🔒 Holders |
| ⭐⭐⭐⭐ Dur | 5 | 8 | 9 | oui | 🔒 Holders |
| ⭐⭐⭐⭐⭐ Très Dur | 6 | 8 | 9 | oui | 🔒 Holders |

### Système de points $FRANC (mode Compétition)

- Banque de départ : **200 $FRANC** (une seule fois, jamais négative)
- Code cassé : **+600 $FRANC**
- Indice : **−200 $FRANC** (max **2 par partie**, révèle une case du code)
- Le **TOP 3** est classé selon les $FRANC gagnés sur une partie

> 💡 Les $FRANC du jeu sont **virtuels** (score interne) et n'ont aucune valeur monétaire.

---

## 🌍 Langues

Français 🇫🇷 / Anglais 🇬🇧 — bascule via les drapeaux, préférence mémorisée.

---

## 📂 Contenu du dépôt

```
Mastermind/
├── index.html        ← le jeu complet (HTML + CSS + JS + images intégrées en base64)
├── README.md         ← ce fichier
├── DEPLOIEMENT.md     ← guide pas-à-pas GitHub Pages + Telegram BotFather
├── LICENSE           ← licence
└── .nojekyll         ← désactive le traitement Jekyll de GitHub Pages
```

Tout tient dans **un seul fichier `index.html`** : aucune dépendance à installer, aucune étape de build. Les 4 illustrations de Francis sont encodées directement dans la page.

---

## 🚀 Déploiement rapide

1. Crée un dépôt **public** nommé exactement `Mastermind` sous le compte `franclecoq`.
2. Verse les fichiers de ce dossier à la racine.
3. Active **GitHub Pages** (Settings → Pages → Branch `main` / dossier `/root`).
4. Le jeu sera en ligne sur **https://franclecoq.github.io/Mastermind** sous 1-2 minutes.
5. Configure la Mini App dans **@BotFather** vers cette URL.

👉 Étapes détaillées dans **[DEPLOIEMENT.md](DEPLOIEMENT.md)**.

---

## 🔗 Wallet / Holders

La détection des holders $FRANC réutilise l'infrastructure existante :

- Page de connexion wallet : `https://franclecoq.github.io/Wallet/connect-wallet.html`
- Vérification via le backend Supabase (`check-franc`), à partir de l'`initData` Telegram.

Aucune configuration supplémentaire n'est nécessaire si le bot et le backend sont déjà en place pour le Sudoku.

---

## 🛠️ Modifier le jeu

Tout est dans `index.html` :

- **Difficultés** → tableau `LEVELS`
- **Couleurs des pions** → tableau `COLORS`
- **Économie $FRANC** → constantes `HINT_COST`, `GRID_REWARD`, `MAX_HINTS`, et banque de départ dans `getFranc()`
- **Traductions** → objet `I18N` (clés `fr` / `en`)
- **URLs wallet / backend** → constantes `WALLET_PAGE` et `BACKEND`

---

🐓 *Cocorico !*
