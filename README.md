# elmarbouh_tp1
Mon premier projet
# TP1
Nom: EL MARBOUH
Prénom: RIDA
## Exercice 1:
Algorithme pin
var N,pin:entier
Début 
         N<-0
   tantque (N<3)faire 
        ecrire("enter voter code pin")
        lire(pin)
            si (pin=2007) alors
                    ecrireln ("succes")     
                    N<-N+4
                 sinon                      
                   ecrireln ("erreur")
                     N<-N+1
            finsi
    fintantque 
    si N=3 alors
        ecrireln("carte sim bloquée")
       sinon
         ecrireln ("au ravoir")
    finsi
FIN
## Exercice 2: