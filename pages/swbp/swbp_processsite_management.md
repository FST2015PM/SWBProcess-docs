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

{%include image.html class="centered medium shadow adjusted" file="screenshots/swbp_newsite_menu.png" alt="Opción para crear sitio"%}

Se presentará el diálogo de creación de sitios como se muestra en la siguiente figura.

{%include image.html class="centered medium shadow adjusted" file="screenshots/swbp_newsite_dialog.png" alt="Diálogo crear sitio"%}

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

{%include image.html class="centered medium shadow adjusted" file="screenshots/swbp_templatesite_menu.png" alt="Opción para crear sitio plantilla"%}

En la zona de trabajo se mostrará la pestaña _Predeterminado_ con la lista de plantillas disponibles para la creación de sitios.

{%include image.html class="centered shadow adjusted" file="screenshots/swbp_template_list.png" alt="Lista de plantillas"%}

En la lista de plantillas presione el icono **instalar** de la plantilla llamada _demo_.

{%include image.html class="centered shadow adjusted" file="screenshots/swbp_template_install.png" alt="Instalar plantilla"%}

Se presentará un formulario para capturar los datos del nuevo sitio. Deberá proporcionar valores válidos conforme a los campos descritos en la sección [creación de un sitio vacío](http://localhost:4000/swbp_processsite_management.html#creacin-de-un-sitio-vaco)

{%include image.html class="centered medium shadow adjusted" file="screenshots/swbp_template_data.png" alt="Datos del nuevo sitio"%}

Cuando haya terminado deberá presionar el botón **Enviar**. Se le solicitará confirmación de la acción.

{% include image.html class="centered medium shadow adjusted" file="screenshots/swbp_template_confirm.png" alt="Confirmar nuevo sitio" %}

Tras aceptar, se mostrará información del progreso. El sitio será instalado cuando en la tabla de progreso se muestre la leyenda _COMPLETO_ en cada columna.

{% include image.html class="centered shadow adjusted" file="screenshots/swbp_template_progress.png" alt="Indicador de progreso" %}

Finalmente, se mostrará un mensaje de confirmación de la acción y en el acordeon de estructura de sitios se presentará el sitio recién creado.

{% include image.html class="centered small shadow adjusted" file="screenshots/swbp_process_created.png" alt="Sitio creado" %}

## Estructura de un sitio Web de procesos
Al crear un nuevo sitio de procesos, ya sea vacío o desde la plantilla predeterminada, éste presentará en los acordeones de estructura, una estructura similar a la de la figura.

{% include image.html class="centered small shadow adjusted" file="screenshots/swbp_site_structure.png" alt="Estructura de un sitio de procesos" %}

Cada elemento (nodo) en el árbol de estructura del sitio se describe a continuación.

|Elemento|Descripción|
|---|---|
|Plantillas|Contiene las plantillas (código HTML de despliegue) y grupos de plantillas existentes en el sitio. SWBProcess cuenta con una sola plantilla llamada _main_ en el grupo denominado _Process_. Puede obtener más información sobre la gestión de plantillas en el [manual](http://www.semanticwebbuilder.org.mx/en_mx/swb/Manuales_Portal_Esoanol/_rid/426/_mto/3/_act/download/doc/Creacion_y_Administracion_de_Plantillas_para_Presentacion_de_Paginas_Web.pdf) correspondiente.|
|Reglas|Contiene las reglas definidas para el sitio, aplicables a los usuarios para el control de acceso. SWBProcess sólo cuenta con una regla llamada _Registrado_ que obliga a que los usuarios tengan un registro para acceder al sitio. Puede obtener más información sobre la gestión de reglas en el [manual](http://www.semanticwebbuilder.org.mx/en_mx/swb/Manuales_Portal_Esoanol/_rid/435/_mto/3/_act/download/doc/Creacion_y_Administracion_de_Reglas_de_Personalizacion.pdf) correspondiente.|
|Calendarios|Contiene las calendarizaciones aplicables a los elementos del sitio. Puede obtener más información sobre la gestión de calendarios en el [manual](http://www.semanticwebbuilder.org.mx/en_mx/swb/Manuales_Portal_Esoanol/_rid/425/_mto/3/_act/download/doc/Creacion_y_Uso_de_Calendarizacion.pdf) correspondiente.|
|Flujos de publicación|Contiene los flujos de publicación aplicables a los contenidos del sitio. Puede obtener más información sobre la gestión de flujos de publicación en el [manual](http://www.semanticwebbuilder.org.mx/en_mx/swb/Manuales_Portal_Esoanol/_rid/424/_mto/3/_act/download/doc/Creacion_y_Administracion_de_Flujos_de_Publicacion.pdf) correspondiente.|
|Lenguajes|Contiene los idiomas aplicables a los elementos y contenidos del sitio. Puede obtener más información sobre la gestión de idiomas en el [manual](http://www.semanticwebbuilder.org.mx/en_mx/swb/Manuales_Portal_Esoanol/_rid/437/_mto/3/_act/download/doc/Administracion_de_Catalogo_de_Lenguajes_y_Paises_de_Presentacion.pdf) correspondiente.|
|Países|Contiene los países asociados a los idiomas del sitio. Puede obtener más información sobre la gestión de países en el [manual](http://www.semanticwebbuilder.org.mx/en_mx/swb/Manuales_Portal_Esoanol/_rid/437/_mto/3/_act/download/doc/Administracion_de_Catalogo_de_Lenguajes_y_Paises_de_Presentacion.pdf) correspondiente.|
|Dispositivos|Contiene una jerarquía de dispositivos utilizados para definir reglas de presentación específicas. Puede obtener más información sobre la gestión de dispositivos en el [manual](http://www.semanticwebbuilder.org.mx/en_mx/swb/Manuales_Portal_Esoanol/_rid/436/_mto/3/_act/download/doc/Adminstracion_de_Catalogo_de_Dispositivos_de_Navegacion_de_Usuarios.pdf) correspondiente.|
|DNS|Contiene mapeos entre nombres de dominio y sitios, con la finalidad de proporcionar un mecanismo para presentar sitios distintos de acuerdo con los nombres de dominio. Puede obtener más información sobre la gestión de DNS en el [manual](http://www.semanticwebbuilder.org.mx/en_mx/swb/Manuales_Portal_Esoanol/_rid/438/_mto/3/_act/download/doc/Adminstracion_de_Catalogo_de_DNS.pdf) correspondiente.|
|Colecciones|Permite crear agrupadores de elementos de un sitio con base en su definición ontológica.|
|Colección de recursos|Permite crear agrupadores de recursos de un sitio.|
|Componentes de estrategia|Contiene el catálogo de componentes de estrategia del sitio. Estos elementos son utilizados como bloques de construcción en las plantillas del sitio. Puede obtener más información sobre la gestión de componentes de estrategia en el [manual](http://www.semanticwebbuilder.org.mx/en_mx/swb/Manuales_Portal_Esoanol/_rid/428/_mto/3/_act/download/doc/Administracion_y_Publicacion_de_Componentes_de_Estrategia.pdf) correspondiente.|
|Componentes de sistema|Contiene el catálogo de componentes de sistema del sitio. Estos elementos son utilizados como bloques de construcción en las plantillas del sitio o como componentes de contenido en las páginas. Puede obtener más información sobre la gestión de componentes de sistema en el [manual](http://www.semanticwebbuilder.org.mx/en_mx/swb/Manuales_Portal_Esoanol/_rid/432/_mto/3/_act/download/doc/Administracion_y_Publicacion_de_Componentes_de_Sistema_v2.pdf) correspondiente.|
|Componentes de contenido|Contiene el catálogo de componentes de contenido del sitio. Estos elementos son utilizados como bloques de funcionalidad o información en las páginas del sitio. Puede obtener más información sobre la gestión de componentes de contenido en el [manual](http://www.semanticwebbuilder.org.mx/en_mx/swb/Manuales_Portal_Esoanol/_rid/423/_mto/3/_act/download/doc/Administracion_y_Publicacion_de_Componentes_de_Contenido.pdf) correspondiente.|
|Herramientas de proceso|Contiene el catálogo de elementos utilizados en la configuración de uno o más procesos: _Certificados_, _Plantillas de notificaciones_, _Intervalos de ejecución_, _Reglas de negocio_, _Conexiones a bases de datos_, _Servicios Web_ y _Propiedades de asignación_.|
|Procesos|Contiene la definición de los procesos de negocio del sitio, sus modelos y sus grupos.|
|Repositorio de usuarios|Contiene el repostorio de usuarios asociado al sitio, los roles y grupos de usuarios.|
|Home(SWBProcess)|Contiene la estructura de páginas Web del sitio. SWBProcess tiene una estructura previamente definida, por lo que no debe editar el nodo llamado _Herramientas de SWBProcess_ en la estructura de páginas. Puede obtener más información sobre la gestión de páginas Web en el [manual](http://www.semanticwebbuilder.org.mx/en_mx/swb/Manuales_Portal_Esoanol/_rid/431/_mto/3/_act/download/doc/Creacion_y_Administracion_de_Paginas_Web.pdf) correspondiente.|

## Edición de la configuración de un sitio de procesos

* Acceder a las pestañas de configración
* Tabla de pestañas

### Activación/desactivación de un sitio de procesos

### Edición de la información principal del sitio
* Tabla de propiedades

### Uso de la papelera de reciclaje del sitio

### Eliminación de sitios Web de procesos


{% include links.html %}
