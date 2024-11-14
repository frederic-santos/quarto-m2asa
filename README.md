Template Quarto pour les mémoires de Master 2 ASA
=================================================

Cette extension Quarto est un template respectant les normes de mise en forme pour les mémoires de Master Archéologie & Sciences pour l'Archéologie de l'Université de Bordeaux.
Elle réutilise le [template LaTeX](https://gitub.u-bordeaux.fr/fsantos/template-latex-m2-bgs) mis en ligne en 2021.

Voici [un exemple de PDF produit à l'aide de ce template](_manuscrit/memoire.pdf).

## Installer l'extension

Pour utiliser ce template, vous pouvez simplement télécharger ce répertoire et travailler directement sur les fichiers adéquats.
Cependant, la méthode recommandée est de créer un dossier sur votre ordinateur, d'y naviguer avec votre console système, et d'y exécuter la commande suivante :

```{bash}
quarto use template frederic-santos/quarto-m2asa
```

## Instructions spécifiques

* Dans le fichier `_quarto_yml`, éditer les métadonnées `title`, `author`, et possiblement aussi la succession de documents devant être compilés pour produire le manuscrit final (`chapters`). Laisser tout le reste de ce fichier inchangé.
* La partie "Introduction" du mémoire doit être rédigée dans le fichier `index.qmd`.
* Les autres parties doivent être rédigées dans les fichiers séparés (et numérotés) `01-materiel-methodes.qmd`, `02-resultats.qmd`, etc. Vous êtes libres d'ajouter davantage de fichiers/parties ou d'en changer les noms, du moment que vous répercutez bien ces changements dans l'entrée `chapters` du fichier `_quarto.yml`.
* Les références bibliographiques doivent figurer dans le fichier `references.bib`, au format BibTeX donc. Ces fichiers peuvent aisément être produits en exportant votre collection Zotero à l'aide du plug-in Zotero "BetterBibTeX".