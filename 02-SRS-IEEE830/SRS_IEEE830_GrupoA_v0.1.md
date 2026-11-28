#ESPECIFICACION DE REQUISITOS DEL SOFTWARE (SRS)
**Proyecto:** Sistema de gestion de un almacén de colchones.

**Estándar:** IEEE Std. 830-1998.

**Versión:** 1.0

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

### 1.2 Alcance:

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

- **Interfaces de Usuarios:** Pantallas, vistas o paneles principales según el rol (administrador, operario de almacén, transportista/repartidor, cliente), formatos de entrada/salida y navegación básica.
- **Interfaces de Hardware/Software:** Navegador web o escritorio, sistema operativo soportado, base de datos o servicios externos (por ejemplo, pasarela de mapas/geolocalización o lectores de códigos de barras/QR si aplica).

### 3.2 Requisitos Funcionales (Organizados por Módulos):

- Se redactan de forma atómica, verificable y numerada (RF-01, RF-02, ...), indicando Entrada, Proceso y Salida (o formato: "El sistema deberá..."). Agrupados por módulos o cascos de uso del dominio logístico:

#### 3.2.1 Módulo 1:

**Gestión de Usuarios y Roles:** Registro, autentificación y permisos diferenciados (adminsitrador, gestor de almacén, repartidor).

#### 3.2.2 Módulo 2:

**Gestión de Inventario y Almacenes:** Alta/baja/modificación de productos, consulta de stock tiempo real, alertas de stock mínimo y ubicación en almacén.

#### 3.2.3 Módulo 3:

**Gestión de Pedidos y Envíos:** Creación de pedidos, asignación a almacén de origen, generación de etiquetas/códigos de seguimiento y actualización de estados (Pendientes, Preparado, En tránsito, Entregado, Incidencia).

#### 3.2.4 Módulo 4:

**Gestión de Flota y Rutas:** Alta de vehículos (capacidad máxima en peso/volumen, disponibilidad), asignación de envíos a vehículos sin superar su capacidad y planificación/consulta de rutas.

3.2.5 Módulo 5:

**Consultas e Informes:** Historial de movimientos, trazabilidad de un envío por código y reportes básicos de entregas o incidencias.

### 3.3 Requisitos de rendimiento:

- Tiempos máximos de respuesta esperados en operaciones críticas (por ejemplo, consulta de estado de envío o actualización de invetario en menos de 2 segundos) y volumen estimado de pedidos/ usuarios concurrentes.

### 3.4 Modelo del dominio:

- Estándares oblgatorios, arquitectura lógica definida (separación Modelo-Vista-Controlador), normativa aplicable (protección de datos de cliente/destinatarios) o limitaciones de entorno.

### 3.5 Restricciones de diseño:

- Numerados (`RNF-01`,`RNF-02`, ...) con métricas comprobables:
  - **Seguridad:** Control de acceso por rol, cifrado de credenciales y trazabilidad (auditoría) de cambios de estado en los envíos.
  - **Fiabilidad y Disponibilidad:** Integridad transaccional (no descontar stock si falla la creación del pedido) y recuperación ante fallos.
  - **Usabilidad y Mantenibilidad:** Interfaz intuitiva para operarios y arquitectura modular desacoplada.

### 3.6 Atributos del sistema software:

- Entidades principales de información que el sistema debe persistir (Usuarios, Almacenes, Productos, Pedidos, Líneas de Pedido, Envíos, Vehículos, Rutas), sus identificadores clave, relaciones y reglas de integridad (por ejemplo, un pedido no puede quedar sin almacén asignado ni un vehículo superar su carga máxima).

---

## 4. APÉNDICES:
