# Exemples d'utilisation de Python pour l'analyse de données omiques

Vous pouvez manipuler en ligne avec Binder les notebooks proposés :

[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/pierrepo/python-omics-use-cases/master?urlpath=lab)


Vous trouverez dans le répertoire `notebooks` 3 notebooks Jupyter :

- `volcano_plot.ipynb` : construction d'un *volcano plot*, représentation graphique couramment utilisée lors de l'analyse de données omiques. Utilisation des bibliothèques *Matplotlib* et *Bokeh*.
- `fusion_données.ipynb` : fusion de deux jeux de données avec *Pandas*.
- `acp_recettes.ipynb` : analyse en composantes principales avec la bibliothèque *Scikit-learn*. Et cette fois, pas de données omiques ;-)


## Manipuler les notebooks localement (sur votre machine)

1. Installez miniconda dans un environnement de type Unix (WSL pour Windows, Mac OSX ou Linux)

2. Clonez le dépôt :
```
git clone https://github.com/pierrepo/python-omics-use-cases.git
```

3. Créez l'environnement conda :
```
cd python-omics-use-cases
conda env create -f binder/environment.yml
bash binder/postBuild
```

4. Activez l'environnement conda :
```
conda activate python-omics-use-cases
```

5. Lancez Jupyter Lab :
```
jupyter lab
```


## Licence

Le contenu de ce dépôt est sous licence libre BSD 3-clause. Pour plus d'informations, consultez le fichier [LICENSE](LICENSE.txt).