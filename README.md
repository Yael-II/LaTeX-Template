# LaTeX template v0
## [FR] Utilisation de mes fichiers LaTeX

Une nouvelle version est disponible.

### Liste des fichiers

Le repo contient les fichiers :
- yii.bst
- preambule_package.tex
- preambule_a4.tex
- s.tex
- fichiers modèles
- logotype d'exemple

### Utilisation
#### Cas général

Dans un premier temps, placer les trois fichiers préambules (`.tex`) dans un repertoire de votre choix (repertoire courant ou facilement accessible depuis la racine).

Pour utiliser les fichiers préambules, se référer aux modèles. Dans tous les cas, pensez à remplacer les lignes 4 et 5 avec les adresses de vos fichiers préambules :
```
\import{/CHEMIN/REPERTOIRE}{preambule_package}
\import{/CHEMIN/REPERTOIRE}{preambule_a4}
```
ainsi que l'adresse du logotype :
```
\includegraphics[height=2cm]{/CHEMIN/REPERTOIRE/logo.png}
```
le logo d'exemple étant évidemment à remplacer.

#### Avec bibliographie (facultatif)

Si vous souhaitez utiliser le style de bibliographie, placer ensuite le fichier `yii.bst` dans le repertoire courant ou `.../texmf-dist/bibtex/bst/base/`. Il faudra ensuite changer la ligne 54 du fichier `preambule_package.tex` :
```
\bibliographystyle{siam} %siam, yii
```
par :
```
\bibliographystyle{yii} %siam, yii
```
avant d'utiliser la commande `\bibliography{...}`. 

## [EN] Usage of my LaTeX Files

A new version is available.

### Files

Repo content:
- yii.bst
- preambule_package.tex
- preambule_a4.tex
- s.tex
- templates files
- example logotype

### Usage
#### General Case

First, place all the three preambule files (`.tex`) in your choosed directory (working directory or a directory easly accessible from the root).

To use the preambule file, please refer to the templates. In any case, replace lines 4 and 5 with the preambule files path:
```
\import{/PATH/DIRECTORY}{preambule_package}
\import{/PATH/DIRECTORY}{preambule_a4}
```
and the adress of the logotype:
```
\includegraphics[height=2cm]{/PATH/DIRECTORY/logo.png}
```
where the example logotype should be replaced.

#### With Bibliography (optional)

If you wish to use my bibliography, place the  `yii.bst` file in the working directory or in  `.../texmf-dist/bibtex/bst/base/`. Then, change line 54 from the file `preambule_package.tex`:
```
\bibliographystyle{siam} %siam, yii
```
with:
```
\bibliographystyle{yii} %siam, yii
```
before using `\bibliography{...}`. 
