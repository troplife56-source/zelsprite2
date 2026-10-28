Zelscript — Action-RPG rétro (Phase 3) Un mini Action-RPG rétro 2D inspiré des classiques de l'aventure, développé entièrement en JavaScript pur ( Phaser 3 ) et HTML5 Canvas. Le jeu fonctionne dans un fichier HTML unique, sans aucun serveur local ni actif externe (les graphismes et les sons sont générés à la volée par le code).

🎮 Aperçu du gameplay Explorez un monde fantastique divisé en plusieurs salles, interagis avec les villageois, équipe ton épée, résous des énigmes avec des clés et affronte le Gardien final dans son donjon !

Salle 1 (Village) : Une zone de départ paisible. Parle au vieillard pour recevoir ta quête et casser les décors.

Salles 2 & 3 (Exploration & Combat) : Affrontez des Slimes et des Octoroks à distance, détruisez les buissons/pots pour looter des cœurs et des rubis, et trouvez la clé cachée dans un coffre.

Salle 4 (Donjon du Boss) : Déverrouillez la porte scellée et affronte le Gardien blindé pour récupérer la relique sacrée et remporter la partie !

🕹️ Commandes et contrôles Touché Action ZQSD / WASD / Flèches Se déplacer (fluide à 8 directions) ESPACE Donner un coup d'épée E Interagir (parler au PNJ, ouvrir un coffre, lire des indices) Je suis ou TAB Ouvrir / Fermer le menu d'inventaire et mettre le jeu en pause M Couper ou relancer la musique chiptune de fond Entrée ou Clic Rejouer (sur l'écran de Game Over / Victoire)

🛠️ Lancement Rapide (Installation) Aucune installation complexe ni Node.js requise !

Enregistrez le code source sous le nom de index.html.

Double-cliquez sur le fichier pour l'ouvrir dans votre navigateur web ( Chrome, Edge ou Firefox ).

Note : Une connexion Internet est nécessaire au premier lancement pour charger la bibliothèque Phaser 3 via le CDN officiel.

⚙️ Caractéristiques Techniques Moteur : Phaser 3 (via CDN)

Audio : Web Audio API (effets sonores procéduraux et boucle musicale chiptune dynamique sans fichiers audio externes).

Rendu Pixel Art : Optimisé avec pixelArt: trueet le filtre CSS image-rendering: pixelatedpour un rendu net et rétro sans flou.

Architecture : Code modulaire en classes ES6 (Joueur, Ennemi, Boss, PNJ, Coffre, Porte, HUD) séparé en deux scènes (MainSceneet HUD).

📜 Licence Projet libre et open-source réalisé dans le cadre d'un prototype de développement web rétro.
