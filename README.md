Travail à faire :Créer un Microservice Spring boot Multi Connecteurs SOAP, REST, GRAPHQL qui permet de
gérer des comptes:
![image](https://user-images.githubusercontent.com/97363124/210270251-4b73691f-f755-4026-a0fd-90d530b02a21.png)

1. Créer un Web service qui permet de :
• Convertir un montant de l’auro en DH
• Consulter un Compte
• Consulter une Liste de comptes
2. Déployer le Web service avec un simple Serveur JaxWS
3. Consulter et analyser le WSDL avec un Browser HTTP
4. Tester les opérations du web service avec un outil comme SoapUI ou Oxygen
5. Créer un Client SOAP Java
6. Créer un Client SOAP Dot Net
7. Créer un Client SOAP PHP
8. Déployer le Web Service dans un Projet Spring Boot
1. Création du Web service « BanqueWS » : 
![image](https://user-images.githubusercontent.com/97363124/210270396-eb1b3a55-5508-47dc-80a4-419293f9f539.png)
2. Déployer le Web service « BanqueWS» : Créer mon propre serveur http JaxWS qui permet d’accéder au web service « BanqueService »
![image](https://user-images.githubusercontent.com/97363124/210270443-9d8b9519-e813-4c2d-a72c-b9933511f935.png)
3. Visualiser le WSDL avec un Browser HTTP :
WSDL c’est un fichier xml qui permet de faire la description de web service dont on trouve les
méthodes et leurs entrées/sorties …
![image](https://user-images.githubusercontent.com/97363124/210270482-6331826a-53b6-48cd-b80b-1671485f452f.png)
Le schéma XML se compose essentiellement de déclarations d'éléments et d'attributs et de
définitions de types de chaque fonctions et attributs du service web « BanqueWS »
![image](https://user-images.githubusercontent.com/97363124/210270525-d7833b7e-93ad-4e11-b543-ea7a158d9e8d.png)
4. Tester le Web Service de type SOAP en utilisant SoapUI :
➢ Tester la méthode « convert » de web service SOAP
![image](https://user-images.githubusercontent.com/97363124/210270557-2de558e9-6213-4e32-a22c-c556f54f1c65.png)
➢ Tester la méthode « getCompte » de web service SOAP
![image](https://user-images.githubusercontent.com/97363124/210270660-3cf14d85-4022-4dea-9394-042400805c01.png)

➢ Tester la méthode « listCompte » de web service SOAP
![image](https://user-images.githubusercontent.com/97363124/210270645-dc2c333e-5a81-4a48-ac05-094195a8cf42.png)

5. Création d’un Client SOAP Java :
![image](https://user-images.githubusercontent.com/97363124/210270628-493d6cc2-e6ba-40e8-8dcf-c035ed7fca94.png)



Résumé
1) Le client demande au stub de faire appel à la méthode conversion(12)
2) Le Stub se connecte au Skeleton et lui envoie une requête SOAP
3) Le Skeleton fait appel à la méthode du web service
4) Le web service retourne le résultat au Skeleton
5) Le Skeleton envoie le résultat dans une la réponse SOAP au Stub
6) Le Stub fournie lé résultat au client
