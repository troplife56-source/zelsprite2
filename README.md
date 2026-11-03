# Zelscript — Action-RPG rétro (« La Relique Sacrée »)

Un mini Action-RPG rétro 2D en vue du dessus, inspiré des classiques de l'aventure, développé en JavaScript pur avec **Phaser 3**. Tout le jeu tient dans **un seul fichier HTML** : les graphismes et les sons sont générés par le code, sans aucun fichier externe.

**▶ Jouer en ligne : https://troplife56-source.github.io/zelsprite2/**

## 🎮 Le jeu

Un voleur a dérobé la relique sacrée du village. Parle au sage, explore la Crypte puis la Forge, vaincs deux boss et reprends la relique.

- **Un monde en grille 5×3** : 15 salles (village, Crypte, Forge, grotte, marais, salles au trésor) avec transitions de caméra et mini-carte.
- **Deux donjons, deux boss** : le **Gardien** de la Crypte (charge, rafales, coup au sol) et le **Golem de feu** de la Forge (anneaux de projectiles, boules de feu invoquées). Le Gardien scelle la route de la Forge.
- **Portes variées** : clé, dalle de pression, salle à vider, sceau de boss.
- **Bestiaire** : slimes, octoroks, chauves-souris rapides, chevaliers qui chargent après un flash rouge.
- **Boutique** : le marchand du village vend potion, flèches, épée forgée (dégâts ×2) et cœurs max. Les rubis servent enfin à quelque chose.
- **Progression** : réceptacles de cœur cachés (jusqu'à 8 cœurs), arc dans la grotte, trésors derrière une grille du marais.
- **Rejouabilité** : record de temps, score, et **Mode Héros** (ennemis renforcés, score ×2) débloqué à la première victoire.
- **Combat** : épée directionnelle avec coups critiques, knockback, invulnérabilité clignotante, arc, pièges (pics, boules de feu).
- **Aides** : objectif permanent, inventaire / pause, musique chiptune qui change selon le lieu.
- **Respect de la vie privée** : bandeau de consentement (Google Consent Mode) ; Analytics désactivé tant que le joueur n'accepte pas.
- **Sauvegarde automatique** : écran d'accueil **Continuer** / **Nouvelle partie**. Après une défaite, **Continuer** sur place (−25 points).

## 🕹️ Commandes

| Touche | Action |
|---|---|
| ZQSD / WASD / Flèches | Se déplacer (8 directions) |
| Espace | Coup d'épée |
| E | Interagir (parler, ouvrir un coffre, lire un panneau) |
| 1 à 4 | Acheter chez le marchand |
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
