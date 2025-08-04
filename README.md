# La galerie en français pour `animint2`

[animint2](https://cran.r-project.org/web/packages/animint2/) est un package R pour la visualisation de données.
<!-- comment -->
Ce dépôt herberge [la galerie pour animint2](https://animint.github.io/gallery/), qui contient exemples de visualisations créées avec `animint2`.
Nous encourageons les contributions !

<!-- comment -->

## Comment contribuer

<!-- comment -->

### Créer une visualisation

<!-- comment -->

1. Utiliser `install.packages("animint2")` dans R pour installer la version actuelle du CRAN (>= 2023.11.21). Les versions récentes permettent l'option `source` pour la fonction `animint()`, qui est nécessaire pour publier une visualisation dans un galerie.
<!-- comment -->
2. Créer une visualisation `vis = animint(ggplots, title="titre", source="https://lien.vers/votre_code.R")` avec options :
<!-- comment -->
  * `title`: un titre ou description pour votre visualisation.
<!-- comment -->
  * `source`: l'URL du code source pour votre visualisation.
<!-- comment -->
3. Utiliser `animint2pages(viz, "ma_vis_dans_un_dépôt_github")` pour créer un nouveau dépôt avec votre visualisation dans la branch `gh-pages`. Voir les instructions détaillées dans [la partie GitHub Pages du Chapitre 5 du manuel pour animint2](https://rcdata.nau.edu/genomic-ml/animint2-manual/Ch05-sharing.html#pages).
<!-- comment -->
4. Faire un capture d'écran de votre visualisation, nommé `Capture.PNG`, et le rajouter dans la branche `gh-pages` du dépôt.

<!-- comment -->

### Rajouter votre visualisation au galérie

<!-- comment -->

En-dessous, SVP remplacer `VOTRE_PSEUDO_GITHUB` avec votre username sur GitHub.

<!-- comment -->

1. Si nécessaire, créer votre [copie (fork) du galérie](https://github.com/animint/gallery/fork). S'assurer que votre copie (fork) contient la branche `gh-pages`. Ceci fait une copie du galérie sur votre liste de dépôts sur GitHub.
<!-- comment -->
2. Si vous avez pas encore une copie (fork) local, SVP faire `git clone git@github.com:VOTRE_PSEUDO_GITHUB/gallery-fr ~/R/gallery-fr`. Ceci fait une copie (fork) dans votre ordinateur.
<!-- comment -->
3. Rajouter `VOTRE_PSEUDO_GITHUB/ma_vis_dans_un_dépôt_github` sur une nouvelle ligne dans `repos.txt`. S'assurer que `ma_vis_dans_un_dépôt_github` est le même nom que vous avez utilisé avec `animint2pages`.
<!-- comment -->
4. Faire `animint2::update_gallery("~/R/gallery-fr")` pour faire la mise à jour du galerie, et ensuite pousser les modifications vers la branche `gh-pages` de votre copie (fork) sur GitHub.
<!-- comment -->
5. Après quelques minutes, vos mises à jour s'affichent sur <https://VOTRE_PSEUDO_GITHUB.github.io/gallery-fr/>.
<!-- comment -->
6. Ouvrir une requête de tirage (pull request),

* depuis la branche `gh-pages` de votre copie (head/compare)
* avec destination la branche `gh-pages` du dépôt principal,  `animint/gallery-fr` (base)
* en cliquant "Contribute" sur le page GitHub de votre copie (fork),
* ou utiliser un URL comme <https://github.com/animint/gallery-fr/compare/gh-pages...VOTRE_PSEUDO_GITHUB:gallery-fr:gh-pages?expand=1>

<!-- comment -->
7. S'assurer que votre requête de tirage (pull request) contient

* un lien vers la version rendu de votre copie (fork) du galerie, par exemple <https://VOTRE_PSEUDO_GITHUB.github.io/gallery-fr/>, pour faciliter la relecture.
* un lien vers la nouvelle visualisation que vous proposer, par exemple <https://VOTRE_PSEUDO_GITHUB.github.io/ma_vis_dans_un_dépôt_github/>.

<!-- comment -->

Voir les instructions détaillées dans [la partie "Organizing animints in a gallery" du Chapitre 5 du manual pour animint2](https://rcdata.nau.edu/genomic-ml/animint2-manual/Ch05-sharing.html#gallery).
