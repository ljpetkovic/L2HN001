---
marp: true
theme: default
markdown.marp.enableHtml: true
paginate: true
extra: true
footer: "Cultures numériques avancées, mineure HN, 24/02/2023"
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



 # Ligne de commande et Bash

### Récapitulatif

![bg left:40% 80% width:150pt height:100pt](https://www.defi-metiers.fr/sites/default/files/doc-kelios/Logo/2021/02/15/sorbonne_nouvelle-devise_bleu.jpg)

###### Ljudmila PETKOVIC

<br>





<small-text>

Cultures numériques avancées
Mineure « Humanités numériques »
Paris, le 24 février 2023

<br>

</small-text>

---

# Git Bash pour Windows

Pour exécuter les commandes et les scripts Shell sur Windows de même manière comme pour Mac / Linux (sans utiliser les commandes équivalentes pour Windows PowerShell), vous pouvez télécharger **Git Bash** ([tutoriel](https://www.simplilearn.com/tutorials/git-tutorial/git-installation-on-windows#git_installation_on_windows)) et l'utiliser en ligne de commande.

Nous allons utiliser le même logiciel dans le cadre des séances consacrées à l'utilisation du **Git**.

Pour s'assurer du bon fonctionnement du Git Bash, tapez :

```bash
git --version
```

![git_version](C:\Users\Utilisateur-P3\Downloads\1_Ligne_de_commande\git_version.png)

---

# Raccourcis pour copier-coller

Pour activer les raccourcis `Ctrl+Shift+C` (pour copier) et `Ctrl+Shift+V` (pour coller) :

1. Clique droite > `Options...`

2. Dans l'onglet Keys, cochez `Ctrl+Shift+letter shortcuts`

   ![copier-coller](C:\Users\Utilisateur-P3\Downloads\1_Ligne_de_commande\copier-coller.png)

---

# Tester toutes les commandes abordées jusqu'à présent

Pour chaque commande, vous trouverez :

* sa description
* ses options courantes (si elles existent)
* quelques exemples de son utilisation 

*L'objectif n'est pas de les mémoriser par cœur, mais de comprendre la logique de leurs leur fonctionnements.*

*Pour tous les autres détails, référez-vous aux diapositives des séances 1-4.*

---

##### `pwd`

* affiche le répertoire courant

* options courantes : aucune

  ```bash
  pwd
  ```

---

##### `ls`

* liste le contenu du répertoire courant ou d'un autre répertoire donné en paramètre

* options courantes : `-a`, `-l`

  ```bash
  ls
  ```

  ```bash
  ls -a
  ```

  ```bash
  ls -l
  ```

  ```bash
  ls -al
  ```

  ```bash
  ls commandes/
  ```

---

##### `cd`

* Change le répertoire courant

* options courantes : aucune

  ```bash
  cd ..
  ```

  ```bash
  cd commandes
  ```

  ```bash
  cd ../..
  ```

  ```bash
  cd Downloads/1_Ligne_de_commande/commandes
  ```

---

##### `help`

* Obtenir de l'aide sur le bash et sur les commandes internes (`pwd`, `ls`, `compgen`…)
* options courantes : `-d`, `-s`, `-m`
  * `-d` : description courte de la commande spécifiée
  * `-s` : synopsis de l'utilisation de la commande spécifiée
  * `-m` : pour formatter la sortie de la commande `help` comme un *manpage* (angl. *manual page*)

```bash
help
```

```bash
help pwd
```

```bash
help -d pwd
```

```bash
help -s pwd
```

```bash
help -m pwd
```

*Si la commande `help` ne couvre pas une commande qui vous intéresse, il suffit de taper le nom de cette commande, suivie par l'option `--help`*

````bash
ls --help
````

---

##### `cp`

* copie un fichier (ou un répertoire, si l'option `-r` est utilisée)

* options courantes : `-r`

  ```bash
  cp fichier_test.txt fichier_test_2.txt
  ```

  ```bash
  cp -r commandes commandes_2
  ```

---

##### `mv`

* déplace (ou renomme) un fichier ou un répertoire

* options courantes : aucune

  ```bash
  mv fichier_test_2.txt commandes
  ```

  ```bash
  mv commandes commandes_2
  ```

---

##### `rm`

* supprime un fichier (ou un répertoire, si l'option `-r` est utilisée)

* options courantes : `-r`

  ```bash
  rm fichier_test.txt
  ```

  ```bash
  rm -r commandes
  ```

---

##### `less`

* affiche un fichier en permettant la navigation, ainsi que certaines possibilités de l'éditeur de texte *vi* (p. ex. : la recherche)

  * pour quitter tapez `:q`

  ```bash
  less commandes/commande_1.sh
  ```

---

##### `touch`

* créé un fichier

  ```bash
  touch mon_script.sh
  ```

---

##### `nano` ou `vim`

* éditeurs de texte

  ```bash
  nano
  ```

  ```bash
  nano mon_script.sh
  ```

  ```bash
  vim mon_script.sh
  ```

  Ajouter un appel de script (*shebang*) suivi par votre script (p. ex. une commande)

  ```
  #!/bin/bash
  echo "Coucou"
  ```

  Sortir : `Ctrl+X`

  *Save modified buffer?* `y`

  *File Name to Write:* `mon_script.sh` (valider par Entrée)

---

##### `file`

* examine le type du fichier 

  ```bash
  file mon_script.sh
  ```

---

##### `mkdir`

* créé un répertoire

  ```bash
  mkdir test
  ```

---

##### `compgen`

* affiche toutes les commandes disponibles ou les *alias*

* options courantes : `-c` (*attention, cela peut prendre un certain temps*), `-a`

  ```bash
  compgen -c
  ```

  ```bash
  compgen -a
  ```

---

##### `echo`

* affiche un message 

  * y compris les cas où une **variable** (p. ex.`$nom`) est contenue dans une chaîne de caractères) 

* ou les résultats d'autres commandes

  ```bash
  echo "Coucou René"
  ```

  ```bash
  echo "Coucou $nom"
  ```

---

##### `grep`

* recherche une chaîne de caractères dans des fichiers 

* options courantes : `-E`, `-o`, `-i`

  ```bash
  grep "ordinateur" fichier_test.txt
  ```

  ```bash
  grep -Eoi "\bm\w+" fichier_test.txt
  ```

---

##### `bash`

* exécute un script *Shell* (avec l'extension `.sh`)

  ```bash
  bash mon_script.sh
  ```

* la commande `bash` peut être enlevée :

  ```bash
  ./mon_script.sh
  ```

  <smaller-text>Si vous obtenez un message d'erreur : `bash: ./mon_script.sh: Permission non accordée`, il faut donner au fichier la permission d'exécution (le rendre exécutable) en tapant `chmod +x mon_script.sh`</smaller-text>

---

##### `read`

* lit une ligne et stocke son contenu dans la variable `$REPLY`

* options courantes : `-p` (pour afficher un message spécifiant les attendus)

  ```bash
  read
  ```

  ```bash
  read -p "Comment t'appelles-tu ? "
  ```

  *Le terminal attend notre saisie : nous saisissons, p. ex. `Simon` et validons par Entrée*

  * Pour voir le message que nous avons saisi :

    ```bash
    echo $REPLY
    ```

---

# Exercice 1

1. Créer un script *Shell* :

   ```
   nano coucou.sh
   ```

2. Déclarer la variable `nom` avec la valeur `"Michel"`
   Imprimer le message `"Coucou Michel"` grâce à la variable créée :

   ```bash
   #!/bin/bash
   nom="Michel"
   echo "Coucou $nom"
   ```

3. Sauvegarder le script : ``Ctrl+X` > `y` > Entrée

4. Lancer le script :

   ```bash
   bash coucou.sh
   ```

---

# Exercice 2

1. Créer un script *Shell* :

   ```bash
   nano coucou_2.sh
   ```

2. Affiche la chaîne d'invite avant de lire l'entrée de l'utilisateur (qui sera stockée dans la variable `nom`), puis la réponse du terminal 

   ```bash
   #!/bin/bash
   read -p "Comment t'appelles-tu ? " nom
   echo "Hello $nom"
   ```

3. Lancer le script :

   ```bash
   bash coucou_2.sh
   ```