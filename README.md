# Résillience (exercice)

### 1. Comment intégreriez-vous l'algorithme Raft au jeu des dames chinoises ? Quel est le rôle du leader ?

Pour implémenter le jeu de dames chinoise, chaque joueur est un client mais aussi un follower, ainsi, quand aucun leader
n'est disponible, un vote à lieu pour en désigner un.

Le leader aura pour rôle d'attendre l'action du joueur courant et le répliquer aux autre joueurs par le mécanisme de
Raft.