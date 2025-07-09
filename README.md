## Ce que ce module fait

 
Ce projet est comme le core des projets de la CdPVD.

Il contient 
<ol>
<li>Les interfaces.
<li>Les staging
<li>Les features
<li>Les dimentions
</ol>
 Par système de la Grics



##Création de l’environnement Fabric

<ol>
<li>Aller sur le site : https://app.fabric.microsoft.com/

<li>Cliquez sur votre photo à droite, puis sur suivez les instructions du site : Capacité d’essai de Fabric - Microsoft Fabric | Microsoft Learn


<li>Configurations supplémentaires
Il faut aller activer des fonctionnalités à partir du site : Fabric

<li>Allez activer les éléments suivants (a votre choix, pour l’ensemble de l’organisation ou pour des utilisateurs ou pour des groupes Entra)

<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="image/image1.png" alt="Logo" width="300"/>
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="image/image2.png" alt="Logo" width="300"/>
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="image/image3.png" alt="Logo" width="300"/>
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="image/image4.png" alt="Logo" width="300"/>
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="image/image5.png" alt="Logo" width="300"/>

</ol>





##Pour implanter les solutions de la CDPVD

Il faut premièrement mettre en place le core créé spécifiquement pour un environnement Fabric.

<ol>
<li>Dans votre Fabric, créez un espace de travail et nommez le "Core_Fabric" (ce nom n’est pas une suggestion, il faut vraiment créer cet espace avec ce nom).
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="image/image_1.png" alt="Logo" width="300"/>


<li>Une fois l’environnement créé, dans le haut à droite, cliquez sur "Paramètres de l’espace de travail"

 <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="image/image_2.png" alt="Logo" width="300"/>


<li>Allez sur Intégration de Git et sélectionnez GitHub
 
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="image/image_3.png" alt="Logo" width="300"/>

<li>Suivez les étapes pour se connecter sur GitHub. Il est possible que vous ayez à créer un Token (Personal Access Tokens (Classic))
Petit point, on vous suggère d’utiliser le même code utilisateur que votre code Office 365.

<li>Une fois connecté sur Git, inscrivez le repo : GitHub - CDPVD/core_fabric, sur la branche main.
 
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="image/image_4.png" alt="Logo" width="300"/>

<li>En cliquant sur "Connexion et synchronisation" tout le nécessaire pour faire fonctionner les interfaces de Paie.

<li>Dans le dossier "Interfaces" allez dans la bibliothèque de variable
 <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="image/image_5.png" alt="Logo" width="300"/>


<li>Allez remplacer la valeur de la variable "Paie" par votre ID. (voir prochaine étape pour savoir où trouver le bon ID)

 <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="image/image_6.png" alt="Logo" width="300"/>

<li>Pour trouver le bon ID à mettre, allez dans la configuration de vos connexions dans votre Gateway (Fabric)

<li>Trouvez la connexion qui se réfère à votre serveur SQL de votre système Paie. Allez dans les paramètres et allez copier l’ID
 
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="image/image_7.png" alt="Logo" width="300"/>


<li>Tester si le tout fonctionne correctement en allant dans le dossier "Interfaces" puis "Paie". Allez dans le "Pipeline" qui se nomme "pl_paie"
 
<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="image/image_8.png" alt="Logo" width="300"/>

<li>Une fois dans le Pipeline, cliquez sur "Exécuté". Si tout s’exécute correctement, dans le bas, vous aurez la mention opération réussie pour chacune des étapes (une étape étant une interface).

<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="image/image_9.png" alt="Logo" width="300"/>


</ol>
