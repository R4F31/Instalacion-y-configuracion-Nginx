# Instalacion-y-configuracion-Nginx

##Instalacion NGINX
1. Abrimos la tarminal de ubuntu y introducimos el siguiente comando.
![imagen](https://github.com/R4F31/Instalacion-y-configuracion-Nginx/blob/main/Ngnix/1.PNG)

2.Una vez ya instalado para verificar que se ha instalado correctamente abriremos el navegador web y en el buscador introducimos localhost y nos tiene que aparecer la siguiente pagina
![imagen](https://github.com/R4F31/Instalacion-y-configuracion-Nginx/blob/main/Ngnix/2.PNG)

##Configuración NGINX

1.En la consola iremos al directorio etc/nginx
![imagen](https://github.com/R4F31/Instalacion-y-configuracion-Nginx/blob/main/Ngnix/3.PNG)

2.Una vez situados en el directorio nos dirigiremos a sites-available

3.Copiaremos el archivo default y le daremos un nombre al dominio que queramos crear. Rste proceso lo repetiremos tantes veces como dominios queramos.
![imagen](https://github.com/R4F31/Instalacion-y-configuracion-Nginx/blob/main/Ngnix/4.PNG)

4.Abriremos los archivos que hemos creado con un editor de texto para posteriormente modificarlos.

5.Tendremos que modificar varios parametros que sera: Eliminar el default_Server, en el campo root tendremos que modificar la ruta a donde estaran nuestros html y modificaremos el nombre del servidor con el nombre que le hayamos puesto a nuestro dominio.
![imagen](https://github.com/R4F31/Instalacion-y-configuracion-Nginx/blob/main/Ngnix/6.PNG)

6. Una vez llegados a este paso tambien tendremos que crear los mismos archivos en el directorio sites-enabled o hacer un link con los archivos de sites-avaible. Tenemos que ir con cuidado ya que estos archivps deberan tener el mismo nombre que los que hemos creado anteriormente.
![imagen](https://github.com/R4F31/Instalacion-y-configuracion-Nginx/blob/main/Ngnix/8.PNG)

7.Posteriormente reiniciamos nginx
![imagen](https://github.com/R4F31/Instalacion-y-configuracion-Nginx/blob/main/Ngnix/9.PNG)

8.Tenemos que modificar el archivo host, este se encuentra en la ruta /etc/hosts. Lo modificamos para poder añadir los dominios que hemos creado 
![imagen](https://github.com/R4F31/Instalacion-y-configuracion-Nginx/blob/main/Ngnix/10.PNG)

9.Llegados a este paso, crearemos los directorios donde iran los archivos html. Debemos crear los directior con el nombre que hemos indicado en el paso 5
![imagen](https://github.com/R4F31/Instalacion-y-configuracion-Nginx/blob/main/Ngnix/11.PNG)

10.Introducimos el codigo html dentro del directorio que hemos creado y lo tenemos que guardar como index.html

##Resultado final
1.Iremos a nuestro navegador web y introduciremos el url de nuestras paginas. En mi caso es prueba1.nginx/index.html y prueba2.nginx/index.html . Si hemos realizado todas las configuraciones correctamente nos deberian salir las dos paginas que hemos creado.
![imagen](https://github.com/R4F31/Instalacion-y-configuracion-Nginx/blob/main/Ngnix/12.PNG)
![imagen](https://github.com/R4F31/Instalacion-y-configuracion-Nginx/blob/main/Ngnix/13.PNG)







