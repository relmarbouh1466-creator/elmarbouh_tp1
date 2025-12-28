calc.py
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
conversion.py
    print(" Convertisseur de Température ")
    print("1. Celsius vers Fahrenheit/Kelvin")
    print("2. Fahrenheit vers Celsius/Kelvin")
    choix = input("Votre choix (1 ou 2) : ")
    try:
        if choix == "1":
         c = float(input("Température en Celsius : "))
         f = c * 9/5 + 32
         k = c + 273.15
         print(f"\n{c}°C = {f}°F = {k}K")
        elif choix == "2":
         f = float(input("Température en Fahrenheit : "))
         c = (f - 32) * 5/9
         k = c + 273.15
            print(f"\n{f}°F = {c}°C = {k}K")
        else:
            print("Choix invalide.")
texte.py
    phrase = input("Entrez un mot ou une phrase : ")
    majuscules = phrase.upper()
    minuscules = phrase.lower()
    inverse = phrase[::-1]
    longueur = len(phrase)
    nettoye = phrase.replace(" ", "").lower()
    est_palindrome = nettoye == nettoye[::-1]
    print(f"\n Analyse de '{phrase}' ")
    print(f"Longueur      : {longueur} caractères")
    print(f"Majuscules    : {majuscules}")
    print(f"Minuscules    : {minuscules}")
    print(f"Inversé       : {inverse}")
    print(f"Palindrome ?  : {'Oui' if est_palindrome else 'Non'}")
    print("\n Note sur l'immuabilité")
    print(f"La variable originale est toujours : '{phrase}'")
    print("En Python, les strings sont immuables. 'phrase.upper()' ne change pas")
    print("la variable 'phrase', mais crée une NOUVELLE chaîne en mémoire.")
