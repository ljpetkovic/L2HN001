# Cultures numériques avancées (L2HN001)

### Informations pratiques

* Université Sorbonne Nouvelle, campus Nation
* Formation : mineure Humanités numériques, licence 1
* Enseignante : Ljudmila PETKOVIC 
* Semestre de printemps
* Salle : B011
* Horaire : mardi 10h-12h
* Matériel : https://icampus.univ-paris3.fr/course/view.php?id=34915

---

### Programme

`Cours 1-4` : [Ligne de commande](https://github.com/ljpetkovic/L2HN001/tree/main/1_Ligne_de_commande)

(à venir)

---

### Prérequis

* Pour les premiers cours, télécharger le dépôt, en cliquant sur `Code` > `Download ZIP` (plus tard nous allons apprendre comment *cloner* un dépôt et manipuler ses fichiers et ses répertoires)

* Pour exécuter les commandes Bash en ligne de commande sous Windows, il faut installer Microsoft Power Shell (le plus simplement est de télécharger le package `.zip` puis d'installer Power Shell → [tutoriel](https://learn.microsoft.com/en-us/powershell/scripting/install/installing-powershell-on-windows?view=powershell-7.3)).

  > Pour Linux Ubuntu, il suffit de taper `Ctrl + Alt + T` ou `terminal` dans le champ de recherche.
  >
  > Pour Mac, il suffit de taper `terminal` dans le champ de recherche (`Terminal.app`  dans `Applications` > `Utilitaires`)
  
* Pour autoriser l'exécution des scripts PowerShell sous Windows :

  * Cliquez sur le bouton **Démarrer** > **Tous les programmes** > **Accessoires** > **Windows PowerShell**.

  * Cliquez avec le bouton droit de la souris sur Windows PowerShell puis cliquez sur **Exécuter en tant qu'administrateur**

  * Dans la fenêtre qui s'ouvre, saisissez la commande suivante : `Set-ExecutionPolicy RemoteSigned` puis validez par **Entrée**.

  * Appuyez sur **O** et validez.

  * Vous pourrez désormais exécuter des scripts PowerShell sur votre ordinateur, par exemple :

     ```powershell
     ./mon_script.ps1 
     ```

* L'autre possibilité est de saisir la commande suivante lors de l'étape **3** : 

  ```powershell
  Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope CurrentUser
  ```

  puis de valider par **Entrée**, et de refaire les étapes **4.** et **5.**

  De cette manière, tous les scripts s’exécutent, mais ce niveau n’est pas du tout
  sécurisé ! si vous optez pour une alternative plus sécurisée, lancez :

  ```powershell
  Set-ExecutionPolicy -ExecutionPolicy Unrestricted -Scope CurrentUser
  ```

  (ou voir d'autres options, comme `Restricted`, `AllSigned` ou `Undefined`)

  Au besoin, cliquez sur le bouton **Démarrer**, tapez « **Autoriser l'execution de**
  **script** » et activer / appliquer l'option d'exécution des scripts (ou cherchez cette
  option dans votre **Espace développeur**)

---

### Citer ce dépôt

Ljudmila Petkovic, _Cultures numériques avancées (L2HN001)_, Paris : université Sorbonne Nouvelle, 2023 https://github.com/ljpetkovic/L2HN001

---

### Contact

ljudmila.petkovic[at]sorbonne-nouvelle.fr

---

### Licence

<img src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" alt="68747470733a2f2f692e6372656174697665636f6d6d6f6e732e6f72672f6c2f62792f322e302f38387833312e706e67" style="zoom:80%;" />

Ce travail est autorisé sous une licence [Creative Commons Attribution 4.0 International Licence](https://creativecommons.org/licenses/by-sa/4.0/deed.fr).

