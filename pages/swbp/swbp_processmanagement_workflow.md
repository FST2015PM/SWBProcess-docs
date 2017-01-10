---
title: Flujo de trabajo
tags: [getting_started]
summary: "Introducción a la gestión de procesos de negocio con SWBProcess"
sidebar: swbp_sidebar
permalink: swbp_processmanagement_workflow.html
folder: swbp
---

## Business Process Management
SemanticWebBuilder process fue diseñado para ayudar a los distintos actores involucrados en la gestión de los procesos de negocio de una organización. Con este objetivo, los componentes integrados en SWBProcess permiten cubrir por completo el ciclo de vida planteado por la metodología Business Process Management (BPM por sus siglas en inglés).

De acuerdo con la definición de Wetzstein et. al.[^wetzstein1], el ciclo de vida de los procesos en BPMN contiene cuatro etapas: Modelado, implementación, ejecución y análisis. La descripción de cada etapa y la manera en que SWBProcess contribuye a su realización se describe en los siguientes párrafos conforme a lo establecido en Pacheco et. al.[^Pacheco1].

* **Modelado:** en esta etapa los analistas del negocio crean un modelo de procesos de negocio con la ayuda de herramientas específicas, estableciendo el orden de las tareas en el modelo. Esta fase es cubierta por _SWBP Modeler_, que soporta el diseño de diagramas de procesos mediante el estándar BPMN 2.0 y los transforma en modelos semánticos de procesos. Adicionalmente, _SWBProcess Documenter_ permite capturar la información de negocio asociada a los procesos y generar un manual en línea.

* **Implementación:** en esta etapa, con la ayuda de los ingenieros en TI, el modelo del proceso es enriquecido con propiedades para convertirlo en un modelo de procesos ejecutable. Esta etapa es cubierta por _SWBProcess Configurator_, que permite la asociación de las propiedades necesarias para la ejecución y despliegue de los procesos en un sistema Web. Adicionalmente, mediante _SWBProcess Forms_, es posible definir las formas de captura y visualización de la información de los procesos conforme a la definición de su modelo semántico.

* **Ejecución:** en esta etapa un motor de procesos crea casos (instancias) a partir de las definiciones en los modelos de procesos ejecutables. El motor de procesos controla la activación de las actividades en el flujo y genera información específica para cada caso. Esta etapa es cubierta por _SWBProcess Engine_ y el componente _Bandeja de Tareas_ del sitio de procesos.

* **Análisis:** en esta etapa los analistas de procesos revisan los datos del desempeño en la ejecución de los distintos casos para identificar mejoras al proceso y tomar decisiones. Esta etapa está cubierta por _SWBProcess Monitor_ y _SWBProcess Reports_, que permiten visualizar la información básica sobre el desempeño de los procesos y generar reportes con información específica de cada caso.

[^wetzstein1]: B. Wetzstein, Z. Ma, A. Filipowska, M. Kaczmarek, S. Bhiri, S. Losada, J.-M. Lopez-Cob, L. Cicurel, "Semantic business process management: A lifecycle based requirements analysis", Workshop on Semantic Business Process and Product Lifecycle Management, 2007.

[^Pacheco1]: H. Pacheco, K. Najera, H. Estrada and J. Solis, "SWB process: A business process management system driven by semantic technologies," 2014 2nd International Conference on Model-Driven Engineering and Software Development (MODELSWARD), Lisbon, 2014, pp. 525-532.


## Flujo de trabajo en SWBProcess
* Modelado de datos
* Configuración de herramientas
* Modelado del proceso
* Configuración del proceso
* Documentación del proceso
* Ejecución del proceso
* Monitoreo del proceso

{% include links.html %}
