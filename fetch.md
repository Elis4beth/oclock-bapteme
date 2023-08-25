# fetch

La méthode fetch() permet d'envoyer des **requêtes HTTP de façon asynchrone (JS).** C'est à dire à un autre moment qu'à l'affichage de **ta page récupérée côté serveur (PHP)**.

Plus concrètement, cela permet par exemple:

-   **D'alléger les chargements des pages et éviter la page blanche** en retournant le strict minimum des données à afficher au début et en les chargeant petit à petit ensuite. Très utilise dans les très grosses applications web !
-   **De récupérer des données dont on avait pas besoin** à l'arrivée sur la page mais dont on a besoin suite à une action utilisateur

**<u>Exemple 1</u>: Alléger le chargement de page**

On a 3 Millions de professeurs sur la page /teachers, cela pourrait être très lourd à afficher dès le début. Gérer cette liste avec des fetch() pour les récupérer 10 par 10 via une pagination sera bien plus agréable et évitera un chargement de page blanche interminable !

**<u>Exemple 2</u>: Dynamiser et afficher des données suite à une action utilisateur**

On veut rendre ton formulaire d'ajout d'étudiant plus dynamique dans ton Challenge. On pourrait imaginer que lorsqu'on sélectionne un Professeur, on afficherait en dessous sa spécialisation en matière de Framework utilisé dans ses cours !?

<u>Voilà concrètement comment cela se passerait</u>:

1.  Ajout d'une **nouvelle route** dans _index.php_

![image.png](/images/media_fetch/image.png)

2.  Implémentation de teacherFramework() dans _TeacherController.php_
   
![image.png](/images/media_fetch/a6c7d516-d5d9-4779-ad1b-a94a86eddbcd_image.png)

5.  Préparation du formulaire dans _student_add.tpl.php_ avec :
    - **Un élément "frameworkField" qui nous permettra d'afficher le résultat** récupéré par notre appel fetch()
    - **L'appel à notre function javascript "OnSelectChange()"** sur l'événement onchange de notre select Professeur
      
![image.png](/images/media_fetch/9556e64d-109c-46ef-8a7b-fe9bc492e2d7_image.png)

6.  **Le plus important: Notre fetch(),** pour cette démonstration rapide, on le met directement dans le head de notre page donc _header.tpl.php_:
   
![image.png](/images/media_fetch/9a31f4b9-1939-468e-8b1f-e3636dd73d8d_image.png)

8.  Et Voilà ! Cela fait qu'**à chaque changement de Professeur** dans le select "Prof", **on récupère le nom d'un Framework** qu'on affiche juste en dessous.
   
![image.png](/images/media_fetch/19baefba-c481-4885-84a5-94ee6ff5915d_image.png)

## 👩‍🍳La petite astuce du Chef

<u>Très pratique quand on travaille avec des fetch():</u>

Dans le F12 (inspection de code) de ton navigateur web, tu as un onglet "Network" ou "Réseau" qui te permet de suivre l'ensemble des requêtes envoyées, dont fetch() !

C'est un outil très pratique quand il s'agira de débug, tu verra !

![image.png](/images/media_fetch/84c8c19e-c7ad-4640-a014-c8a5bfa8c62b_image.png)

