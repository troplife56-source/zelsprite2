# Zelscript — Action-RPG rétro (« La Relique Sacrée »)

Un mini Action-RPG rétro 2D en vue du dessus, inspiré des classiques de l'aventure, développé en JavaScript pur avec **Phaser 3**. Tout le jeu tient dans **un seul fichier HTML** : les graphismes et les sons sont générés par le code, sans aucun fichier externe.

**▶ Jouer en ligne : https://troplife56-source.github.io/zelsprite2/**

## 🎮 Le jeu

Un voleur a dérobé la relique sacrée du village. Parle au vieux sage, explore le donjon et affronte le Gardien pour la récupérer.

- **Un donjon en grille 3×3** : 9 salles reliées par des couloirs, avec une transition de caméra fluide.
- **Le village** : un PNJ te donne ta quête (dialogue « machine à écrire »).
- **Combat** : épée directionnelle avec coups critiques, knockback, invulnérabilité clignotante, Slimes qui chargent et Octoroks qui tirent.
- **Décor destructible** : buissons et pots qui lâchent cœurs, rubis et flèches.
- **Énigmes** : une dalle de pression ouvre une grille, un coffre cache la clé de la porte scellée.
- **L'arc** : trouvé dans un coffre, il tire à distance et peut activer une dalle.
- **Pièges** : pics qui sortent du sol et boules de feu rebondissantes.
- **Boss** : le Gardien a une barre de vie, tire en rafales, frappe le sol (onde de choc) et enrage à mi-vie.
- **Aides** : objectif affiché en permanence, mini-carte des salles visitées, inventaire / pause.
- **Sauvegarde automatique** : la progression est enregistrée dans le navigateur ; l'écran d'accueil propose **Continuer** ou **Nouvelle partie**. Après une défaite, on peut aussi **Continuer** sur place (−25 points).

## 🕹️ Commandes

| Touche | Action |
|---|---|
| ZQSD / WASD / Flèches | Se déplacer (8 directions) |
| Espace | Coup d'épée |
| E | Interagir (parler, ouvrir un coffre) |
| F ou clic | Tirer à l'arc (une fois trouvé) |
| I ou Tab | Inventaire / pause |
| M | Couper / relancer la musique |
| Entrée | Continuer (après une défaite) |
| R | Recommencer (écran de fin) |

**Sur téléphone** : joystick virtuel à gauche, boutons ÉPÉE / ARC / AGIR à droite, plus INV et SON en haut.

## 🛠️ Lancement rapide

Aucune installation, pas de Node.js. Ouvre simplement `index.html` dans Chrome, Edge ou Firefox (connexion Internet nécessaire pour charger Phaser 3 depuis le CDN), ou joue directement via le lien ci-dessus.

## ⚙️ Technique

- **Moteur** : Phaser 3 (CDN), Arcade Physics, rendu pixel art net (`pixelArt: true`, mise à l'échelle FIT).
- **Audio** : Web Audio API, effets et boucle musicale chiptune générés par le code.
- **Architecture** : classes ES6 (`Player`, `Enemy`, `Boss`, `NPC`, `Chest`, `Door`, `Plate`, `Spikes`, `Fireball`, `Arrow`, `Projectile`, `Breakable`), deux scènes (`MainScene`, `HUD`), Y-sorting dynamique.
- **Statistiques** : le jeu envoie des statistiques anonymes (démarrage, progression) à Google Analytics. La sauvegarde reste uniquement dans le navigateur du joueur (`localStorage`).

## 📜 Licence

Projet libre et open-source réalisé dans le cadre d'un prototype de développement web rétro.
