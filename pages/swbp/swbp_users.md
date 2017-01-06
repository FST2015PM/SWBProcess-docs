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
Un repositorio de usuarios es creado de manera automática cada vez que se crea un sitio de procesos nuevo y se selecciona la opción _Exclusivo_ en el tipo de repositorio a utilizar (consultar sección [crear un sitio vacío](http://localhost:4000/swbp_processsite_management.html#creacin-de-un-sitio-vaco)). Sin embargo, usted puede crear un repositorio de usuarios mediante la barra de menús.

Para crear un nuevo repositorio seleccione la opción **Nuevo** en el menú **Archivo** > **Crear Repositorio de Usuarios**.

{% include image.html class="centered small shadow adjusted" file="screenshots/swbp_newrepo_menu.png" alt="Opción para crear repositorio" %}

Se presentará el diálogo de creación de repositorios como se muestra en la siguiente figura.

{%include image.html class="centered small shadow adjusted" file="screenshots/swbp_newrepo_dialog.png" alt="Diálogo crear repositorio"%}

Deberá capturar en el diálogo los datos del formulario de acuerdo a la siguiente descripción de campos.

|Campo|Descripción|
|---|---|
|Título|Nombre visible del repositorio en toda la administración, este nombre es usado como campo de búsqueda.|
|Identificador|Identificador único del repositorio. Éste es sensible a mayúsculas y minúsculas. De existir el valor capturado se marcará el campo como erróneo.|

Finalmente, deberá presionar el botón **Guardar**. El repositorio se presentará en el acordeón correspondiente.

### Creación de roles
En SemanticWebBuilder Process un rol representa de manera conceptual, una función, puesto o papel que un usuario desempeña dentro de la organización. A través de los roles se delimita el acceso a secciones, procesos, actividades y contenidos en el sitio de procesos o el sitio de administración.

Asignar un rol a un usuario significa que se le está concediendo un perfil nuevo dentro de los sitios y que en consecuencia podrá acceder a la información que esté filtrada para ese rol en particular.

{{site.data.alerts.callout_success}}
Los permisos asociados a los roles son acumulativos, es decir, un usuario con varios roles asignados tendrá acceso a las secciones y contenidos establecidas en cada uno de esos roles.
{{site.data.alerts.end}}

Para crear un rol, deberá primero ubicar el repositorio de usuarios deseado en el acordeón de **repositorios de usuarios** y deberá expandir su estructura usando el ícono _Expandir_ {% include inline_image.html file="screenshots/spriteTree.gif" %} a la izquierda del nombre del repositorio.

Posteriormente, deberá hacer click con el botón derecho en el nodo _Roles_ {% include inline_image.html file="screenshots/icon_role.png" class="icon" %} y seleccionar la opción **Agregar Rol** como se muestra en la siguiente figura.

{%include image.html class="centered small shadow adjusted" file="screenshots/swbp_addrole_menu.png" alt="Opción para agregar rol"%}

Se presentará el diálogo _Agregar Rol_ como se muestra en la siguiente figura.

{%include image.html class="centered medium shadow adjusted" file="screenshots/swbp_newrole_dialog.png" alt="Diálogo crear repositorio"%}

Deberá capturar en el diálogo los datos del formulario de acuerdo a la siguiente descripción de campos.

|Campo|Descripción|
|---|---|
|Título|Nombre visible del rol en toda la administración, este nombre es usado como campo de búsqueda.|
|Identificador|Identificador único del rol. Éste es sensible a mayúsculas y minúsculas. De existir el valor capturado se marcará el campo como erróneo.|

Finalmente, deberá presionar el botón **Guardar**. El nuevo rol se presentará en el árbol del repositorio correspondiente.

{%include image.html class="centered small shadow adjusted" file="screenshots/swbp_newrole_tree.png" alt="Nuevo rol en el repositorio"%}

Al mismo tiempo, se mostrarán las pestañas de edición del rol en la zona de trabajo, con la pestaña _Información_ seleccionada, como se muestra en la siguiente figura.

{%include image.html class="centered shadow adjusted" file="screenshots/swbp_role_tabs.png" alt="Pestañas de configuración del rol"%}

### Eliminación de roles
Podrá eliminar un rol de un repositorio presionando el botón **Eliminar** en el formulario de la pestaña de información del rol.

{%include image.html class="centered shadow adjusted" file="screenshots/swbp_role_removebutton.png" alt="Botón de eliminación"%}

También puede realizar la acción desde el árbol del repositorio, haciendo click con el botón derecho sobre el nombre del rol y seleccionando la opción **Eliminar**, como se muestra en la siguiente figura.

{%include image.html class="centered small shadow adjusted" file="screenshots/swbp_role_removeoption.png" alt="Opción de eliminación del rol"%}

En cualquier caso, se solicitará confirmación de la acción. Si acepta, el rol será eliminado y desaparecerá del árbol del repositorio de usuarios.

{%include image.html class="centered small shadow adjusted" file="screenshots/swbp_role_deleteconfirm.png" alt="Opción de eliminación del sitio"%}

{{site.data.alerts.callout_warning}}
Al eliminar un rol, se eliminan las asociaciones del mismo con los usuarios y los elementos del sitio, por lo que las restricciones de acceso cambiarán en consecuencia.
{{site.data.alerts.end}}

### Creación de grupos de usuarios
En SemanticWebBuilder Process un grupo de usuarios representa de manera conceptual un área o departamento de una organización y su función es categorizar a los usuarios de manera independiente a los roles que desempeñen dentro de un área. A través de los grupos se delimita el acceso a secciones, procesos, actividades y contenidos en el sitio de procesos o el sitio de administración.

Asignar un grupo a un usuario significa que se le está concediendo un perfil nuevo dentro de los sitios y que en consecuencia podrá acceder a la información que esté filtrada para ese grupo en particular.

Para crear un grupo de usuarios, deberá primero ubicar el repositorio de usuarios deseado en el acordeón de **repositorios de usuarios** y deberá expandir su estructura usando el ícono _Expandir_ {% include inline_image.html file="screenshots/spriteTree.gif" %} a la izquierda del nombre del repositorio.

Posteriormente, deberá hacer click con el botón derecho en el nodo _Grupos de usuarios_ {% include inline_image.html file="screenshots/icon_usergroup.png" class="icon" %} y seleccionar la opción **Agregar Grupo de Usuarios** como se muestra en la siguiente figura.

{%include image.html class="centered small shadow adjusted" file="screenshots/swbp_addrole_menu.png" alt="Opción para agregar rol"%}

Se presentará el diálogo _Agregar Grupo de Usuarios_ como se muestra en la siguiente figura.

{%include image.html class="centered medium shadow adjusted" file="screenshots/swbp_newrole_dialog.png" alt="Diálogo crear repositorio"%}

Deberá capturar en el diálogo los datos del formulario de acuerdo a la siguiente descripción de campos.

|Campo|Descripción|
|---|---|
|Título|Nombre visible del grupo en toda la administración, este nombre es usado como campo de búsqueda.|
|Identificador|Identificador único del grupo. Éste es sensible a mayúsculas y minúsculas. De existir el valor capturado se marcará el campo como erróneo.|

Finalmente, deberá presionar el botón **Guardar**. El nuevo grupo se presentará en el árbol del repositorio correspondiente.

{%include image.html class="centered small shadow adjusted" file="screenshots/swbp_newrole_tree.png" alt="Nuevo rol en el repositorio"%}

Al mismo tiempo, se mostrarán las pestañas de edición del grupo en la zona de trabajo, con la pestaña _Información_ seleccionada, como se muestra en la siguiente figura.

{%include image.html class="centered shadow adjusted" file="screenshots/swbp_role_tabs.png" alt="Pestañas de configuración del rol"%}

## Gestión de usuarios

### Edición de las propiedades de un usuario

### Activación/desactivación de usuarios

### Eliminación de usuarios

## Control de acceso

### Asignación de roles

### Asignación de grupos

### Aplicación de filtros de usuario

{% include links.html %}
