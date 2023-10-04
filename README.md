# EXERCICI 1
T1 = ["gener", "febrer", "març"]
T2 = ["abril", "maig", "juny"]
T3 = ["juliol", "agost", "setembre"]
T4 = ["octubre", "novembre", "decembre"]
meses = T1+T2+T3+T4
print(meses)

RDO: ['gener', 'febrer', 'març', 'abril', 'maig', 'juny', 'juliol', 'agost', 'setembre', 'octubre', 'novembre', 'decembre']

# EXERCICI 2
# segundo mes del primer trimestre
n1 = T1 [1]
print (n1)

RDO: febrer

# meses del primer mes
n2 = meses [ :3]
print (n2)

RDO: ['gener', 'febrer', 'març']

# acceder a septiembre y octubre
sept = meses[8]
oct = meses [9]
print (sept)
print (oct)

RDO: setembre
octubre

#EXERCICI 3
# llista amb nombres desordenats
lista = [ 3, 6, 7, 10, 45, 67, 4, 7, 89, 5, 67, 56, 3, 5, 90]
# numeros de la llista
print(len (lista))

RDO: 15
#quantes vegades apareix el numero 3
x = lista.count (3)
print (x)

RDO: 2

# quantes vegades apareix el numero 3 i 5
n3 = 0
n5 = 0
for numero in lista:
    if numero == 3:
        n3 += 1
    elif numero == 5:
        n5 += 1
print(n3, n5)

RDO: 2 2 

# quin es el numero mes gran
numeromax = max(lista)
print(numeromax)

RDO 90

# los 3 numeros mas pequeños
x = sorted (lista)
numeros_mas_pequeños = x [ :3]
print(numeros_mas_pequeños)

RDO: [3, 3, 4]

#quin es el rango de la llista. Es la dif entre valor max i min
x = max(lista)
y = min(lista)

rango = x -y
print(rango)

RDO: 87

# crear diccionari
compra =  {
    "pomes": {"qty": 5, "eur": 0.42},
    "peres": {"qty": 3, "eur": 0.66}
}
print(compra)

RDO {'pomes': {'qty': 5, 'eur': 0.42}, 'peres': {'qty': 3, 'eur': 0.66}}

#afeguir una altre fruita
compra["taronges"] = {"qty": 8, "eur": 0.81}
print(compra)

RDO {'pomes': {'qty': 5, 'eur': 0.42}, 'peres': {'qty': 3, 'eur': 0.66}, 'taronges': {'qty': 8, 'eur': 0.81}}

#cuando cuestan las peras
total_peres = compra ["peres"]["qty"] * compra ["peres"]["eur"]
print(total_peres)

RDO 1.98

#quantes fruites s'han comprat en total
total_frutas = compra ["peres"]["qty"] + compra ["pomes"]["qty"] + compra ["taronges"]["qty"]
print(total_frutas)

RDO 16

# Quina es la fruita mes cara
x= max(compra, key=lambda fruta: compra[fruta]["eur"])
print(x)

RDO taronges



