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

Pour verifier s'il y a une `clé` dans le dictionnaire. 

```
'france' in europe # True
```

Pour enlever une `clé` il faut utiliser `del`
```
del(europe["france"])
```

## Dataframes

L'objet est similaire à une excel. Pour créer un Pandas DataFrame:

```
import pandas as pd

data = { .. }

df = pd.dataframe(data)
```

Quelques attributs importantes:

`ndim` : nombre de dimensions `# ex: 2`
`shape`: nombre d'éléments dans chaque dimension `# ex: (27, 4)`
`size` : nombre total d'éléments `# 108`

Deux méthodes pour afficher les premières ou dernières lignes de notre tableau.

```
df.head(n = 2) # montre deux premières lignes 
df.head(n = 3) # montre trois dernières lignes
```

L'objet Series sur pandas est liée à chacune des clés présents dans le dataframe `df`. Alors, si on veut extraire une colonne du dataframe, il suffit d'écrire: `col_pays = df['pays']`, avec `pays` comme un clé dans le dataframe. Ainsi, on peut accéder à la valeur de la "Series" `col_pays[23]` comme si c'est une liste ou un numpy.array.

On doit utiliser `.loc[]` pour accéder à une ligne de `df`, exemple: 
```
df.loc[23]
```

Pour savoir les **étiquettes des lignes** : `df.index`
Pour savoir les **noms de columns** : `df.columns`

Pour extraire des info dans une colonne par exemple: `df.loc[1:4, 'capitale']`. Il existe aussi `iloc[]`, `.at[]` et `.iat[]`.




