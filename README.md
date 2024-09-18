# NginxDocker
Configurar un Docker con Nginx con el puerto 80 eh instalar dentro de ese Docker Python , crear un usuario y ejecutar el ejemplo de FLASK, configurar proxy para responder por enpoint /pagina para resolver el puerto 5000 del FLASK.

# Instlacion de Nginx
Ejecutamos el siguiente comando para descargar la imagen de nginx

![image](https://github.com/user-attachments/assets/3a229396-cfbd-4ba8-9bb2-d8b1e584e73d)

## Ejecutamos el siguiente comando 

![image](https://github.com/user-attachments/assets/2f137aa1-d3db-4ec7-91fa-6629a7f27031)

* --name mi-nginx: Le da un nombre al contenedor 
* -p 8080:80: Mapea el puerto 80 del contenedor al puerto 8080 de tu máquina local.
* -d: Ejecuta el contenedor en segundo plano (detached mode).
* nginx: El nombre de la imagen que deseas usa

**Abrimos el navegador en el localhost y puero 80 para verificar que nginx esta corriendo**

![image](https://github.com/user-attachments/assets/afa16871-098f-4112-93ef-7b5a8ec95b08)

**Con los siguientes comandos ejecutamos un comando dentro de la imagen de Nginx en ejecucion esto nos permite interactuar con la imagen**

![image](https://github.com/user-attachments/assets/e5718a28-da23-46e0-b1e9-53cc4776132a)

Creamos un nuevo usuario dentro de la imagen de Nginx
![image](https://github.com/user-attachments/assets/90549080-6cab-47b0-9213-278554537128)

Una vez dentro de la imagen de nginx la acualizamos y intlamos python3 
* apt update
* apt install python3-pip

**Cambiamos de usuario y creamos el directorio donde crearemos el entorno virtual para flask**
![image](https://github.com/user-attachments/assets/f1c82b54-c99f-46e2-a45e-321a1e1f33b9)

Iniciamos el entorno virtual y procemos a instalar flask 
![image](https://github.com/user-attachments/assets/ca3bb978-d5e6-4735-a01f-7a801b1b882d)

![image](https://github.com/user-attachments/assets/fcdf1f0b-99ba-4cf8-8b3d-7aa78d9ec42e)


creamos un archivo con el hola mundo de flask 

![image](https://github.com/user-attachments/assets/478c9cc0-312e-475b-978f-1720e4e8b2fc)

Modificamos el archivo defaulf.conf que se encuentra en la ruta **/etc/nginx/conf.d/defaulf.conf**





  
