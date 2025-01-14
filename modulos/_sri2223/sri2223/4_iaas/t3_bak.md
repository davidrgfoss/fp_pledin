---
title: "Taller 3: Gestión de instancias en OpenStack"
---

## ¿Qué vas a aprender en este taller?

* Creación de instancias con OpenStack.
* Configuración de la instancia con cloud-init.
* Instantáneas de instancias.

## Recursos para realizar este taller

* Capítulo 3 del [Curso OpenStack](https://github.com/josedom24/curso_openstack_ies).

## ¿Qué tienes que hacer?

Los siguientes pasos los debes hacer con el cliente de OpenStack, puedes entrar en Horizon para comprobar si se ha realizado de forma correcta la acción realizada.

1. Crea una instancias Linux, con las siguientes características configuradas con cloud-init:
	* Al iniciarse se deben actualizar los paquetes.
	* Se debe instalar Apache2.
	* Se debe crear un usuario (con tu nombre) y contraseña.
2. Asigna a la instancia una dirección IP flotante.
3. Añade una regla en el cortafuegos para abrir el puerto 80.
4. Accede a la máquina por SSH y cambia el fichero `index.html`.
5. Accede desde un navegador web al servidor web de la instancia y comprueba el cambio del fichero `index.html`.
6. Crea una instantánea de la instancia (puedes buscar cómo hacerla con OSC o lo puedes realizar desde horizon).
7. Crea una nueva instancia desde la instantánea. Asígnale una nueva IP flotante y comprueba a acceder desde un navegador web al servidor web de la nueva instancia. ¿Tiene el mismo fichero `index.html`?

{% capture notice-text %}
## ¿Qué tienes que entregar?

1. Acceso por SSH a la instancia con el usuario que has creado. Comprobación de que tiene el servidor web apache2 instalado.
2. Acceso desde un navegador web a la instancia.
3. Comprobación de que has realizado una instantánea.
4. Acceso a la nueva instancia creada desde un navegador web. ¿Tiene el mismo fichero `index.html`?
{% endcapture %}<div class="notice--info">{{ notice-text | markdownify }}</div>
