#ESPECIFICACION DE REQUISITOS DEL SOFTWARE (SRS)
**Proyecto:** Sistema de gestion de un almacén de colchones.

**Estándar:** IEEE Std. 830-1998.

**Versión:** 1.1.1  

**Fecha:** 11/12/2026 

**Equipo de Desarrollo:** Adrian Canillas, Alejandro Martínez, Alejandro Vazquez, Alexandru Luis Budurea, Daniel del Molino, Lucas Durán, Lucas Alvarez, Matei Mihai Popescu.

--- 
## ÍNDICE DE CONTENIDOS
1. [1. INTRODUCCIÓN](#1-introducción)
    * [1.1 Propósito](#11-propósito)
    * [1.2 Alcance](#12-alcance)
    * [1.3 Definiciones, Acrónimos y Abreviaturas](#13-definiciones-acrónimos-y-abreviaturas)
    * [1.4 Referencias](#14-referencias)
    * [1.5 Resumen](#15-resumen)
2. [2. DESCRIPCIÓN GENERAL](#2-descripción-general)
   * [2.1 Perspectiva del Producto](#21-perspectiva-del-producto)
   * [2.2 Funciones del Producto](#22-funciones-del-producto-alto-nivel)
   * [2.3 Características de los Usuarios](#23-características-de-los-usuarios)
   * [2.4 Restricciones](#24-restricciones)
   * [2.5 Supuestos y Dependencias](#25-supuestos-y-dependencias)
   * [2.6 Requisitos Futuros](#26-requisitos-futuros)
3. [3. REQUISITOS ESPECÍFICOS](#3-requisitos-específicos)
   * [3.1 Requisitos de Interfaces Externos](#31-requisitos-de-interfaces-externos)
   * [3.2 Requisitos Funcionales](#32-requisitos-funcionales-organizados-por-módulos)
   * [3.2.1 Módulo 1:](#321-módulo-1)
   * [3.2.2 Módulo 2: Compras y Recepción de Proveedores](#322-módulo-2)
   * [3.2.3 Módulo 3: Salidas y Despacho de Pedidos](#323-módulo-3)
   * [3.3 Requisitos de Rendimiento](#33-requisitos-de-rendimiento)
   * [3.4 Modelo del Dominio](#34-modelo-del-dominio)
   * [3.5 Restricciones de Diseño](#35-restricciones-de-diseño)
   * [3.6 Atributos del Sistema Software](#36-atributos-del-sistema-software)
4. [4. APÉNDICES](#4-apéndices)
---
---
## 1. INTRODUCCIÓN 

### 1.1 Propósito:
El propósito fundamental de este documento de Especificación de Requisitos Software (SRS, *Software Requirements Specification*) es definir de manera formal, completa, no ambigua y verificable los requisitos del **Sistema de Gestión de Almacén de Colchones (SGAC**). La SRS establece la base contractual e ingenieril para un acuerdo explícito entre los desarrolladores y las partes interesadas sobre el comportamiento que debe tener el software. Asimismo, este documento sirve como el punto de referencia indispensable para reducir el esfuerzo de desarrollo, estimar costes, planificar el proyecto y guiar las tareas de validación y verificación de pruebas.

Esta especificación se dirige a una amplia audiencia con roles y responsabilidades diferentes respecto al ciclo de vida del software:

* **Cliente y dirección de operaciones:** Responsables de evaluar y validar que los servicios y funciones especificados cubren las necesidades operativas y de negocio del almacén.
* **Equipo de desarrollo y arquitectura:** Ingenieros encargados de usar esta especificación como base para la fase de diseño técnico, el modelado UML en la herramienta *CASE IBM RATIONAL SOFTWARE ARCHITECT (RSA)* y la posterior codificación.
* **Equipo de SQA (Software quality assurance) y evaluadores:** Revisores e inspectores cuyos criterios para evaluar la calidad, realizar RTFs (Revisiones técnicas formales) y diseñar casos de prueba incluirán las especificaciones contenidas en este documento.
* **Usuarios finales (Jefes de compras, gestores de ventas y trabajadores del almacén):** Personas que interactuarán con el sistema de manera directa y requieren de la verificación de la usabilidad y de la adecuación de las operaciones descritas.

Como elemento de configuracion software (ECS) compuesto, este documento está inmovilizado como línea base y sujeto a control formal de versiones y cambios dentro de la gestión de la configuración del software (GCS).

### 1.2 Alcance:
El producto software se identifica oficialmente con el nombre de ***Sistema de Gestión de Almacén de Colchones (SGAC)***.

<u>Funcionalidad y beneficios del sistema:</u>
 El sistema automatizará y optimizará la gestión logística integral de un almacén especializado en productos de descanso, transformando la información de entrada en salidas estructuradas.

 Entre sus objetos operativos y beneficios principales se incluyen:

 1. **Control de inventario y ubicaciones:** Registro en tiempo real de las existencias físicas organizadas por sus respectivos atributos (modelo, medidas, materiales y niveles de firmeza), asignando ubicaciones precisas dentro del almacén, organizado en pasillos y estanterías.
 2. **Gestión de entradas y recepción de lotes:** Registro y validación de recibos de entrada provenientes de fabricantes de colchones, etiquetado de lotes entrantes mediante códigos numéricos (*EAN-13/RFID*) y control de la capacidad máxima de almacenamiento.
 3. **Gestión de salidas y despacho:** Procesamiento de pedidos de venta solicitados por los clientes, generación automática de hojas de extracción (picking) optimizadas por rutas internas de pasillos y expedición de mercancía.
 4. **Trazabilidad e informes:** Seguimiento del historial de movimiento de cada lote e integración de consultas rápidas sobre existencias disponibles y reservadas.

<u>Exclusiones explícitas del sistema:</u>
 Para delimitar su ámbito con precisión y evitar ambigüedades, se establecen múltiples funciones que el sistema no realizará:
 
 * No gestionará la nómina, horarios ni la administración de recursos humanos del personal asignado al almacén.
 * No realizará el seguimiento por GPS ni la navegación de flota de los vehículos de transporte fuera de las instalaciones del almacén.
 * No procesará directamente pasarelas de pago bancario en linea ni la contabilidad financiera general de la empresa.

### 1.3 Definiciones, Acrónimos y Abreviaturas:

### 1.4 Referencias:
1. IEEE Std. 830-1998, *IEEE Recommended Practice for Software Requirements Specifications*.
2. Guía docente del Proyecto - Ingeniería del Software I.

### 1.5 Resumen:

--- 
## 2. DESCRIPCIÓN GENERAL 

### 2.1 Perspectiva del Producto:

### 2.2 Funciones del Producto (Alto Nivel):

### 2.3 Características de los Usuarios:

### 2.4 Restricciones:

### 2.5 Supuestos y Dependencias:

### 2.6 Requisitos Futuros:

---
## 3 REQUISITOS ESPECÍFICOS
### 3.1 Requisitos de Interfaces Externos:

### 3.2 Requisitos Funcionales (Organizados por Módulos):

#### 3.2.1 Módulo 1:

#### 3.2.2 Módulo 2:

#### 3.2.3 Módulo 3:

#### 3.2.n Módulo n:
(esto es una plantilla, puede haber tantos módulos como consideremos)

### 3.3 Requisitos de rendimiento:

### 3.4 Modelo del dominio: 

### 3.5 Restricciones de diseño:

### 3.6 Atributos del sistema software:

---
## 4. APÉNDICES:
