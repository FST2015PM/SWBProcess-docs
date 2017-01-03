---
title: Prerequisitos
tags: [setup]
keywords: release notes, announcements, what's new, new features
sidebar: swbp_sidebar
permalink: swbp_prerequisites.html
folder: swbp
---

## JDK 1.7 o superior

Aunque SWB Process puede desplegarse utilizando OpenJDK, se recomienda el uso de la [versión de Oracle](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html).

## Servidor de Base de Datos

SWB Process solo se podrá instalar en Bases de Datos que se encuentren soportadas en los conectores SDB y TDB, por  ejemplo  MySQL, Oracle 10gR2, SQL Server 2005, etc. Para mayor información sobre  dichos  conectores  dirigirse  a  la  [documentación  del  proyecto  jena](http://jena.apache.org/documentation/sdb/databases_supported.html).

## Servidor de aplicaciones Java

Consideraciones  Importantes:  SWB  solo  se  puede  instalar  en  Java  Application Servers,  como  por  ejemplo,  Jetty,  Tomcat,  GlassFish,  JBoss, WebLogic.
(Para mayor información  revise la documentacion  en http://www.oracle.com/technetwork/java/javaee/overview/compatibility-jsp-136984.html)

## Archivo WAR de la aplicación

Descargar  el  archivo  “swb.war”  de  http://www.semanticwebbuilder.org.mx/en/swb/SWB_Portal, o "swbp.war" de http://www.semanticwebbuilder.org.mx/en/swb/SWB_Process; este  archivo  se puede  descomprimir  como  .jar  o  con  algun software de compresion  y  posteriormente  el contenido  se  transfiere a la carpeta webapps dentro del Tomcat.

## Requerimientos de Hardware

Dada la gran variedad y velocidad de cambio de los diversos procesadores actuales y diversos modelos de entrega de poder de computo (Ambientes virtualizados y de nube), para los que existe una implementación de la máquina virtual java, recomendamos que como MÍNIMO se cuente con el procesamiento equivalente a un procesador Xeon 2007 a 1Ghz (1vCore) y 600MB de RAM.

De manera general requerimos 2vCore y 1.7GB de RAM


{% include links.html %}
