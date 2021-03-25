# Exemples d'utilisation de Python pour l'analyse de données omiques

Vous pouvez manipuler les notebooks proposés en ligne avec Binder :

[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/pierrepo/python-omics-use-cases/master?urlpath=lab)


Vous trouverez dans le répertoire `notebooks` 3 notebooks Jupyter :

- `volcano_plot.ipynb` : construction d'un *volcano plot*, représentation graphique couramment utilisée lors de l'analyse de données omiques, dans cet exemple avec des données de protéomique. Utilisation des bibliothèques graphiques *Matplotlib* et *Bokeh*.
- `fusion_donnees.ipynb` : fusion de deux jeux de données avec *pandas*. Un premier jeu de données avec des résultats de protéomique et un second avec des descriptions de protéines provenant d'UniProt.
- `acp_recettes.ipynb` : analyse en composantes principales avec la bibliothèque *Scikit-learn*. Et cette fois, sans donnée omique ;-)


## Manipuler les notebooks localement (sur votre machine)

1. Installez miniconda dans un environnement de type Unix (WSL pour Windows, Mac OSX ou Linux)

2. Clonez le dépôt :
    ```
    git clone https://github.com/pierrepo/python-omics-use-cases.git
    ```

3. Déplacez-vous dans le répertoire du dépôt :
    ```
    cd python-omics-use-cases
    ```

4. Créez l'environnement conda :
    ```
    conda env create -f binder/environment.yml
    ```

5. Activez l'environnement conda :
    ```
    conda activate python-omics-use-cases
    ```

6. Chargez les extensions Jupyter Lab :
    ```
    bash binder/postBuild
    ```

7. Lancez Jupyter Lab :
    ```
    jupyter lab
    ```


Pour des utilisations ultérieures, seules les étapes 3, 5 et 7 seront nécessaires.


## Remarques pour les utilisateurs de Windows (sans WSL)

Si vous avez installé miniconda sur Windows avec le PowerShell (donc pas dans WSL), vous pouvez également installer cet environnement sur votre machine. 

Dans un premier temps, installez `git` si ce n'est pas déjà fait en exécutant cette commande dans un terminal :
```
conda install -c conda-forge git
```

Réalisez ensuite les étapes 2, 3, 4 et 5. 

Pour l'étape 6, exécutez, manuellement et l'une après l'autre, les commandes contenues dans le fichier `binder/postBuild` :
```
jupyter labextension install @jupyter-widgets/jupyterlab-manager
jupyter labextension install @bokeh/jupyter_bokeh
jupyter labextension install @jupyterlab/toc
```

Cette étape peut prendre du temps.

Terminez enfin par l'étape 7.


## Affichage de l'aide contextuel dans Jupyter Lab

Dans le *Launcher*, cliquez sur *Show Contextual Help*

![](notebooks/jupyter_lab_contextual_help.gif)


## Licence

Le contenu de ce dépôt est sous licence libre BSD 3-clause. Pour plus d'informations, consultez le fichier [LICENSE](LICENSE.txt).
