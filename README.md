# **Table of Contents**

1. [Introduction](#introduction)
2. [Overall Description](#overall-description)
3. [System Features](#system-features)
4. [External Interface Requirements](#external-interface-requirements)
    1. [User Interfaces](#user-interfaces)
    2. [Hardware Interfaces](#hardware-interfaces)
    3. [Software Interfaces](#software-interfaces)
    4. [Communications Interfaces](#communications-interfaces)
5. [Other Nonfunctional Requirements](#other-nonfunctional-requirements)
    1. [Performance Requirements](#performance-requirements)
    2. [Safety Requirements](#safety-requirements)
    3. [Security Requirements](#security-requirements)
    4. [Software Quality Attributes](#software-quality-attributes)
6. [Other Requirements](#other-requirements)

## 1. Introduction

## 2. Overall Description

## 3. System Features

### **3.1 Feature 001 Envío de correos personalizados**
 
```
3.1.1. Description and Priority
    Permite crear correos con contenido personalizado en base a la información de clientes y clientes potenciales.
    Prioridad: High
    Riesgo: 8  
    
3.1.2. Stimulus/Response Sequences
    * El usuario ingresa a la sección de Mail Marketing
    * El sistema muestra la pantalla de Mail Marketing en donde se ve un historial de todos los mails personalizados realizados.
    * El usuario selecciona la opción de nuevo envío de correo.
    * El sistema le muestra el formulario de correos personalizados
    * El usuario Rellena los campos de 
        o Seleccionar grupo de clientes
        o Título del correo
        o Contenido del Correo
    * Selecciona Enviar.  
    
3.1.3 Functional Requirements  

    REQ-001:El usuario debe ser capaz de ver el listados de todos los correos enviados a través del sistema y poder visualizar el detalle de cada correo  
    
    REQ-002: El usuario debe ser capaz de crear un nuevo correo a ser enviado. Debe de poder escoger el grupo de clientes a los cuales desea de enviar el correo.  
    
    REQ-003: En el contenido del correo debe de poder insertarse imágenes, enlaces. Debe de poder ingresar tag especiales en donde luego el sistema reemplace por datos del cliente. Los tag son %NOMBRE% (nombre del cliente) %EMPRESA% (empresa donde trabaja el cliente) %DIRECCION% (dirección del cliente).  
    
    REQ-004: El usuario debe ser capaz de crear correos de respuesta y enlazarlos a un correo, para que este sea enviado en caso de ser respondido el primer correo y así sucesivamente en una cadena de correos.

```    

### **3.2 Feature 002 Cartera de Clientes**

```
3.1.1. Description and Priority
    Creación, modificación, listado y eliminación de Clientes.
    Prioridad: High
    Riesgo: 8  
    
3.1.2. Stimulus/Response Sequences
    * El usuario ingresa a la sección de Cartera de Clientes
    * El sistema muestra la pantalla de Cartera de Clientes en donde se lista todos los clientes del sistema.
    * El usuario selecciona la opción de nueva cliente
    * El sistema le muestra el formulario de registro
    * El usuario Rellena los campos de 
        o Nombre
        o Edad
        o Dirección
        o Empresa
        o Cantidad de familia
        o Enfermedades
        o Salario
        o Selecciona Guardar 
        o El sistema muestra un pop-up indicando que se ha guardado  
        
3.1.3 Functional Requirements  
    REQ-001: El usuario debe ser capaz de ver el listados de todos los clientes.  
    
    REQ-002: El usuario debe ser capaz de crear un nuevo Cliente rellenando un formulario con los siguientes campos Nombre, edad, dirección, empresa, cantidad de familia, seleccionar listado de enfermedades, Salario.  
    
    REQ-003: El usuario debe ser capaz de modificar la información de un cliente.  
    
    REQ-004: El usuario debe ser capaz de eliminar un cliente.  
    
    REQ-005: El usuario debe ser capaz que registrar clientes por batch, cargando archivos csv.

```

### **3.3 Feature 003 Grupo de Clientes**

```
3.1.1. Description and Priority
    Creación, modificación, listado, eliminación de grupo de clientes y asignación de Clientes a un grupo.
    Prioridad: High
    Riesgo: 8  
    
3.1.2. Stimulus/Response Sequences
    * El usuario ingresa a la sección de Grupo de Clientes
    * El sistema muestra la pantalla de Grupo de Clientes en donde se lista todos los grupos de clientes del sistema.
    * El usuario selecciona la opción de nuevo grupo
    * El sistema le muestra el formulario de registro
    * El usuario Rellena los campos de 
        o Nombre
    * Selecciona Guardar 
    * El sistema muestra un pop-up indicando que se ha guardado  
    
3.1.3 Functional Requirements  
    REQ-001: El usuario debe ser capaz de ver el listado de todos los grupos clientes  
    
    REQ-002: El usuario debe ser capaz de crear un nuevo grupo rellenando un formulario con el siguiente campo Nombre.  
    
    REQ-003: El usuario debe ser capaz de modificar la información de un grupo cliente.  
    
    REQ-004: El usuario debe ser capaz de eliminar un grupo de cliente.  
    
    REQ-005: El usuario debe ser capaz de asignar clientes a un grupo.  
    
    REQ-006: El usuario debe ser capaz de subir un archivo de lotes en formato csv para asignar clientes a un grupo.  
```

### **3.4 Feature 004 Blog**

```
3.1.1. Description and Priority
    Creación, modificación, listado, eliminación de blogs.
    Prioridad: Medium
    Riesgo: 6 
    
3.1.2. Stimulus/Response Sequences
    * El usuario ingresa a la sección de blogs
    * El sistema muestra la pantalla de blogs en donde se lista todos los blogs del sistema.
    * El usuario selecciona la opción de nuevo blogs
    * El sistema le muestra el formulario de registro
    * El usuario Rellena los campos de 
        o Título del blog
        o Contenido del blog
    * Selecciona Guardar 
    * El sistema muestra un pop-up indicando que se ha guardado  
    
3.1.3 Functional Requirements  
    REQ-001: El usuario debe ser capaz de ver el listado de todos los blogs incluyendo el link con el cuál se puede ingresar al blog externamente.
    
    REQ-002: El usuario debe ser capaz de crear un nuevo blog rellenando un formulario con los siguientes campos Título del blog, contenido del blog.
    
    REQ-003: El usuario debe ser capaz de modificar la información de un blog.
    
    REQ-004: El usuario debe ser capaz de eliminar un blog.
    
    REQ-005: En el contenido del blog debe permitir insertar imágenes, enlaces, gifs,
    
    REQ-006: El blog debe de tener una sección de comentarios la cual solo los usuarios registrados deben de poder comentar.
    
    REQ-007: El blog debe de tener una sección de descarga para descargar contenido extra. Para poder descargar el contenido el cliente debe de registrarse en un landing page (Feature 006) para luego dejarle descargar el contenido.  
```

### **3.5 Publicaciones a través de la Api de facebook**

```
3.1.1. Description and Priority
    Realización de publicaciones de contenido y promoción de usando el api de Facebook.
    Prioridad: Low
    Riesgo: 2
    
3.1.2. Stimulus/Response Sequences
    * El usuario ingresa a la sección de publicidad para Facebook
    * El sistema muestra la pantalla de publicidad para Facebook en donde se ve un historial de todas las publicaciones realizadas.
    * El usuario selecciona la opción de nueva publicación
    * El sistema le muestra el formulario de publicaciones
    * El usuario Rellena los campos de 
        o Título de publicidad
        o Tiempo de duración
        o Pago de la publicidad por ciclo de vida o por cantidad de vistas 
        o Cantidad del pago
        o Contenido de la publicidad
    * Selecciona Aceptar 
    * El sistema muestra un pop-up indicando que se ha realizado la publicación
    
3.1.3 Functional Requirements  
    REQ-001:El usuario debe ser capaz de ver el listados de todas publicaciones realizadas a través del sistema y poder visualizar el detalle de cada publicación  
    
    REQ-002: El usuario debe ser capaz de crear una nueva publicación, rellenando un formulario con los siguientes campos título de publicidad, tiempo de duración, tipo de pago de publicidad ya sea por ciclo de vida o por cantidad de vistas, cantidad del pago y el contenido de la publicidad.
  
```

### **3.6 Feature 006 Landing page**

```
3.1.1. Description and Priority
    Pagina de registro de datos del cliente.
    Prioridad: High
    Riesgo: 9
    
3.1.2. Stimulus/Response Sequences
    * El cliente ingresa a la página de landing page
    * El sistema muestra la pantalla de landing page.
    * El cliente Rellena los campos de 
        o Nombre
        o Edad
        o Dirección
        o Empresa(no obligatorio)
        o Cantidad de familia(no obligatorio)
        o Enfermedades(no obligatorio)
        o Salario(no obligatorio)
    * Selecciona Enviar 
    * El sistema lo reenvía a la página que solicita el cliente.

    
3.1.3 Functional Requirements  
    REQ-001: El cliente debe de ser capaz de rellenar los campos de nombre, edad, dirección, empresa, cantidad de familia, enfermedades, salario. Los campos obligatorios son Nombre, edad y dirección. Estos datos deben de ser registrados en el sistema creando un cliente y ser asignados automáticamente a un grupo configurable.
    
    REQ-002: El landing page debe de ser inicializado con una página para ser direccionada. En caso que el cliente se registre entonces debe de ser redireccionado.
    
    REQ-003: El landing page debe de mostrar una opción a etiquetar permitiendo a la empresa enviar correo de ofertas y promociones.
    
    REQ-004: El sistema debe de enviar un correo personalizado a los clientes que se registren en el landing page.

```

### **3.7 Feature 007 Reportes**

```
3.1.1. Description and Priority
    Se deben de generar reportes de Cantidad de clientes registrados, cantidad de vistas de publicaciones, cantidad de vista de blogs, cantidad de mail enviados, cantidad de mails respondidos.
    Prioridad: Medium
    Riesgo: 5
    
3.1.2. Stimulus/Response Sequences
    * El usuario ingresa a la página de reportes
    * El sistema muestra la pantalla de reportes
    * El usuario selecciona el reporte que desea ver
    * El usuario Rellena los campos de 
        o Rango de fechas
    * Selecciona generar 
    * Se muestra el reporte con los criterios
    * Selecciona exportar y selecciona el tipo (Excel, pdf)
    * Se descarga el reporte
    
3.1.3 Functional Requirements  
   REQ-001: Generar reporte de cantidad de clientes registrados en un determinado rango de fechas.
   
   REQ-002: Generar reporte de vistas de publicaciones en un determinado rango de fechas.
   
   REQ-003: Generar reporte de cantidad de vistas en blogs en un determinado rango de fechas.
   
   REQ-004: Generar reporte de cantidad de mails enviados en un determinado rango de fechas.
   
   REQ-005: Generar reporte de cantidad de mails respondidos en un determinado rango de fechas.
   
   REQ-006: Se debe de poder exportar los reportes en formato Excel o pdf.
```

## 4. External Interface Requirements

## 4.1 User Interfaces
>Mocku Login

![](/login.png)

>Mockup Menu

![](/menu.png)

The user must create a login page when accessing any page in case he has not done it before. Administrative tasks must have a Ui interface.
The Facebook interface should allow you to send publications without having to log in repeatedly. The e-mail delivery interface must follow these as there may be some error in the shipment.

## 4.2 Hardware Interfaces
All server-side components must execute on server-class computers. All client-side components
must execute on workstation-class and personal-class computers.

## 4.3 Software Interfaces
The software interface must follow the Model-View-Controller (**MVC**) model to render and model data objects. The interface must be able to connect to a database to store the different data of the system. In some cases the source and destination formats must include **HTML** and Comma Separated Value (**CSV**).

## 4.4 Communications Interfaces

The communication architecture must follow the **client-server** model. The communication must be through **HTTP** Secure **(HTTPS)**. 

Between the client and the server must use a web service that complies with REST, both for the web and for communications with other platforms such as Facebook.

## 5 Other Nonfunctional Requirements

## 5.1 Security Requirements
The percentage of error when sending an email must be as small as possible.
Security in the management of customer information since data are handled strictly by people.
