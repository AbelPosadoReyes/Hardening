author: Abel Posado Reyes
summary: Instalación y configuración Grub(v.0.97)
id: Grub(v.0.97)
categories: codelab,markdown
environments: Web
status: Published
feedback link: Un enlace en el que los usuarios puedan darte feedback (quizás creando un issue en un repositorio de git)
analytics account: ID de Google Analytics
# Configuración Grub(v.0.97).

##Idioma
Duration: 0:02:00

Vamos a elegir el idioma de la computadora.

![Releases de claat](img/4.1.png)

##Usuarios
Duration: 0:02:00

Lo siguiente que deberemos realizar es el poner nombre a la máquina, en mi caso va a ser de Debian5.

![Releases de claat](img/4.2.png)

A continuación vamos a dejar el dominio en blanco, en este momento no nos hace falta.

![Releases de claat](img/4.8.png)

Le adjuntamos una contraseña a nuestro usuario administrador.

![Releases de claat](img/4.9.png)

Ponemos nombre completo a nuestro usuario (va a ser igual que el nombre de usuario).

![Releases de claat](img/4.10.png)
![Releases de claat](img/4.11.png)

Le adjudicamos una contraseña a dicho usuario.

![Releases de claat](img/4.12.png)

##Disco Duro
Duration: 0:05:00

A continuación vamos a organizar las particiones del disco duro, en este caso vamos a utilizar el disco completo sin configuración LVM.

![Releases de claat](img/4.3.png)

Seleccionamos el disco duro, en este caso tiene una capacidad de 10.7 GB.

![Releases de claat](img/4.4.png)

Debian nos da la posibilidad de separar las particiones /home, /usr, /var y /tmp, nos hubiera gustado que nos dejará crear las particiones nosotros, para añadir algunas particiones como /boot.

![Releases de claat](img/4.5.png)

Nos enseña como quedaria el disco completamente creado.

![Releases de claat](img/4.6.png)

Una vez acabado con los pasitos anteriores se nos instalará nuestro sistema operativo en nuestra computadora.

![Releases de claat](img/4.7.png)

##Configuración de Grub
Duration: 0:10:00

Una vez que estemos dentro vamos a insertar el comando grub-md5-crypt en una consola de comandos para adquirir un hash md5 de una contraseña que hemos añadido.

![Releases de claat](img/4.13.png)

Vamos a insertar ese hash en el fichero menu.lst situado en /boot/grub, antes de añadir el hash debemos poner password --md5.

![Releases de claat](img/4.14.png)

A continuación cabiaremos los permisos al fichero, para ello vamos a darle todos los permisos (escritura,lectura y ejecución), para ello vamos a añadir chmod 700 /boot/grub/menu.lst

![Releases de claat](img/4.15.png)

Y para finalizar nuestra protección sobre grub, vamos a cambiar el timeout de nuestro sistema operativo para que arranque directamente el sistema.

![Releases de claat](img/4.16.png)
