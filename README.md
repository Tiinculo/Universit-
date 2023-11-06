# Università-
Es.1 30/10/2023

def bubble_sort( a ):
    n= len(a)

    for c in range(n-1):
        ordinata=True
        for i in range(n-1-c):
           if a[i]>a[i+1]:
               ordinata=False
               a[i], a[i+1] = a[i+1], a[i]
        # print(a)       
        if ordinata:
           return
        
x=input('inserire dei numeri')
a=x.split()
bubble_sort(a)
print(a) 

Es.2


def bubble_sort( a ):
    n= len(a)

    for c in range(n-1):
        ordinata=True
        for i in range(n-1-c):
           if a[i]>a[i+1]:
               ordinata=False
               a[i], a[i+1] = a[i+1], a[i]
        # print(a)       
        if ordinata:
           return

x=input('Inserisci la prima parola: ')
y=input('Inserisci la seconda parola: ')
x=list(x) #le stasformo in liste perche le stringhe non si possono modificare
y=list(y)
bubble_sort(x)
bubble_sort(y)

if x==y:
    print('Le due parole sono anagrammi ')
else:
    print('Le due parole non sono anagrammi ')
