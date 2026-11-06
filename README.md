cisla = []

pocet = int(input("Koľko čísel chceš zadať? "))

for i in range(pocet):
    cislo = int(input("Zadaj číslo: "))
    cisla.append(cislo)

for i in range(len(cisla)):
    for j in range(i + 1, len(cisla)):
        if cisla[i] > cisla[j]:
            pomocna = cisla[i]
            cisla[i] = cisla[j]
            cisla[j] = pomocna

print("Zoradené čísla:", cisla)# Ine
