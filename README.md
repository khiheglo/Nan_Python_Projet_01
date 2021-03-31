# Nan_Python_Projet_01
Développement d'application Web avec Python - Projet n° 1

## EXERCICE 1
``` python
from random import randint

nbre = randint(1,100)
rep = int(input("Veuillez donner un nombre compris entre 1 et 100"))
cpt = 1

if rep != nbre:
    if rep < nbre:
        print("Le nombre saisi est trop petit")
    else:
        print("Le nombre saisi est trop grand")

    q = input("Voulez-vous continuer avec un autre nombre ? (O/N)")
    
    while (q != "N" or rep == nbre):
        rep = int(input("Veuillez donner un nombre compris entre 1 et 100"))
        cpt += 1
        if rep < nbre:
            print("Le nombre saisi est trop petit")
        elif rep > nbre:
            print("Le nombre saisi est trop grand")
        else:
            print(f"Félicitations vous avez reussi, après {cpt} tentative(s).")
            break
        
        q = input("Voulez-vous continuer avec un autre nombre ? (O/N)")
else:
    print("Félicitations vous avez reussi à la première tentative.")

```

## EXERCICE 2
``` python
def purge(chaine, caractere):

    rep = ""
    for c in chaine:
        if c != caractere:
            rep += c  
    return rep

```
