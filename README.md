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
        var3 <- var1
        var1 <- var2
        var2 <-? var3
    Ecrire("la valeur de var 1",var1)
    Ecrire("la valeur de var 2",var2)
FIN
## Exercice 3:
#qustion 1

ALGORITHME PGCD
Var a,b,rest: ENTIER
DEBUT
        ecrire("enter la valeur de prmier nomber a")       1
        lire(a)                                            1
        ecrire("enter la valeur de prmier nomber b")       1
        lire(b)                                            1
    tanque(b<>0) FAIRE                                     n
        reste <- a modulo b                                 2n
        a <- b                                              n
        b <- reste                                          n
    fintanque
    RETOURNER a                                            1
    ecrire("le PGCD enter a et b est",a)                   1
FIN                                        
#qustion 2

algorithme pgcd2
var a,b:ENTIER
Fonction PGCD(a, b):ENTIER
    Si b = 0 alors 
        Retourner a
    Sinon
        Retourner PGCD_Recursif(b, a mod b) 
    Fin Si
Fin Fonction
debut
        ecrire("enter la valeur de prmier nomber a") 
        lire(a)
        ecrire("enter la valeur de prmier nomber b")   
        lire(b)
        ecrireln("le PGCD enter a et b est",PGCD(a, b))
FIN
#qustion3
complexite de premier algorithme O(log(min(a, b)))
complexite de deuxieme algorithmeO(log(min(a, b)))
## Exercice 4:
Algorithme Diviseurs1
Variables :
    N,i : Entier
Début
    Écrire("Entrer un nombre :")
    Lire(N)
    Pour i de 1 à n Faire
        Si n mod b = 0 Alors
            Écrire(b)
        FinSi
    FinPour
Fin
Algorithme Diviseurs_Methode2
Variables :
    n, i : Entier
Début
    Écrire("Entrer un nombre :")
    Lire(n)
    Pour i de 1 à √n Faire
        Si n mod d = 0 Alors
            Écrire(d)
            autre ← n / d
            Si autre ≠ d Alors
                Écrire(autre)
            FinSi
        FinSi
    FinPour
Fin







