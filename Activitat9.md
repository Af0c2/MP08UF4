# Copies de seguretat:

## Importància de les còpies de seguretat:

Quan treballem com administradors d'un servei ens hem de preocupar de com evitar que es perdin les dades o guardar-les per migrar-les a un altre servidor.

Per aquest motiu és important conèixer la informació necessària per poder recuperar el servei en cas d'error o migració.

També podem fer còpies de seguretat únicament de cursos per passar-los a un altre Moodle o crear un curs idèntic.

## Còpia de seguretat d'un curs:

![image](https://user-images.githubusercontent.com/110727546/212052894-c02acab1-3004-4a59-be6d-480c5457bb79.png)

![image](https://user-images.githubusercontent.com/110727546/212726727-6e23b7c5-566c-43d4-b634-22f19e80de9d.png)


Les còpies de seguretat d'un únic curs es fan des de'l mateix Moodle.

Serveixen per duplicar cursos, pasar informació i recursos d'un curs a un altre o migrar un curs a un nou servidor de Moodle.

[Tutorial a Moodle](https://docs.moodle.org/all/es/Respaldo_del_curso)
[Tutorial a Youtube](https://youtu.be/rH6DJ_lbMm0)

## Còpia de seguretat de tot Moodle:

Si volem migrar el servei o recuperar-lo hem de pensar quina informació estem utilitzant a Moodle i on està guardada.

### Pensem...

![image](https://user-images.githubusercontent.com/110727546/212053271-9d1305d7-af49-41a4-b6d5-846816c6bb69.png)
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
### Directori de Moodle: 

El directori amb els fitxers necessaris per què funcioni Moodle. A la nostra pràctica és a /var/www/html/moodle probablement.

### Directori de dades:

El directori on es guarden fitxers pujats pels usuaris/es de Moodle, com les pràctiques. A la nostra pràctica probablement estarà a /home/moodledata.

### Base de dades:

A la base de dades estaran guardades  les dades de cursos, usuaris, puntuacions... 

La forma de fer backup de la base de dades canviarà segons la bbdd que utilitzem.

### Possar-ho tot al lloc una altra vegada:

Després de recuperar tota aquesta informació caldrà ficar-la al nou servidor i comprovar que tot funciona bé.

### Tutorial de migració de Moodle:

[Tutorial a Moodle](https://docs.moodle.org/all/es/Migraci%C3%B3n_de_Moodle)

# Activitat:

L'activitat, que realitzareu per parelles, es divideix en dues pràctiques diferents, cadascuna amb el mateix valor:

## A1 - Backup i restauració de curs:

- Fareu una còpia de seguretat del vostre curs elaborat a Moodle.
  Anirem al curs de Programació en Python, anirem a la rodeta de dalt de tot i escollirem l'opció de còpies de seguretat. 
  ![image](https://user-images.githubusercontent.com/104194793/213736104-cb84b649-f347-438a-9b6a-2a101dd888ac.png)
  
  Escollirem el que volem que se'ns baixi en la còpia de seguretat. 
  ![image](https://user-images.githubusercontent.com/104194793/213738182-5571cf83-bb97-48dd-89a9-379aa729e2c2.png)
  
  Un cop escollit, li donarem al botó de FES LA CÒPIA.
  ![image](https://user-images.githubusercontent.com/104194793/213739351-94445b1c-404f-409d-b85c-417769c64940.png)
  
  Un cop completada ens sortirà aquest missatge.
  ![image](https://user-images.githubusercontent.com/104194793/213739697-8160a484-ac37-4027-8e08-84b865e0611e.png)

- Passareu el fitxer al server del company/a de grup.
  ![image](https://user-images.githubusercontent.com/104194793/213742407-a75971af-4059-4708-ae09-e20aeb26713c.png)
  ![image](https://user-images.githubusercontent.com/104194793/213742656-7d629b9d-9457-42c6-9e3d-f8f25a9b414a.png)

- Recuperareu el curs al seu Moodle.
  ![image](https://user-images.githubusercontent.com/104194793/213744979-eb11e0ca-7deb-46a3-864f-7542e6c93a82.png)
  ![image](https://user-images.githubusercontent.com/104194793/213745191-b945e21a-8d32-4824-8548-b72e721a9993.png)
  ![image](https://user-images.githubusercontent.com/104194793/213745313-40e06cf8-ad48-4cb8-9163-ba45f9e3587c.png)
  ![image](https://user-images.githubusercontent.com/104194793/215109715-9c8aeb39-8c1e-4097-9e9b-83f945cd0d06.png)
  ![image](https://user-images.githubusercontent.com/104194793/215110031-3c7628f3-3a7e-497b-89d2-08b6fb68f2ea.png)
  ![image](https://user-images.githubusercontent.com/104194793/215110155-4b8c1727-aa84-4081-92af-bda3fa1e60ce.png)
  ![image](https://user-images.githubusercontent.com/104194793/215110863-2c1ee557-0ade-4862-a4eb-d0c279b46cdb.png)
  ![image](https://user-images.githubusercontent.com/104194793/215110974-7426914f-4c40-45e0-891b-d9eafff13bc1.png)
  
  - Comprovareu que tot funciona correctament.
  
    
- Aquest procés serà recíproc entre els dos companys/es de grup.
- Fareu un vídeo explicant el procés i mostrant el resultat de com a màxim 6 minuts.

## A2 - Migració de Moodle:

- Per aquesta pràctica necessitareu un servidor ubuntu net que serà el receptor del Moodle.
- Migrareu tota la informació d'un dels dos Moodles actuals (escolliu un) a la màquina ubuntu server nova.
  Per començar el que farem serà activar el mode de manteniment del moodle. 
  
  Recolzarem la base de dades del moodle al servidor antic. 
  
  Restaurarem el suport de la base de dades al nou servidor. 
  
  Copiem el fitxer moodledata des de l'antic servidor al nou servidor.
  
  Copiem el codi del Moodle des de l'antic servidor al nou.
  
  Actualitzem el fitxer config.php amb l'URL del nou servidor.
  
  Provem el lloc copiat.
  
  Actualitzem els enllaços que contenen wwwroot a la base de dades. 
  
  Treiem el moodle del mode de manteniment. 
  
  
- Fareu un vídeo explicant el procés i mostrant el resultat de com a màxim 6 minuts.

# Recursos per a fer vídeos:

- [Editor Kdenlive](https://kdenlive.org/es/).
- [Editor online de vídeo Cliupchamp](https://clipchamp.com/en/) 

