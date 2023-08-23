# Feedback4

## 🌊Tu t'es laissé submerger ?

**On dirait que tu n'as pas réussi les premières étapes du Challenge et que tu as quand même voulu avancer sur la suite** des exercices jusqu'à te faire submerger de problèmes et erreurs PHP, non ? C'est bien de ne pas t'être démonté et d'avoir voulu avancer mais malheureusement cela t'empêche peut être de valider des compétences importantes.

**Prends le temps de corriger tes erreurs PHP une par une avant de vouloir avancer trop loin.** Le code te parle et te dit ce qu'il ne va pas, il faut juste réussir à le comprendre.

## 👄 Lire et parler PHP

Des premières erreurs PHP que je rencontre, je peux déjà te dire que **tu dois être plus rigoureux** sur ce que tu écris et les nommages de tes fichiers, Controllers, function etc... Le code ne peut pas s'exécuter correctement si tu ne lui donne pas **les bons noms** ou si tu appelles des **éléments qui n'existent pas**.

Deux exemples:

-   Lorsque tu importes des fichiers, tu dois t'assurer que tu n'as pas fait d'erreur dans le nom et que **celui-ci existe bien** (ex: "MainController not found" dans index.php). Il s'agit de la première erreur affichée en arrivant sur ton site, c'est normal, tu utilise un MainController.php dans ton index.php alors que ce fichier n'existe pas dans le projet.
-   Tu es libre d'appeler tes Controllers comme tu le souhaites en restant un minimum cohérant avec la logique métier mais une fois que tu as choisi un nom, **il doit être identique partout** où tu l'utiliseras (ex: StudentsController.php qui est appelé plusieurs fois sans le "s" dans index.php ligne 108 et 118)
-   **De même pour le nom de tes variables !** Dans StudentsController.php ligne 21, tu utilise une variable que tu viens de créer en faisant une faute dans le nom, c'est dommage. N'hésite pas à faire des copier-coller pour éviter ce genre d'erreur ($studentsModel / $studentsdModel)

Ce sont 3 exemples parmi plusieurs autres, ce sont des erreurs que tu refais trop souvent !

☎**Je te propose un call pour:**

-   **Te débloquer et t'aider à apprendre à lire tes erreurs PHP.** Le but serait que tu sois plus à l'aise et capable de les comprendre par toi même pour les prochains Challenge !
-   **Afficher la liste des professeurs:** On regardera aussi ta méthode teachers() de TeachersController afin de faire ensemble cette partie du Challenge et s'assurer que tu aies compris les bases MVC dont tu aura besoin pour la suite

