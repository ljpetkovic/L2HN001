---
marp: true
theme: default
markdown.marp.enableHtml: true
paginate: true
extra: true
footer: "Cultures numériques avancées, mineure HN, 11/04/2023"
html: true

---

<style>
section {
  background-color: white;
  color: black;
}


h1 {
  color: DarkBlue;
}

h2 {
  color: DarkBlue;
}

h3 {
  color: DarkBlue;
}

h4 {
  color: DarkBlue;
}

h5 {
  color: DarkBlue;
}

h6 {
  color: DarkBlue;
  font-size: 30px;
  font-weight:normal;
}

blockquote {
  background: #ffedcc;
  border-left: 10px solid #d1bf9d;
  margin: 1.5em 10px;
  padding: 0.5em 10px;
}
blockquote:before{
  content: unset;
}

blockquote:after{
  content: unset;
}

small-text {
    font-size: 0.75rem;
  }

smaller-text {
    font-size: 0.5rem;
  }

</style>

<!-- _class: lead -->



 # Markdown

![bg left:40% 80% width:150pt height:100pt](https://www.defi-metiers.fr/sites/default/files/doc-kelios/Logo/2021/02/15/sorbonne_nouvelle-devise_bleu.jpg)

###### Ljudmila PETKOVIC

<br>





<small-text>

Cultures numériques avancées
Mineure « Humanités numériques »
Paris, le 11 avril 2023

<br>

<smaller-text>_Diapositives adaptées du [tutoriel Markdown](https://www.markdowntutorial.com/)_</smaller-text>



</small-text>

---

# Markdown

* langage de balisage (angl. _mark-up language_) et moyen d'écrire du contenu web
* écrit en texte brut (angl. _plain text_) : seulement les caractères contenus, sans leur apparence
  * seule une numérotation des caractères est utilisée, la police de caractères étant fournie par un mécanisme indépendant
  * Markdown utilise un alphabet normal, avec quelques symboles familiers, comme l'astérisques ( * ) et l'accent grave ( ` )


---

# Avantages de l'utilisation de Markdown

* Contrairement aux applications de traitement de texte encombrantes (p. ex. Word), le texte écrit dans Markdown peut être facilement partagé entre les ordinateurs, les téléphones mobiles et les personnes. → intéropérabilité
* Il devient rapidement la norme d'écriture pour les universitaires, les scientifiques, les écrivains et bien d'autres. 
  * Des sites Web comme [GitHub](https://github.com/) et [Reddit](https://www.reddit.com/) utilisent Markdown pour styliser leurs commentaires.
* Le formatage de texte dans Markdown a une courbe d'apprentissage très douce. Il ne change pas la taille, la couleur ou le type de police du texte (≠ CSS). 
  * Tout ce que vous contrôlez est l'affichage du texte, comme la mise en gras, la création d'en-têtes et l'organisation de listes.

---

# Italique et Gras

---

# Italique

Pour mettre un élément (mot, symbole...) en italique dans Markdown, il faut l'entourer d'un trait de soulignement (`_`) ou d'un asterisque (`*`). 

Par exemple, le mot `_italique_`  ou `*italique*` devient _italique_. 

```markdown
Voici comment écrire en _italique_. Ceci est également écrit en *italique*.
```

Résultat :

Voici comment écrire en _italique_. Ceci est également écrit en *italique*. 

---

# Gras

Entourer un élément de deux traits de soulignement ou de deux astérisques :

```markdown
Voici comment écrire en **gras**. Et voici encore un mot en __gras__.
```

Voici comment écrire en **gras**. Et voici encore un mot en __gras__.

---

## Italique ET gras

Placer les astérisques à l'extérieur et le trait de soulignement à l'intérieur, pour raison de lisibilité :

```markdown
Voici comment écrire en **_italique et gras_**.
```

Voici comment écrire en **_italique et gras_**.

---

# En-têtes

---

# En-têtes

* fréquemment utilisés sur les sites Web, les articles de magazines et les bulletins, pour attirer l'attention sur une section 
* agissent comme des titres ou des sous-titres au-dessus des sections

---

## Types d'en-têtes

6 types d'en-têtes, par tailles décroissantes :

* # En-tête 1

* ## En-tête 2

* ### En-tête 3

* #### En-tête 4

* ##### En-tête 5

* ###### En-tête 6 

---

# En-têtes

* Faire précéder un élément d'un signe dièse (`#`)

* Placer le même nombre de dièses que la taille de l'en-tête souhaitée
  * Par exemple, pour un en-tête 1, vous utiliserez un signe dièse 
    * `# En-tête 1`,
  * pour un en-tête 2, vous en utiliserez deux 
    * `## En-tête 2`,
  * et ainsi de suite.

---

# En-têtes

C'est à vous de décider quand il convient d'utiliser quel en-tête. 

En général, les en-têtes un et six doivent être utilisés avec parcimonie. 

Vous ne pouvez pas vraiment mettre un en-tête en gras, mais vous pouvez mettre certains mots en italique. 

```markdown
### Mon en-tête 3 _italicisé_
```

### Mon en-tête 3 _italicisé_

---

# Liens

---

# Liens

Créer des hyperliens vers d'autres sites Web dans Markdown

Deux types de liens différents dans Markdown, mais les deux s'affichent exactement de la même manière. 

1. liaison automatique (angl. *inline link*)
2. lien externe (angl. *reference link*)

---

# *Inline link*

Placez le texte du lien entre crochets (`[ ]`), puis le lien entre parenthèses (`( )`). 

Par exemple, pour créer un lien hypertexte vers https://github.com/, avec un texte de lien qui dit, « Cliquer ici », écrire : `[Cliquer ici](https://github.com/)`.

[Cliquer ici](https://github.com/)

---

## Formatage des liens

* Lien en gras :

  ```markdown
  Vous devez **[vraiment](https://github.com/)** cliquer ici
  ```

  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Vous devez **[vraiment](https://github.com/)** cliquer ici

* Lien en italique

  ```markdown
  Vous devez _[vraiment](https://github.com/)_ cliquer ici
  ```

  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Vous devez _[vraiment](https://github.com/)_ cliquer ici

* Lien dans le titre

  #### Mon [titre](https://github.com/)

---

## *Reference link*

Le lien est en fait une référence à un autre endroit du document.

```markdown
     Ceci est [un lien web][premier site web].
     Ceci est [un autre lien web][deuxième site web].
     Et maintenant nous revenons au [premier lien web][premier site web].

     [premier endroit]: www.github.com
     [deuxième endroit]: www.google.com
```

Ceci est [un lien web][premier site web].

Ceci est [un autre lien web][deuxième site web].

Et maintenant nous revenons au [premier lien web][premier site web].

[premier site web]: https://github.com/
[deuxième site web]: https://github.com/ljpetkovic/L2HN001

---

## *Reference link*

* Les « références » sont le deuxième ensemble de crochets : `[premier site web]` et `[deuxième site web]`. 

* Au bas d'un document Markdown, ces crochets sont définis comme des liens appropriés vers des sites web externes. 

* Un avantage de ce type de formatage est que plusieurs liens vers le même lieu ne doivent être mis à jour qu'une seule fois. Par exemple, si nous décidons de rediriger tous les liens `[premier site web]` ailleurs, nous n'avons qu'à changer le lien de référence unique. 

* Les liens de référence n'apparaissent pas dans le Markdown rendu. Vous les définissez en fournissant le même nom de balise entouré de crochets, suivi de deux-points, suivi du lien. `[premier site web]: https://github.com/`

---

# Images

---

# Images

Les images ont également deux styles, tout comme les liens, et les deux s'affichent exactement de la même manière. 

1. *inline image link*. 
2. *reference image link*

La différence entre les liens et les images est que les images sont précédées d'un point d'exclamation (`!`). 

Pour créer un *inline image link*, tapez un point d'exclamation (`!`), placez le texte alternatif entre crochets (`[ ]`), puis placez le lien entre parenthèses (`( )`). 

NB : Le texte alternatif est une expression ou une phrase qui décrit l'image pour les personnes malvoyantes, utilisant des lecteurs d'écran ou ne disposant pas de connexions Internet haut débit.

---

## *Inline image link*

Par exemple, pour créer un *inline image link* vers https://www.digitalocean.com/_next/static/media/intro-to-cloud.d49bc5f7.jpeg, avec un texte alternatif indiquant « Shell », écrire :

```markdown
![Shell](https://www.digitalocean.com/_next/static/media/intro-to-cloud.d49bc5f7.jpeg)
```

 ![Benjamin Bannekat](https://www.digitalocean.com/_next/static/media/intro-to-cloud.d49bc5f7.jpeg)

---

## *Reference image link*

Faire précéder le Markdown d'un point d'exclamation, puis fournir deux crochets pour le texte alternatif, puis deux autres pour la balise d'image, comme ceci : 

```markdown
![En-tête][markdown]
```

Au bas de la page Markdown, définir une image pour le tag : 

`[markdown]: https://raw.githubusercontent.com/sanity-io/sanity-plugin-markdown/HEAD/assets/example.png`

---

## *Reference image link*

```markdown
![En-tête][markdown]
```

`[markdown]: https://raw.githubusercontent.com/sanity-io/sanity-plugin-markdown/HEAD/assets/example.png`

![Prise de notes avec markdown][markdown] 

[markdown]: https://raw.githubusercontent.com/sanity-io/sanity-plugin-markdown/HEAD/assets/example.png

---

# Citations bloc

---

# Citations bloc

* une citation bloc est une phrase ou un paragraphe qui a été spécialement formaté pour attirer l'attention du lecteur

* pour attirer une attention particulière sur une citation d'une autre source ou pour concevoir une citation tirée d'un article de magazine, faites précéder la ligne du signe « supérieur à » (`>`), par exemple :

  ```markdown
  > « Je pense, donc je suis ».
  ```

  > « Je pense, donc je suis ».

  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(René Descartes)

---

## Formatage des citations bloc

* italique, gras et hyperlien

  ```markdown
  > « Etre libre, ce n'est pas pouvoir faire ce que l'on _veut_, 
  > mais c'est vouloir ce que l'on **peut**. » ([source](https://citations.ouest-france.fr/citation-jean-paul-sartre/etre-libre-pouvoir-faire-veut-19476.html))
  ```

  > « Etre libre, ce n'est pas pouvoir faire ce que l'on _veut_, 
  > mais c'est vouloir ce que l'on **peut**. » ([source](https://citations.ouest-france.fr/citation-jean-paul-sartre/etre-libre-pouvoir-faire-veut-19476.html))

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(Jean-Paul Sartre)

---

# Listes

---

# Listes

Deux types de listes : 

1. non ordonnée (avec des puces)
2. ordonnée (avec des chiffres)

---

## Liste non ordonnée

Faire précéder chaque élément de la liste d'un astérisque (`*`)

Chaque élément de la liste obtient également sa propre ligne. Par exemple, une liste de courses dans Markdown pourrait ressembler à ceci :

```markdown
* Lait
* Œufs
* Saumon
```

* Asperges
* Roquefort
* Gruyère

---

## Liste ordonnée

Une liste ordonnée est précédée de chiffres au lieu d'astérisques. 

Exemple : recette

```markdown
1. Bien égoutter les asperges et les disposer dans un petit plat à gratin.
2. Emietter le roquefort et le mélanger à la crème fraîche. Poivrer et saler.
3. Verser le mélange sur les asperges et répartir du gruyère pour faire gratiner.
4. Mettre l'ensemble au four à 180°C (thermostat 6) pendant 15 min environ.
```

1. Bien égoutter les asperges et les disposer dans un petit plat à gratin.
2. Emietter le roquefort et le mélanger à la crème fraîche. Poivrer et saler.
3. Verser le mélange sur les asperges et répartir du gruyère pour faire gratiner.
4. Mettre l'ensemble au four à 180°C (thermostat 6) pendant 15 min environ.

---

## Formatage des listes

Vous pouvez choisir d'ajouter des italiques, du gras ou des liens dans les listes.

Par exemple, mettons les noms latins des plantes en italique.

```markdown
* Azalea (_Ericaceae Rhododendron_)
* Chrysanthemum (_Anthemideae Chrysanthemum_)
* Dahlia (_Coreopsideae Dahlia_)
```

* Azalea (_Ericaceae Rhododendron_)
* Chrysanthemum (_Anthemideae Chrysanthemum_)
* Dahlia (_Coreopsideae Dahlia_)

---

# Listes imbriquées

Pour créer une liste plus approfondie, nous pouvons imbriquer une liste dans une autre. 

Indenter chaque astérisque d'un espace de plus que l'élément précédent (certains éditeurs, comme Typora, permettent de faire une tabulation). 

---

## Exemple des listes imbriquées

Par exemple, dans la liste suivante, nous allons ajouter une sous-liste au premier et au deuxième élément de la liste, ainsi qu'un autre élément imbriqué dans le deuxième élément imbriqué :

```markdown
* Mon premier élément de la liste
  * Un élément imbriqué dans le premier élément
* Mon deuxième élément de ma liste
  * Un élément imbriqué dans le deuxième élément
    * Un autre élément imbriqué dans le deuxième élément imbriqué
```

* Mon premier élément de la liste
  * Un élément imbriqué dans le premier élément
* Mon deuxième élément de ma liste
  * Un élément imbriqué dans le deuxième élément
    * Un autre élément imbriqué dans le deuxième élément imbriqué

---

## Listes avec des paragraphes

Bonne pratique : arrêter d'ajouter des sous-listes après trois niveaux pour raison de lisibilité.

Pour créer une liste nécessitant un contexte supplémentaire (mais pas une autre liste), le paragraphe doit commencer sur une ligne à lui tout seul sous la puce ou le chiffre, et il doit être indenté d'au moins un espace (ou alors, il faut faire un retour à la ligne et supprimer la nouvelle puce ou le nouveau chiffre) :

```markdown
1. Cassez trois œufs au-dessus d'un bol.   

 Maintenant, vous allez vouloir casser les œufs de manière à ne pas faire de dégâts. 
```

1. Cassez trois œufs au-dessus d'un bol.   

   Maintenant, vous allez vouloir casser les œufs de manière à ne pas faire de dégâts.  

---

### Convertir les puces en leurs propres paragraphes

```markdown
1. Couper le fromage   
   * Assurez-vous que le fromage est coupé en petits triangles.
2.  Trancher les tomates
   * Soyez prudent lorsque vous tenez le couteau.
```

1. Couper le fromage   
   * Assurez-vous que le fromage est coupé en petits triangles.
2. Trancher les tomates
   * Soyez prudent lorsque vous tenez le couteau.

---

# Paragraphes

---

# Paragraphes

* Pour créer une nouvelle ligne sans créer un nouveau paragraphe ou casser la liste qui le précède, il faut utiliser les *soft breaks* (`Shift + Entrée` ou en insérant deux espaces après chaque nouvelle ligne, selon l'éditeur).

  Exemple : poésie.

  Ne me quitte pas
  Il faut oublier 

* Ne pas confondre avec les _hard breaks_ (`Entrée/Retour`)

  Ne me quitte pas

  Il faut oublier

  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Jacques Brel, « Ne me quitte pas »

---

## Plusieurs paragraphes dans une liste

Rappelez-vous que nous avons inséré une nouvelle ligne (`Entrée`) pour plusieurs paragraphes dans une liste.

Au lieu d'utiliser des *hard breaks*, nous pouvons resserrer les sous-paragraphes avec des *soft breaks* :

```markdown
1. Cassez trois œufs au-dessus d'un bol.
 Maintenant, vous allez vouloir casser les œufs de manière à ne pas faire de dégâts. 
```

1. Cassez trois œufs au-dessus d'un bol.
   Maintenant, vous allez vouloir casser les œufs de manière à ne pas faire de dégâts.  

---

# D'autres types de formatage du texte

---

# D'autres types de formatage du texte

* Insérer trois tirets `---` pour séparer les diapositives ou les sections du texte

* Texte barré : `~~barré~~` : Ceci est mon texte ~~barré~~

* Texte souligné : `<ins>souligné</ins>` : Ceci est mon texte <ins>souligné</ins>

* Texte à l'intérieur de deux accents graves : `git add` (idéal pour des commandes simples)

* Texte à l'intérieur de trois accents graves, suivi par un retour à la ligne (idéal pour les bouts de code)

  ```
  git add README.md
  git commit -m "Mon README"
  git push
  ```

---

# Exercices

[Tutoriel Markdown](https://www.markdowntutorial.com)



