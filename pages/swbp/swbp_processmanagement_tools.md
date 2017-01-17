---
title: Configuración de las herramientas de proceso
summary: "Esta sección describe las acciones asociadas con la configuración de los elementos reutilizables en un proceso de negocio"
sidebar: swbp_sidebar
permalink: swbp_processmanagement_tools.html
folder: swbp
---

## Herramientas de Proceso
Las herramientas de proceso, descritas en las siguientes secciones, son elementos reutilizables que se organizan en catálogos. Dichas herramientas se ubican en el nodo _Herramientas de Proceso_ {% include inline_image.html class="icon" file="screenshots/icon_processtools.png" %} del árbol de estructura del sitio, como se muestra en la siguiente figura.

{% include image.html class="centered x-small shadow adjusted" file="screenshots/swbp_processtools.png" alt="BPM" %}

## Certificados X509
X509 es un estándar que define, entre otras cosas, el manejo de certificados digitales y comunicación segura en la web y por e-mail. SWBProcess utiliza certificados bajo este estándar para proporcionar firmado electrónico al cierre de las tareas.

{{site.data.alerts.callout_success}}
SWBProcess no utiliza una entidad validadora para procesar los certificados. En su lugar, utiliza los datos en el certificado en asociación con el perfil del usuario para validar la identidad.
{{site.data.alerts.end}}

### Creación de un certificado
Para crear un certificado necesitará un archivo de certificado creado en este estándar (archivo .cer). Puede conseguir este archivo con alguna entidad generadora de certificados.

Deberá hacer click con el botón derecho en el nodo _Certificados X509_ {% include inline_image.html file="screenshots/icon_X509.png" class="icon" %} y seleccionar la opción **Agregar Certificado X509** como se muestra en la siguiente figura.

{% include image.html class="centered shadow adjusted" file="screenshots/swbp_addx509_menu.gif" alt="Opción para agregar certificado" %}

Se presentará el diálogo _Agregar Certificado X509_ como se muestra en la siguiente figura. En el diálogo deberá presionar el botón **Select File** del campo **Archivo**.

{% include image.html class="centered medium shadow adjusted" file="screenshots/swbp_newx509_dialog.png" alt="Diálogo crear certificado" %}

Se mostrará una pantalla de selección donde deberá ubicar su archivo de certificado.

{% include image.html class="centered medium shadow adjusted" file="screenshots/swbp_newx509_selectdialog.png" alt="Diálogo seleccionar certificado" %}

Una vez seleccionado el archivo, se mostrará un mensaje de confirmación de la carga y podrá presionar el botón **Guardar**.

{% include image.html class="centered medium shadow adjusted" file="screenshots/swbp_newx509_confirmdialog.png" alt="Confirmación de carga de certificado" %}

Finalmente, se mostrará en la zona de trabajo el nuevo certificado con la pestaña _Información_ seleccionada por defecto. En el campo **Sujeto** del formulario se presentará la información contenida en el certificado y en el campo **Serie** se mostrará el valor utilizado para asociar el certificado con un perfil de usuario.

{% include image.html class="centered shadow adjusted" file="screenshots/swbp_x509_tabs.png" alt="Pestañas del certificado" %}

### Asociación de un certificado con un perfil de usuario
La asociación de un perfil de usuario con un certificado X509 se realiza mediante el valor del campo **Serie** del certificado. Para ello, deberá primero ubicar ese valor en la pestaña de _Información_ del certificado, como se muestra en la siguiente figura.

{% include image.html class="centered shadow adjusted" file="screenshots/swbp_x509_serial.png" alt="Pestañas del certificado" %}

Posteriormente, deberá acceder a la configuración de los datos del usuario al que desea asociar el certificado. Para ello, puede consultar el procedimiento en la sección [Edición de las propiedades de un usuario](http://localhost:4000/swbp_users.html#edicin-de-las-propiedades-de-un-usuario). Una vez en la pestaña de configuración del usuario, ubique el campo **ID externo** y capture el valor del campo **Serie** del certificado.

{% include image.html class="centered shadow adjusted" file="screenshots/swbp_user_externalID.png" alt="Pestañas del certificado" %}

Finalmente, presione el botón **Guardar** para actualizar la información del usuario. Desde ese momento, la identidad del usuario será relacionada con el certificado referido.

### Modificación de la configuración de un certificado
Para modificar las propiedades de un certificado deberá acceder a la pestaña de información del mismo. Se presentará un formulario donde podrá modificar la información de acuerdo con la siguiente tabla.

|Propiedad|Descripción|
|---|---|
|Archivo|Muestra una ventana de selección para ubicar un archivo .cer|
|Eliminar|Si marca esta casilla, el archivo .cer asociado al certificado será eliminado.|
|Fecha de expiración|Muestra un calendario para establecer una fecha de expiración del certificado.|

### Eliminación de certificados
Podrá eliminar un certificado presionando el botón **Eliminar** en el formulario de la pestaña de información del mismo.

{% include image.html class="centered shadow adjusted" file="screenshots/swbp_x509_removebutton.png" alt="Botón de eliminación" %}

También puede realizar la acción desde el árbol de estructura del sitio, haciendo click con el botón derecho sobre el nombre del certificado y seleccionando la opción **Eliminar**, como se muestra en la siguiente figura.

{% include image.html class="centered small shadow adjusted" file="screenshots/swbp_x509_removeoption.gif" alt="Opción de eliminación del certificado" %}

En cualquier caso, se solicitará confirmación de la acción. Si acepta, el certificado será eliminado y desaparecerá del árbol del sitio.

{% include image.html class="centered medium shadow adjusted" file="screenshots/swbp_x509_deleteconfirm.png" alt="Opción de eliminación del certificado" %}


## Plantillas de notificaciones

## Plantillas de archivos

## Intervalos de ejecución

## Reglas de negocio

## Conexiones a BD

## Servicios web

## Propiedades de asignación

{% include links.html %}
