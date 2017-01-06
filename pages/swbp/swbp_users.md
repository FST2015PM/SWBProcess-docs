---
title: Gestión de usuarios y permisos
tags: [getting_started, troubleshooting, support]
summary: "Soporte técnico al producto"
sidebar: swbp_sidebar
permalink: swbp_users.html
folder: swbp
---

## Repositorios de usuarios
Los perfiles de usuarios en SemanticWebBuilder Process proveen una cuenta de acceso a las personas relacionadas con los sitios de procesos o el sitio de administración. El manejo de usuarios se realiza por medio de repositorios de usuarios, que son catálogos que almacenan tanto los perfiles individuales de cada persona como los grupos de usuarios y roles correspondientes.

{{site.data.alerts.callout_success}}
Un repositorio de usuarios puede ser compartido entre varios sitios, aunque no es una práctica común.
{{site.data.alerts.end}}

SWBProcess cuenta con un repositorio denominado _Admin_. Este repositorio está asociado al sitio de administración de SWBProcess y contiene el registro de los usuarios con facultades para administrar los distintos sitios de procesos. Por otro lado, el sitio de demostración instalado con SWBProcess contiene un repositorio de usuarios con los siguientes perfiles para realizar pruebas:

|Usuario|Password|Descripción|
|---|---|---|
|admin|webbuilder|Usuario con rol de administrador|
|empleado|empleado|Usuario con rol de empleado|
|director|director|Usuario con rol de director|
|humanos|humanos|Usuario con rol de RH|

{{site.data.alerts.callout_success}}
A los usuarios del repositorio <i>Admin</i> se les denomina usuarios administradores. Es importante no asignar el repositorio <i>Admin</i> a los sitios de procesos.
{{site.data.alerts.end}}

Podrá acceder a los repositorios de usuario haciendo click en el acordeón **Repositorios de usuarios**.

{% include image.html class="centered shadow adjusted" file="screenshots/swbp_user_repaccordeon.png" alt="Acordeon de repositorios de usuarios" %}

Al expandirse el acordeón se mostrará la lista de los repositorios existentes, sus roles y grupos relacionados como se muestra en la siguiente figura.

{% include image.html class="centered x-small shadow adjusted" file="screenshots/swbp_userrep_list.png" alt="Lista de repositorios de usuarios" %}

### Creación de un repositorio de usuarios
Un repositorio de usuarios es creado de manera automática cada vez que se crea un sitio de procesos nuevo y se selecciona la opción _Exclusivo_ en el tipo de repositorio a utilizar (consultar sección [crear un sitio vacío](http://localhost:4000/swbp_processsite_management.html#creacin-de-un-sitio-vaco)). Sin embargo, usted puede crear un repositorio de usuario mediante la barra de menús.

Para crear un nuevo repositorio seleccione la opción **Nuevo** en el menú **Archivo** > **Crear Repositorio de Usuarios**.

{% include image.html class="centered small shadow adjusted" file="screenshots/swbp_newrepo_menu.png" alt="Opción para crear repositorio" %}

Se presentará el diálogo de creación de repositorios como se muestra en la siguiente figura.

{%include image.html class="centered small shadow adjusted" file="screenshots/swbp_newrepo_dialog.png" alt="Diálogo crear repositorio"%}

Deberá capturar en el diálogo los datos del formulario de acuerdo a la siguiente descripción de campos, seleccionando **Exclusivo** y **Sitio de Procesos** para los campos _Repositorio a utilizar_ y _Tipo de sitio_ respectivamente:

|Campo|Descripción|
|---|---|
|Título|Nombre visible del sitio en toda la adminisración, este nombre es usado como campo de búsqueda.|
|Identificador|Identificador único del sitio, usado en la URL de navegación. De existir el valor capturado se marcará el campo como erróneo.|
|Repositorio a utilizar|Combo de opciones para seleccionar el repositorio de usuarios a utilizar. Se mostrarán los repositorios existentes así como las opciones _Exclusive_, _Default UserRepository_ y _Admin UserRepository_ |
|Tipo de sitio|Combo de opciones para seleccionar el modelo de sitio a utilizar. Se mostrarán opciones como _Sitio Web_, _Sitio de Administración_ y _Sitio de Procesos_|

Finalmente, deberá presionar el botón **Guardar**. Se mostrará un mensaje de confirmación de la acción y en el acordeon de estructura de sitios se presentará el sitio recién creado.

### Creación de roles

### Creación de grupos

## Creación de usuarios

### Edición de las propiedades de un usuario

### Activación/desactivación de usuarios

## Control de acceso

### Asignación de roles

### Asignación de grupos

### Aplicación de filtros de usuario

## Eliminación de usuarios

{% include links.html %}
