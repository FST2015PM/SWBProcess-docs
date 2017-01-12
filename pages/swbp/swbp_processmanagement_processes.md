---
title: Procesos y grupos de procesos
tags: [getting_started]
sidebar: swbp_sidebar
permalink: swbp_processmanagement_processes.html
folder: swbp
---

## Grupos de procesos
SemanticWebBuilder Process permite organizar los procesos de negocio en grupos y subgrupos, de manera que su navegación y búsqueda sea más sencilla, obedeciendo a una estructura jerárquica. Los grupos y subgrupos en SWBProcess se muestran en el árbol de estructura del sitio, bajo el nodo denominado _Procesos_ {% include inline_image.html file="screenshots/icon_processgroup.png" %}, como se muestra en la siguiente figura.

{%include image.html class="centered x-small shadow adjusted" file="screenshots/swbp_processgroups.png" alt="Estructura de grupos de procesos"%}

{{site.data.alerts.callout_success}}
Debe considerar que la navegación por la documentación del sitio de procesos obedece a la estructura de grupos y subgrupos definida en el sitio Web de procesos.
{{site.data.alerts.end}}

### Creación de grupos de procesos
Usted podrá crear un grupo de procesos de primer nivel haciendo click con el botón derecho del ratón en el nodo _Procesos_ {% include inline_image.html file="screenshots/icon_processgroup.png" %} y seleccionando la opción **Agregar grupo de procesos**.

{% include image.html class="centered small shadow adjusted" file="screenshots/swbp_processgroups_addoption.gif" alt="Opción Agregar grupo de procesos" %}

Se mostrará el diálogo _Agregar grupo de proceos_, donde deberá capturar un título para el nuevo grupo, como se muestra en la siguiente figura.

{% include image.html class="centered small shadow adjusted" file="screenshots/swbp_processgroups_adddialog.png" alt="Diálogo Agregar grupo de procesos" %}

Finalmente, deberá presionar el botón **Guardar**. Tenga en cuenta que los títulos no son únicos, es decir, pueden repetirse si así lo desea. El nuevo grupo de procesos se mostrará en estado inactivo bajo el nodo de procesos.

{% include image.html class="centered x-small shadow adjusted" file="screenshots/swbp_processgroups_groupadded.png" alt="Nuevo grupo creado" %}

{{site.data.alerts.callout_warning}}
Los procesos contenidos en grupos de procesos inactivos no son mostrados en la navegación de la documentación en el sitio Web de procesos. Tampoco son mostrados en los componentes para creación de instancias de procesos.
{{site.data.alerts.end}}

Adicionalmente, en la zona de trabajo se mostrarán las pestañas de configuración del grupo de procesos con la pestaña _Información_ seleccionada por defecto. en esta pestaña podrá modificar las propiedades del grupo.

{% include image.html class="centered shadow adjusted" file="screenshots/swbp_processgroup_tabs.png" alt="Pestañas de configuración del grupo de procesos" %}

Para crear un grupo de procesos en un nivel distinto, repita el procedimiento haciendo click con el botón derecho del ratón sobre el subgrupo deseado.

### Activación/desactivación de un grupo de procesos
Podrá activar o desactivar un grupo de procesos marcando o desmarcando la casilla del campo **Activo** en el formulario de su pestaña de información.

{%include image.html class="centered shadow adjusted" file="screenshots/swbp_processgroup_active.png" alt="Casilla de activación del grupo"%}

También puede realizar la acción desde el árbol de estructura, haciendo click con el botón derecho sobre el nombre del grupo y seleccionando la opción **Activar** o **Desactivar** según corresponda, como se muestra en la siguiente figura.

{%include image.html class="centered small shadow adjusted" file="screenshots/swbp_processgroup_activemenu.gif" alt="Opción de activación del grupo"%}

En cualquier caso, el icono del grupo cambiará de acuerdo con la configuración. Éste será azul {% include inline_image.html file="screenshots/icon_processgroup_active.png" %} cuando el grupo esté activo y rojo {% include inline_image.html file="screenshots/icon_processgroup_inactive.png" %} cuando el grupo esté inactivo.

### Reorganización de grupos de procesos
Puede reorganizar los grupos y subgrupos de procesos arrastrando los elementos en el árbol como se muestra en la siguiente figura.

{%include image.html class="centered shadow adjusted" file="screenshots/swbp_processgroup_move.gif" alt="Reorganización de grupos"%}

Se solicitará confirmación de la acción. Si acepta, el grupo se moverá como hijo del elemento al cual lo arrastró.

{%include image.html class="centered medium shadow adjusted" file="screenshots/swbp_processgroup_moveconfirm.png" alt="Confirmación de movimiento de grupos"%}

### Eliminación de un grupo de procesos
Podrá eliminar un grupo de procesos presionando el botón **Eliminar** en el formulario de la pestaña de información del mismo.

{%include image.html class="centered shadow adjusted" file="screenshots/swbp_processgroup_delete.png" alt="Botón de eliminación"%}

También puede realizar la acción desde el árbol de estructura, haciendo click con el botón derecho sobre el nombre del grupo y seleccionando la opción **Eliminar**, como se muestra en la siguiente figura.

{%include image.html class="centered shadow adjusted" file="screenshots/swbp_processgroup_removeoption.gif" alt="Opción de eliminación del grupo"%}

En cualquier caso, se solicitará confirmación de la acción. Si acepta, el grupo será eliminado y desaparecerá del acordeón de estructura de sitios.

{%include image.html class="centered medium shadow adjusted" file="screenshots/swbp_processgroup_confirmdelete.png" alt="Confirmación de eliminación del grupo"%}

{% include links.html %}
