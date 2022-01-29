# etu-02-demarche-de-modelisation


## Dictionnaires

- Un dictionnaire est une collection de paires clé-valeur qui sont accessibles via leur clé, ils se ressemblent à une liste grâce à qu'ils sont capables d'stocker n'importe quel type de valeur.

```
{
    "key" : "valeur"
}
```

Par exemple si on veut trouver la valeur associé, dans un dictionnaire de pays et capitals:

```
europe = { "france" : "paris" }

print(europe["france"]) # "paris"
```

On peut utiliser la méthode `capitalize` pour changer la valeur:

```
print(europe["france"].capitalize()) # "Paris"
```