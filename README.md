# kalkulator.py
Kalkulator napisany w Pythonie

Kod żródłowy:

# Program Kalkulator

# Tutaj definiujemy funkcje

def dodawanie(a, b):
    return a + b

def odejmowanie(a, b):
    return a - b

def mnozenie(a, b):
    return a * b

def dzielenie(a, b):
    return a / b

# Tutaj tworzymy pętlę while, która pozwoli użytkownikowi wybrać działanie.

while True:

    print("Wybierz działanie:")
    print("1. Dodawanie")
    print("2. Odejmowanie")
    print("3. Mnożenie")
    print("4. Dzielenie")
    print("5. Wyjście")
    wybor = input("Wybierz (1/2/3/4/5):")
    
    # Sprawdzamy, co wybrał użytkownik
    if wybor == '1':
        liczba1 = int(input("Wprowadź pierwszą liczbę: "))
        liczba2 = int(input("Wprowadź drugą liczbę: "))
        print(liczba1, "+", liczba2, "=", dodawanie(liczba1,liczba2))
    
    elif wybor == '2':
        liczba1 = int(input("Wprowadź pierwszą liczbę: "))
        liczba2 = int(input("Wprowadź drugą liczbę: "))
        print(liczba1, "-", liczba2, "=", odejmowanie(liczba1,liczba2))
    
    elif wybor == '3':
        liczba1 = int(input("Wprowadź pierwszą liczbę: "))
        liczba2 = int(input("Wprowadź drugą liczbę: "))
        print(liczba1, "*", liczba2, "=", mnozenie(liczba1,liczba2))
    
    elif wybor == '4':
        liczba1 = int(input("Wprowadź pierwszą liczbę: "))
        liczba2 = int(input("Wprowadź drugą liczbę: "))
        print(liczba1, "/", liczba2, "=", dzielenie(liczba1,liczba2))
        
    elif wybor == '5':
        break
    
    else:
        print("Błędny wybór!")
