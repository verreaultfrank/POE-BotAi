(NOT A REAL HOMEPAGE) 

Ce document servira à donner les grandes lignes directrices du projet de ai/bot pour path of exile.
- Github: https://github.com/verreaultfrank/POE-BotAi
- Trello: Demandez je vais vous add

-------------Idée générale pour le patern du bot-------------
1. Effectuer analyse du screen shot.
1.1 Si Rouge ataquer + mettre à jour carte
1.2 Si pas Rouge analyser mouvements via deux frames
2. Laisser le bot attaquer en fonction des infos qu'il possède


-------------Carte-------------
1. Se fier à  la map en haut en droit dun frame (analyser avec un réseau)
- On ajoute toujours les objets/monstres/obstacles


-------------D'étection mouvements-------------
1. S'inspirer du blog suivant https://github.com/nicholastoddsmith/poeai


-------------Personnage-------------
1. Évaluer sa vie et mana avec digits(analyse via reseau (utiliser le tuto tensorflow)) 
-La position en entrant dans une carte sera (0,0)


-------------Entrainement-------------
1. Feeder les info à un réseau qui outputera une décisions selons une action possible
- Verifier si il es possible d'optimiser une fonction de fitness(analyser la performance de différentes fonctions de fitness GENETIC ALGO)
- Params de fonction de fitness : vie, mana, shield, exp, temps d'exploration, dodging(how)
- Genetic algorith pour evolution du reseau de décision


-------------Bonnus(À implémenter si on a quelque chose de fonctionnel et que le projet est nice :D)-------------
1. Auto update gems
2. Auto skill points
3. Auto gearing
4. Auto skills seting
5. Auto selling/keeping stuffs
6. Training permanant si possible
7. Adapter à plusieurs résolution
8. Auto setting des params de poe pour que le bot fonctionnel
