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
algorithme var
var var1,var2,var3:entier
debut
    Ecrire("Entrez la valeur de la permier variable")
    lire(var1)
    Ecrire("Entrez la valeur de la deuxieme variable")
    lire(var2)
        var3←var1
        var1←var2
        var2←var3
    Ecrire("la valeur de var 1",var1)
    Ecrire("la valeur de var 1",var1)
FIN