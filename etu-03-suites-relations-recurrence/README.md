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






