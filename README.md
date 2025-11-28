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
        var2 <- var3
    Ecrire("la valeur de var 1",var1)
    Ecrire("la valeur de var 2",var2)
FIN
## Exercice 3:
#qustion 1

ALGORITHME PGCD
Var a,b,rest: ENTIER
DEBUT
        ecrire("enter la valeur de prmier nomber a")       
        lire(a)                                            
        ecrire("enter la valeur de prmier nomber b")       
        lire(b)                                            
    tanque(b!=0) FAIRE                                     
        reste <- a modulo b                                 
        a <- b                                              
        b <- reste                                          
    fintanque
    RETOURNER a                                            
    ecrire("le PGCD enter a et b est",a)                   


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
complexite de deuxieme algorithme O(log(min(a, b)))
## Exercice 4:
#qustion 1
Algorithme Diviseurs1
Variables :
    N,i : Entier
Début
    Écrire("Entrer un nombre :")
    Lire(N)
    Pour i de 1 à n Faire
        Si (n mod i) = 0 Alors
            Écrire(i)
        FinSi
    FinPour
Fin
#qustion 2
Algorithme Diviseurs2
Variables :
    n, i : Entier
Début
    Écrire("Entrer un nombre :")
    Lire(n)
    Pour i de 1 à racineCarree(n) Faire
        Si n mod i = 0 Alors
            Écrire(i)
            A <- n / i
            Si A != i Alors
                Écrire(A)
            FinSi
        FinSi
    FinPour
Fin
#qustion 3
complexite de premier algorithme O(n)
complexite de deuxieme algorithme O(√n) 
## Exercice 5:
Algorithme JEUX
fonction aleatoire(debut,fin:entier):entier
var T,n;n3;x: entier
debut
    X <- aleatoire(1,100)
    T <- 0
    repeter
        tanque(T != 5 ) faire
            ecrire("choisi un nombre entre 1 et 100")
            lire(n)
         si n = X alors
            ecrire("felicitations")
            T <- 6
          sinon 
            T <- T-1
           si n < X ALORS
              ecrire ("trop petit")
             sinon
              ecrire ("trop grand") 
            finsi
         finsi
        fintanque
      ecrireln ("le nomber est :",aleatoire(1,100))
      ecrireln (" Voulez-vous rejouer? si oui tape 1")
      lire (n3)
     si n3 = 1 alors
      T <- 0
       sinon 
         ecrire("au revior")
     finsi
   jusque (T=5) 
fin
## Exercice 6 :
Algorithme TriangleFloyd
var n,m,i,j:entier
Début
    Écrire ("Donnez un nombre n : ")
    Lire (n)
    M ← 1
    Pour i de 1 à n faire
        Pour j de 1 à i faire
            Écrire (M," ")
            M ← M + 1
        FinPour
        ecrireln(" ")
    FinPour
Fin
la complexite: O(n²)
## Exercice 7 :
#qustion 1
ALGORITHME somme_des_entiers
     VAR nombre,s:ENTIER
debut
     ecrire("Donner un nombre: ")
     lire(nombre)
     s ← 0
     pour i de 1 à n:
     s ← s + i
     retourner s
     ecrire(" La somme est: ", s)
fin

#qustion 2
ALGORITHME somme_des_entiers
      VAR nombre,somme:ENTIER
      Fonction sommeEntier (n:ENTIER): ENTIER
            Si (n = 1 ) Alors
                  retourne  n
            Sinon
                  retourne  n + sommeEntier(n-1)
            Fin Si
      Fin Fonction

DEBUT
      
      ecrire("Donner un nombre: ")
      lire(nombre)
      somme <-- sommeEntier(nombre)
      ecrire(" La somme est: ", somme)
FIN
#qustion 3
complexite de premier algorithme O(n)
complexite de deuxieme algorithme O(n) 
 










