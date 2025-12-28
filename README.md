1. Mini-calculatrice

    print("Ma Mini-Calculatrice")
    try:
        num1 = float(input("Entrez le premier nombre : "))
        num2 = float(input("Entrez le deuxième nombre : "))
        print("\nOpérations disponibles : +, -, *, /")
        operation = input("Choisissez une opération : ")
        if operation == "+":
            resultat = num1 + num2
        elif operation == "-":
            resultat = num1 - num2
        elif operation == "*":
            resultat = num1 * num2
        elif operation == "/":
            if num2 == 0:
            return print("Erreur : Division par zéro impossible.")
            resultat = num1 / num2
        else:
        return print("Erreur : Opérateur invalide.")
        print(f"\nRésultat : {num1} {operation} {num2} = {resultat}")
