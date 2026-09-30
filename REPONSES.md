# Réponses — chasse au trésor

<!-- Format imposé, une réponse par ligne :
Q01: <réponse>
commande: <commande(s) utilisée(s)>
-->

Q01: 32
commande: git rev-list --count depart

Q02: 
commande: 

Q03: 4459c91715f9b1c97cf4776ad2e5afbdb3aa7051
commande:   git bisect start ; 
            git bisect bad depart ; 
            git bisect good v0.2.0 ; 
            git bisect run node scripts/controle-alertes.js

Q04: 
commande: 

Q05: 
commande: 

Q06: 17
commande: git rev-list --count v0.2.0..v1.0.O

Q07: commit
commande: git cat-file -t essai-perf (commande faite sur tous les tags)

Q08: 
commande: 

Q09: src/utils.js
commande: git log --follow --name-status -- src/outils.js

Q10: 
commande: 

Q11: 
commande: 

Q12: 
commande: 

Q13: 
commande: 

Q14: 
commande: 

Q15: 
commande: 
