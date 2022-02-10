# etu-03-suites-relations-recurrence

## `while`

```
while (3 > 2):
    # do something
```

Avec une variable `n` qui puisse varier, on peut arreter le flux d'exécution du cycle `while`.

```
n = 0

while n < 3:
    print("La valeur de n=" + str(n))
    n += 1
```

> Pour arreter le boucle `while`, lors d'une condition, il suffit d'ajouter l'instruction `break`. Mais ce n'est pas recommandé de l'utiliser assez souvent :'). C'est la programmation spaghetti.

## `for`

```
for i in range(5):
    print(i) # 0  1  2  3  4
```

Pour cela on utilise l'instruction `range(start, stop, step)`.

> Si on veut transformer un objet `range` en objet `list`

```
list(range(5))
```

On peut utiliser l'instruction `enumerate()` pour savoir l'indice de chaque élement.

> Pour itérer sur un dictionnaire `for k, v in dictionnaire.items():`. Avec `k` le mot clé et `v` sa valeur.

Pour numpy:

> Si on veut itérer sur tous les éléments d'un tableau 2D, on peut utiliser la fonction Numpy `np.nditer()`

Pour Pandas dataframe:

> Si on veut itérer sur un dataframe il suffit: `for label, row in df.iterrows():`, avec `label` comme l'indice de la ligne et `row` comme la valeur de toute la ligne.

Si on veut obtenir une colonne en particulaire, il faut par exemple dans l'itération: `row['colonne']`, avec `'colonne'` le nom de la colonne à filtrer.

On peut aussi filtrer avec `df.iteritems()` au lieu de `df.iterrows()`. ça va filtrer par colonnes.







