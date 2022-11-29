# Instal·lació Moodle

## Creem la màquina virtual

- El primer que farem serà posar com a xarxa l'adaptador pont i a emmagatzematge posarem la iso del Ubuntu Server. 
  ![image](https://user-images.githubusercontent.com/104194793/204559342-0ed97402-51c3-4f1d-999e-5e88dedc91ec.png)

  ![image](https://user-images.githubusercontent.com/104194793/204559563-5299ccb1-32c6-4a49-970b-471310bf0814.png)

## Instal·lació del Moodle

1. El primer que farem un cop instal·lada la màquina serà posar *ip a*, per així saber la ip de la nostra màquina.
  ![image](https://user-images.githubusercontent.com/104194793/204563025-d0f12bf5-834b-4a99-a906-a9ffdeb75f90.png)
  
2. Ara el que farem serà posar la comanda *ssh afolque@192.168.203.158*
  ![image](https://user-images.githubusercontent.com/104194793/204563522-01e259c6-70bb-42c5-876e-6df93a8d2463.png)

3. Un cop posada la comanda ssh afolque@192.168.203.158, instal·larem l'apache.
   ![image](https://user-images.githubusercontent.com/104194793/204564056-b962205b-f2e7-4606-b6b0-2070c8987aab.png)
   ![image](https://user-images.githubusercontent.com/104194793/204564238-e9ba08f8-5fdf-4d5b-804a-8b4eeb068067.png)

4. El següent serà instal·lar MariaDB.
  ![image](https://user-images.githubusercontent.com/104194793/204564497-c8d2e548-0bc1-439e-ae7f-d1c6f16c692d.png)

5. Un cop instal·lada MariaDB, instal·larem la configuració de seguretat de mysql.
  ![image](https://user-images.githubusercontent.com/104194793/204564764-413ca477-4864-4b64-be04-5f7fd251df2a.png)

6. Un cop instal3lada la configuració de seguretat de mysql, el que farem serà comprovar si podem entrar. 
  ![image](https://user-images.githubusercontent.com/104194793/204566076-96d0afc6-bd7d-47b3-b213-88556be00f5f.png)
  
7. Ara instal·larem el php7.3.

  ![image](https://user-images.githubusercontent.com/104194793/204568233-a5ec0a09-0cf7-4f21-86e0-1b608c969777.png)
  ![image](https://user-images.githubusercontent.com/104194793/204568423-b641a827-a884-4224-9fde-654d0e4b4a1b.png)

8. El següent que farem serà editar següent el fitxer per a que així ens mostri index.php, en compte de index.html.
  ![image](https://user-images.githubusercontent.com/104194793/204569746-56b5baa4-0d3c-4317-b9b3-a9f4f6cb1e80.png)
  ![image](https://user-images.githubusercontent.com/104194793/204570053-40ebb10f-189a-4f5e-bbcd-f32e4a8386f3.png)
  
9. Un cop editat aquest fitxer, reiniciarem el servidor apache per així guardar tots els canvis. 
  ![image](https://user-images.githubusercontent.com/104194793/204570530-17003a40-f234-4cc4-bfe4-06506c0f3ab7.png)

10. Per últim mirarelm l'estat del servidor. 
  ![image](https://user-images.githubusercontent.com/104194793/204570829-7f67ac02-8185-43a4-90c6-608ca8cf5ca3.png)

11. El següent que farem serà crear el fitxer index.php
  ![image](https://user-images.githubusercontent.com/104194793/204572462-f491741a-1111-4bb1-98f6-9fbde64a5b5e.png)
  ![image](https://user-images.githubusercontent.com/104194793/204572686-846ff5fd-9ca6-4535-a8ac-95429c817ec6.png)

12. A continuació instal·larem el moodle.
  ![image](https://user-images.githubusercontent.com/104194793/204573166-501df8d3-93b4-4f42-8e67-d19276085142.png)

13. Descomprimirem la carpeta. 
  ![image](https://user-images.githubusercontent.com/104194793/204573505-5742c94e-10ab-4c4f-8b61-3af1f5837c52.png)
  ![image](https://user-images.githubusercontent.com/104194793/204573838-3958d8cf-5098-4e89-b345-328a8131235c.png)

14. Canviarem els permisos.
  ![image](https://user-images.githubusercontent.com/104194793/204574086-f9dc51d4-d7b0-4e7d-a393-84be405f55be.png)

15. Entrarem al directori /home, crearem la carpeta *moodledata* i li donarem els permisos.
  ![image](https://user-images.githubusercontent.com/104194793/204574676-821efd95-881e-4628-bf1d-8f0ec2989fd4.png)

16. El següent que farem serà accedir a la base de dades amb el mode root.
  ![image](https://user-images.githubusercontent.com/104194793/204574904-4d7a9552-0a2b-49a9-b208-3e6dee2701d0.png)

17. Creem l'usuari *moodlemanager* dins de la base de dades.
  ![image](https://user-images.githubusercontent.com/104194793/204575253-a2331d1f-957f-449a-a236-2105f827b206.png)

18. Creem la base de dades del moodle.
  ![image](https://user-images.githubusercontent.com/104194793/204575473-40fe57d6-dcdf-482b-a0a5-cdfb4f245a66.png)

19. Donarem permisos a l'usuari.
  ![image](https://user-images.githubusercontent.com/104194793/204575729-b3c09218-6f09-4341-b6a4-819c9f91dbf3.png)
  ![image](https://user-images.githubusercontent.com/104194793/204575839-9f57b5c5-960d-45d2-bbc0-0cfbf05f175c.png)

20. Per últim anirem al buscador i posarem *la nostra ip*/moodle.
    ![image](https://user-images.githubusercontent.com/104194793/204576133-97ab855b-0a3f-4d3c-b167-b4ec8a5fb3f0.png)

  
  


