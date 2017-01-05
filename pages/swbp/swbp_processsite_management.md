---
title: Gestión de sitios de procesos
tags: [getting_started]
summary: "Descripción de las herramientas y acciones asociadas con la gestión de sitios de procesos"
sidebar: swbp_sidebar
permalink: swbp_processsite_management.html
folder: swbp
---

## Creación de sitios Web de procesos

### Creación de un sitio vacío
{{site.data.alerts.callout_warning}}
No se recomienda la creación de sitios Web vacíos
{{site.data.alerts.end}}
Un sitio Web de procesos vacío contiene los elementos generales para la gestión de procesos desde el sitio de administración, sin embargo, no cuenta con la configuración de los componentes para la documentación y operación de los procesos (bandeja, monitor, herramientas de colaboración). Por lo anterior, este tipo de sitio sólo es útil para desarrolladores que necesiten un punto de partida para crear su propio sitio de procesos con componentes ad-hoc.

Para crear un sitio de procesos vacío, seleccione en la barra de menús la opción **Nuevo** en el menú **Archivo > Crear Sitios Web**, como se muestra en la siguiente figura.

![Opción para crear sitio](images/screenshots/swbp_newsite_menu.png)

Se presentará el diálogo de creación de sitios como se muestra en la siguiente figura.

![Diálogo crear sitio](images/screenshots/swbp_newsite_dialog.png)

Deberá capturar en el diálogo los datos del formulario de acuerdo a la siguiente descripción de campos, seleccionando **Exclusivo** y **Sitio de Procesos** para los campos _Repositorio a utilizar_ y _Tipo de sitio_ respectivamente:

|Campo|Descripción|
|---|---|
|Título|Nombre visible del sitio en toda la adminisración, este nombre es usado como campo de búsqueda.|
|Identificador|Identificador único del sitio, usado en la URL de navegación. De existir el valor capturado se marcará el campo como erróneo.|
|Repositorio a utilizar|Combo de opciones para seleccionar el repositorio de usuarios a utilizar. Se mostrarán los repositorios existentes así como las opciones _Exclusive_, _Default UserRepository_ y _Admin UserRepository_ |
|Tipo de sitio|Combo de opciones para seleccionar el modelo de sitio a utilizar. Se mostrarán opciones como _Sitio Web_, _Sitio de Administración_ y _Sitio de Procesos_|

Finalmente, deberá presionar el botón **Guardar**. Se mostrará un mensaje de confirmación de la acción y en el acordeon de estructura de sitios se presentará el sitio recién creado.

{{site.data.alerts.callout_success}}
Si desea obtener más información sobre la creación de sitios Web y la descripción de los tipos de sitios y repositorios, puede consultar la <a href="http://semanticwebbuilder.org.mx/swb/swb/Manuales_Portal_Esoanol">página de documentación</a> de SemanticWebBuilder.
{{site.data.alerts.end}}

### Creación de un sitio desde la plantilla predeterminada
La opción recomendada para la creación de sitios de procesos es mediante el uso de la plantilla de sitio predeterminada. Esta plantilla de sitio tiene configurados los componentes necesarios para permitir la operación de procesos e incorpora la imagen de producto de SemanticWebBuilder Process. El sitio demo creado en la instalación de SWBProcess es creado mediante esta plantilla.

Para crear un sitio de procesos desde la plantilla predeterminada, seleccione en la barra de menús la opción **Predeterminado** en el menú **Archivo > Crear Sitios Web**, como se muestra en la siguiente figura.

![Opción para crear sitio plantilla](images/screenshots/swbp_templatesite_menu.png)

En la zona de trabajo se mostrará la pestaña _Predeterminado_ con la lista de plantillas disponibles para la creación de sitios.

![Lista de plantillas](images/screenshots/swbp_template_list.png)

En la lista de plantillas presione el icono **instalar** de la plantilla llamada _demo_.

![Instalar plantilla](images/screenshots/swbp_template_install.png)

Se presentará un formulario para capturar los datos del nuevo sitio. Deberá proporcionar valores válidos conforme a los campos descritos en la sección [creación de un sitio vacío](http://localhost:4000/swbp_processsite_management.html#creacin-de-un-sitio-vaco)

![Datos del nuevo sitio](images/screenshots/swbp_template_data.png)

Cuando haya terminado deberá presionar el botón **Enviar**. Se le solicitará confirmación de la acción.

![Confirmar nuevo sitio](images/screenshots/swbp_template_confirm.png)

Tras aceptar, se mostrará información del progreso. El sitio será instalado cuando en la tabla de progreso se muestre la leyenda _COMPLETO_ en cada columna.

![Confirmar nuevo sitio](images/screenshots/swbp_template_progress.png)

Finalmente, se mostrará un mensaje de confirmación de la acción y en el acordeon de estructura de sitios se presentará el sitio recién creado.

## Estructura de un sitio Web de procesos



## Edición de la configuración de un sitio de procesos

## Eliminación de sitios Web de procesos


{% include links.html %}
