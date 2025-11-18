Template Quarto pour les mémoires de Master 2 ASA
=================================================

Ce template Quarto respecte les normes de mise en forme pour les mémoires de Master Archéologie & Sciences pour l'Archéologie de l'Université de Bordeaux.
Il réutilise le [template LaTeX](https://gitub.u-bordeaux.fr/fsantos/template-latex-m2-bgs) mis en ligne en 2021.

Voici [un exemple de PDF produit à l'aide de ce template](_manuscrit/memoire.pdf).

## Utilisation

Pour utiliser ce template, vous pouvez simplement télécharger ce répertoire et travailler directement sur les fichiers adéquats.

* Dans le fichier `_quarto.yml`, éditer les métadonnées `title`, `author`, et possiblement aussi la succession de documents devant être compilés pour produire le manuscrit final (`chapters`). Laisser tout le reste de ce fichier inchangé.
* La partie "Introduction" du mémoire doit être rédigée dans le fichier `index.qmd`. (Attention : ce fichier `index.qmd` ne gère donc pas la page de garde ; voir plus bas pour des détails à ce sujet.)
* Les autres parties doivent être rédigées dans les fichiers séparés (et numérotés) `01-materiel-methodes.qmd`, `02-resultats.qmd`, etc. Vous êtes libres d'ajouter davantage de fichiers/parties ou d'en changer les noms, du moment que vous répercutez bien ces changements dans l'entrée `chapters` du fichier `_quarto.yml`.
* Le contenu de la page de garde est géré dans le fichier `./tex/_titlepage.tex`. Ce dossier `./tex/` contient un certain nombre de fichiers au format LaTeX. La plupart n'ont pas à être modifiés directement ; seuls les fichiers `_titlepage.tex` (pour la page de garde) et `remerciements.tex` sont à éditer et à compléter par l'utilisateur final.
* Les références bibliographiques doivent figurer dans le fichier `references.bib`, au format BibTeX donc. Ces fichiers peuvent aisément être produits en exportant votre collection Zotero à l'aide du plug-in Zotero "BetterBibTeX".

Pour compiler le document final, les utilisateurs de Rstudio peuvent cliquer sur le bouton "Render book" de l'onglet "Build". (Raccourci clavier : Ctrl + Shift + B.)

## Ressources utiles

Quelques liens utiles pour apprendre Quarto :

- [Awesome Quarto](https://github.com/mcanouil/awesome-quarto), une impressionnante liste de ressources, tutoriels et exemples sur Quarto.
- Et bien sûr, [la documentation officielle](https://quarto.org/docs/guide/) !

## Support

Pour toute question ou signalement de bug, ouvrir un ticket de support (*Issue*) sur ce dépôt GitHub.
