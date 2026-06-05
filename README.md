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

🐓 *Cocorico !*
