# Réponses — chasse au trésor

<!-- Format imposé, une réponse par ligne :
Q01: <réponse>
commande: <commande(s) utilisée(s)>
-->

Q01: 32
commande: git rev-list --count depart

Q02: c'est sarah Benali qui a editée la fonction formaterLigne 
commande: git blame -L :formaterLigne depart -- src/format.js


Q03: 4459c91715f9b1c97cf4776ad2e5afbdb3aa7051
commande:   git bisect start ; 
            git bisect bad depart ; 
            git bisect good v0.2.0 ; 
            git bisect run node scripts/controle-alertes.js

Q04: on obtient le contenu du fichier .env avant sa suppression, on peut donc voir que la variable d'environnement SECRET_KEY a été supprimée.
API_KEY = sk_live_01de6ba0c9f4d846

commande: git log --diff-filter=D --name-only --oneline depart puis git show 11544ab~1:.env 

Q05: Le SHA du commit qui a retiré le fichier est 11544ab
commande: git log --diff-filter=D --oneline depart -- .env

Q06: 17
commande: git rev-list --count v0.2.0..v1.0.O

Q07: commit
commande: git cat-file -t essai-perf (commande faite sur tous les tags)

Q08: experiment/cache-redis
commande: commande: git branch -r --no-merged depart puis git log --oneline --graph --all

Q09: src/utils.js
commande: git log --follow --name-status -- src/outils.js

Q10: 
commande: git shortlog -sn depart

Q11: 2026-03-24
commande: git show v1.0.0

Q12: feat(cli): bannière de démarrage
commande: git log --grep="revert" -i depart puis git log -1 --format=%s ceb6092 

Q13: de5637a
commande: git log --onelien --merges

Q14: la reponse est 16
commande: git diff --numstat v0.1.0 v1.0.0 -- src/stock.js

Q15: 6d6b920
commande: git log -S "TODO: gérer les quantités négatives" --oneline
