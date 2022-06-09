# App Web en PHP
Uso de **App Services** para implementar una página web hecha con PHP.

-----------------------------------------------------------------------------------------------
## Requisitos
- Suscripción Azure activa.
- Cuenta de GitHub que poseea un archivo preferentemente **index.php**.

-----------------------------------------------------------------------------------------------

## Procedimiento
1. Entramos a [Portal Azure](https://portal.azure.com).
![Portal Azure](https://github.com/OrtegaRamiro31/P3_AppService-paginaPHP-/blob/main/imgs/1.png)

2. En el buscador escribimos **App Services** y le damos click. Después también hacemos click en **Crear**.
![App Services](https://github.com/OrtegaRamiro31/P3_AppService-paginaPHP-/blob/main/imgs/2.png)

3. Llenamos los campos. Se necesita:
    * Una suscripcion
    * Grupo de recursos
    * Nombre (que será para la URL)
    * Elegir si queremos subir Código, Contendeor Docker o Aplicación web estática.
    * Sistema operativo (Linux en este caso).
    * Región
![Llenado de campos App Services](https://github.com/OrtegaRamiro31/P3_AppService-paginaPHP-/blob/main/imgs/3.png)

4. Un poco más abajo tenemos **Plan de Linux**, se deja por defecto. Sin embargo, en **Sku y tamaño** damos click en **Cambiar tamaño** y seleccionamos **F1**. Esto evitará cobros.
![Sku](https://github.com/OrtegaRamiro31/P3_AppService-paginaPHP-/blob/main/imgs/4.png)

5. No es necesario hacer otra cosa, simplemente nos vamos al apartado de **Revisar y crear** y al final seleccionamos **Crear**.
![Creación de App Services](https://github.com/OrtegaRamiro31/P3_AppService-paginaPHP-/blob/main/imgs/5.png)

6. La implementación comenzará y tardará unos minutos en terminar. Damos click en **Ir al recurso**.
![Implementación de App Services](https://github.com/OrtegaRamiro31/P3_AppService-paginaPHP-/blob/main/imgs/6.png)

7. Una vez dentro del recurso, seleccionamos **Centro de implementación** y una vez dentro seleccionamos de **Origen** a GitHub. 
    * Nos logueamos con nuestra cuenta.
    * En organización seleccionamos nuestra cuenta de usuario.
    * En repositorio seleccionamos el repositorio con la página web.
    * En rama, seleccionamos la correspondiente, en este caso, main.
![Uso de GitHub en Azure para implementar la página](https://github.com/OrtegaRamiro31/P3_AppService-paginaPHP-/blob/main/imgs/7.png)

Al final solo se da click en **Guardar**.

8. En nuestro repositorio de GitHub podemos ver las acciones que está sucediendo. Para observar lo anterior, seleccionamos nuestro repositorio y seleccionamos **Action**. La acción que aparecerá se debe a lo que hicimos anteriormente en Azure. Cuando la página esté lista aparecerá un círculo verde con una palomita. 
![Actions en GitHub](https://github.com/OrtegaRamiro31/P3_AppService-paginaPHP-/blob/main/imgs/8.png)

9. Regresando a el recurso creado, en la parte de **Introducción** damos click en el enlace que aparece al lado derecho de **URL**, esto nos redirigirá a nuestra página web.
![Introducción de App Services](https://github.com/OrtegaRamiro31/P3_AppService-paginaPHP-/blob/main/imgs/9.png)

10. En este caso, este es el resultado obtenido cuando entramos a la página web.
![Página web por defecto](https://github.com/OrtegaRamiro31/P3_AppService-paginaPHP-/blob/main/imgs/10.png)

11. Si tenemos otro archivo php o html podemos acceder a él simplemente modificando en la barra de direcciones como se muestra en la siguiente imágen.
![Página web 2 del mismo repositorio](https://github.com/OrtegaRamiro31/P3_AppService-paginaPHP-/blob/main/imgs/11.png)
