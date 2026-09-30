# Réponses — chasse au trésor

<!-- Format imposé, une réponse par ligne :
Q01: <réponse>
commande: <commande(s) utilisée(s)>
-->

Q01: 
commande: 

Q02: c'est sarah Benali qui a editée la fonction formaterLigne 
commande: git blame -L :formaterLigne depart -- src/format.js


Q03: 
commande: 

Q04: on obtient le contenu du fichier .env avant sa suppression, on peut donc voir que la variable d'environnement SECRET_KEY a été supprimée.
API_KEY=sk_live_01de6ba0c9f4d846

commande: git log --diff-filter=D --name-only --oneline depart puis git show 11544ab~1:.env 

Q05: Le SHA du commit qui a retiré le fichier est 11544ab
commande: git log --diff-filter=D --oneline depart -- .env

Q06: 
commande: 

Q07: 
commande: 

Q08: experiment/cache-redis
commande: commande: git branch -r --no-merged depart puis git log --oneline --graph --all

Q09: 
commande: 

Q10: 
commande: git shortlog -sn depart

Q11: 
commande: 

Q12: feat(cli): bannière de démarrage
commande: git log --grep="revert" -i depart puis git log -1 --format=%s ceb6092 

Q13: 
commande: 

Q14: la reponse est 16
commande: git diff --numstat v0.1.0 v1.0.0 -- src/stock.js

Q15: 
commande: 
