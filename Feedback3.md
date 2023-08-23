# Feedback3

# 🕑Tic tac ! On veut aller trop vite ?

**C'est dommage car tu as fait du bon travail,** notamment du côté de ton StudentController, l'ajout d'un Etudiant se passe bien et ça c'est top 🔥 ! C'est une très bonne approche que de vouloir gérer tes méthodes GET/POST dans une même méthode de Controller, Bravo 👏 !

Malheureusement, commencer à avancer dans l'exercice alors que les bases du projet sont bâclées, ca peut te sembler être une bonne idée au début pour gagner du temps mais à terme ça peut se retourner contre toi en générant des erreurs qui n'ont rien à voir avec ce que tu développes au moment T et t'empêcher d'avancer correctement. On dirait bien que c'est ce qu'il s'est passé d'ailleurs 😢 !

**En début de projet, penses à bien prendre le temps de découper tes templates VIEW** afin d'avoir ton menu de navigation sur toutes tes pages et que ce soit plus fluide dans tes tests dès le début.

-   <u>Ce que cela t'apporte:</u>
    -   **De la duplication de code en moins** donc de possibles erreurs en moins. En tout cas, si il y en a une, elle ne sera à corriger qu'à un seul endroit !
    -   **Gain de temps**, tu n'as pas à recopier le header, la navigation etc... à chaque nouvelle page de ton site
    -   **Du code plus lisible** pour toi et les autres développeurs, tes templates "teacher" ou "student" ne sont consacrés qu'au code qui les concerne
-   <u>Cela te demande de:</u>
    -   **Mettre les bons require_once dans ton MainController.php** (ex: header.tpl.php, $viewname et footer.tpl.php)
    -   **Créer ces 3 templates dans un dossier qui pourrait s'appeler "layout"**. Pour les noms, c'est comme tu veux mais l'essentiel est que tu aies ce code qu'à un seul endroit comme ça si il y a une mauvaise URL sur un lien, cela se corrige à un seul endroit au lieu d'avoir à modifier tous tes fichiers !

* * *

## ✔Aide-toi de la correction pour:

-   **Remettre ton Front au propre,** tu dois pouvoir naviguer facilement sur ton site grâce à des templates bien organisés
-   **Remettre au propre l'ajout d'un Teacher** car tu as déjà tout ce qu'il faut, il y a juste des petites erreurs d'inattention sûrement suite à des copier-coller un peu trop hâtifs provenant de ton code Student:
    -   **Tu peux corriger le lien "ajouter" de ton teacher_list.tpl.php** qui envoi vers student/add au lieu de teacher/add
    -   **Corriger le code de ton TeacherController qui a une méthode studentAdd()** au lieu de teacherAdd(). Attention, il n'y a pas que le nom de méthode qui pêche… tu as laissé traîné de mauvais noms de variables et autre dans ta function !

☎ **Dis-moi quand c'est bon qu'on se fasse un call !** Si tu bloques, n'attends pas trop longtemps non plus, on regardera ensemble.

