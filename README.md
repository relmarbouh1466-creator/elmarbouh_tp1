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
2. Conversion de températures
def convertir_temperature():
    print("--- Convertisseur de Température ---")
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
