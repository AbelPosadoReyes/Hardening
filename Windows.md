author: Abel Posado Reyes
summary: Reestablecer contraseña Windows 10
id: reestablecer-contraseña
categories: codelab,markdown
environments: Web
status: Published
feedback link: Un enlace en el que los usuarios puedan darte feedback (quizás creando un issue en un repositorio de git)
analytics account: ID de Google Analytics

#Reestablecer contraseña W10

##Paso 1
Duration: 0:02:00

Escribimos una contraseña al azar para que podamos reestablecer la contraseña, entramos para cambiar dicha contraseña.

![Releases de claat](img/3.1.png)

##Paso 2
Duration: 0:02:00
Deberemos poner las respuestas correctas en los apartados correspondientes.

![Releases de claat](img/3.2.png)

![Releases de claat](img/3.3.png)

##Paso 3
Duration: 0:02:00

Entraremos a nuestro Windows con normalidad.

![Releases de claat](img/3.4.png)

<DESACTIVACIÓN DE OPC REESTABLECER
Esta opción de deshabilitar la opción de reestablecer contraseña no podemos realizarla, ya que Microsoft nos deja solo una alternativa si no nos acordamos de nuestra clave.>

##Paso 4 
Duration: 0:02:00

En este apartado vamos a deshabilitar el proceso utilman.exe. Antes de comenzar debemos saber que el fichero esta situado en c:\Windows\System32, antes de denegar el proceso para todos los usuarios debemos cambiarle los permisos del fichero. Para ello insertaremos el siguiente comando en una cmd: takeown /f c:\Windows\System32\utilman.exe.

![Releases de claat](img/6.1.png)

Una vez hayamos realizado el paso anterior, debemos reiniciar el equipo para actualizar los cambios realizados.

Una vez que hayamos inicie el equipo de nuevo debemos Denegar todos los permisos de los usuarios, para ello debemos asistir a la carpeta del fichero y modificar sus propiedas de seguridad.

![foto1](img/6.2.png)
![foto2](img/6.3.png)
![foto3](img/6.4.png)
![foto4](img/6.5.png)
![foto5](img/6.6.png)
![foto6](img/6.7.png)