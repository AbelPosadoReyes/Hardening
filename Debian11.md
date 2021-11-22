author: Abel Posado Reyes
summary: Instalación y configuración Grub(v.2.04)
id: Grub(v.2.04)
categories: codelab,markdown
environments: Web
status: Published
feedback link: Un enlace en el que los usuarios puedan darte feedback (quizás creando un issue en un repositorio de git)
analytics account: ID de Google Analytics
# Configuración Grub(v.2.04).

##Instalar el SO
Duration: 0:02:00

Vamos a elegir Graphical install para instalar el sistema operativo en nuestra computadora graficamente.

![Releases de claat](img/5.1.png)

##Idioma
Duration: 0:02:00

Lo siguiente que deberemos realizar es ponerle el idioma a nuestra computadora.

![Releases de claat](img/5.2.png)

##Usuarios
Duration: 0:05:00

A continuación vamos a proponer un nombre para nuestra computadora, en este caso va a ser Debian11.

![Releases de claat](img/5.3.png)

Vamos a dejar nuestro equipo sin dominio previamente.

![Releases de claat](img/5.4.png)

Vamos a añadir una contrasela a nuestro usuario administrador, preferiblemente que contenga números, minúsculas y mayúsculas.

![Releases de claat](img/5.5.png)

Le adjudicamos un nombre a nuestro usuario y su respectiva contraseña

![Releases de claat](img/5.6.png)
![Releases de claat](img/5.7.png)

##Disco Duro
Duration: 0:05:00

Vamos a realizar un disco duro con sus respectivas particiones, no vamos a añadirle una configuración LVM.

![Releases de claat](img/5.8.png)

Seleccionamos el disco correspondiente.

![Releases de claat](img/5.9.png)

Vamos a realizar la separación de particiones de /home, /var y /tmp. Me gustaría haber podido separar /usr, /boot, /swap, etc...

![Releases de claat](img/5.10.png)

Nos saldría dos pantallas para verificar las particiones.

![Releases de claat](img/5.11.png)
![Releases de claat](img/5.12.png)

##Inicio

Una vez hayamos realizado los pasos anteriores correctamente se nos reiniciara el equipo y podremos acceder a nuestro equipo.

![Releases de claat](img/5.13.png)

##Configuración de Grub
Duration: 0:10:00

Vamos a entrar con el comando su en el fichero 40_custom, situado en la siguiente ruta: /etc/grub.d.

![Releases de claat](img/5.14.png)

Lo siguiente que vamos a realizar es la protección de del usuario root, para ello vamos a generar la contraseña con el comando ___________ y la vamos a añadir al fichero junto a password root.

![Releases de claat](img/5.15.png)

A continuación vamos cambiar los permisos del fichero y vamos a dejarlo en 700 (el propietario es el único que tiene acceso a lectura, escritura y ejecución)

![Releases de claat](img/5.16.png)

Ahora vamos a reconfigurar el timeout del sistema, para ello vamos a ingresar en el fichero /etc/default/grub y lo vamos a poner a cero.

![Releases de claat](img/5.17.png)

El último paso que debemos realizar es la actualización de grub con los cambios realizados anteriormente.

![Releases de claat](img/5.18.png)

