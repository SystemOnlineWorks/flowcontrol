# MANUAL DE USUARIO
# FlowControl Print
# Software de Facturación Profesional integrado con QuickBooks para Honduras

---

**Versión del documento:** 1.0  
**Fecha:** 03 de noviembre de 2026  
**Aplicativo:** FlowControl Print v1.0.0.0  
**Plataforma:** Windows Desktop (.NET Framework)  
**Integración:** QuickBooks Desktop (Pro, Premier, Enterprise)

---

## Tabla de Contenidos

1. [Introducción](#1-introducción)
2. [Requisitos del Sistema](#2-requisitos-del-sistema)
3. [Instalación y Primer Arranque](#3-instalación-y-primer-arranque)
4. [Activación de Licencia](#4-activación-de-licencia)
5. [Interfaz Principal](#5-interfaz-principal)
6. [Conexión con QuickBooks](#6-conexión-con-quickbooks)
7. [Gestión de Empresas](#7-gestión-de-empresas)
8. [Gestión de CAI (Código de Autorización de Impresión)](#8-gestión-de-cai)
9. [Gestión de Transacciones](#9-gestión-de-transacciones)
10. [Impresión de Facturas](#10-impresión-de-facturas)
11. [Manejo de Facturas Exoneradas](#11-manejo-de-facturas-exoneradas)
12. [Sistema de Logs](#12-sistema-de-logs)
13. [Cumplimiento SAR Honduras](#13-cumplimiento-sar-honduras)
14. [Preguntas Frecuentes](#14-preguntas-frecuentes)
15. [Soporte Técnico](#15-soporte-técnico)

---

## 1. Introducción

### 1.1 ¿Qué es FlowControl Print?

**FlowControl Print** es un software de facturación profesional diseñado específicamente para el mercado hondureño, que se integra de forma nativa con **QuickBooks Desktop** para emitir facturas que cumplen con todos los requisitos del **Servicio de Administración de Rentas (SAR)** de Honduras.

### 1.2 Características Principales

- ✅ **Integración total con QuickBooks Desktop** (Pro, Premier y Enterprise)
- ✅ **Gestión de CAI** con múltiples autorizaciones y rangos autorizados
- ✅ **Formato fiscal SAR** completo: valor en letras, RTN, importes exonerados, gravados 15% y 18%
- ✅ **Manejo de exonerados**: correlativos de orden de compra exenta, constancias de registro exonerado y SAG
- ✅ **RTN automático** de clientes desde campos personalizados de QuickBooks
- ✅ **Impresión profesional** con logo, paginación automática y multi-copia
- ✅ **Licencia de por vida** con validación en línea
- ✅ **Multi-empresa**: configuración de varias empresas con sus propios datos

### 1.3 Público Objetivo

Este aplicativo está dirigido a:
- Contadores y administradores de empresas hondureñas
- Empresas que ya utilizan QuickBooks Desktop como sistema contable
- Negocios que requieren cumplir con la normativa fiscal del SAR

---

## 2. Requisitos del Sistema

<!-- TAG: Requisitos, Hardware, Software, Instalacion -->
<!-- AUDIENCE: Tecnico, Administrador -->
<!-- LEVEL: Basico -->
<!-- SEARCH: requisitos sistema windows quickbooks .net framework -->

### 2.1 Requisitos de Hardware

| Componente | Mínimo | Recomendado |
|------------|--------|-------------|
| Procesador | Intel Core i3 | Intel Core i5 o superior |
| Memoria RAM | 4 GB | 8 GB o superior |
| Espacio en disco | 500 MB libres | 1 GB libres |
| Resolución de pantalla | 1024 x 768 | 1920 x 1080 |
| Impresora | Compatible con Windows | Impresora láser a color |

### 2.2 Requisitos de Software

| Componente | Versión Requerida |
|------------|-------------------|
| Sistema Operativo | Windows 10 / Windows 11 (64 bits) |
| .NET Framework | 4.6 o superior |
| QuickBooks Desktop | Pro, Premier o Enterprise (cualquier versión compatible con QBFC16) |
| QuickBooks File | Archivo .QBW válido y accesible |

### 2.3 Requisitos de Red

- Conexión a Internet **solo para la activación inicial de la licencia**
- Una vez activada, la licencia queda registrada y **no requiere conexión permanente**

---

## 3. Instalación y Primer Arranque

### 3.1 Proceso de Instalación

1. Descargue el instalador de FlowControl Print desde el sitio oficial.
2. Ejecute el archivo de instalación con permisos de administrador.
3. Siga las instrucciones del asistente de instalación.
4. Al finalizar, se creará un acceso directo en el escritorio y en el menú de inicio.

### 3.2 Primer Arranque

Al ejecutar FlowControl Print por primera vez, se mostrará la ventana principal con el siguiente aspecto:

---

![IMAGEN 1 - Pantalla Inicial del Aplicativo](https://i.postimg.cc/VLPvqp53/image.png)

**Descripción de la Imagen 1:**
- **Barra de título:** Muestra el nombre de la empresa y el CAI activo seleccionado.
- **Barra de menú:** Opciones (Empresa, Preferencias, Tema, Licencia) y Logs.
- **Panel izquierdo:** Botones de acción (Conectar, Empresas, CAI), lista de CAI disponibles, campo de búsqueda por número de referencia, y panel de información.
- **Panel derecho (gris):** Área donde se cargarán las transacciones de QuickBooks.
- **Barra de estado inferior:** Muestra el CAI activo, fecha y rango autorizado.

---

## 4. Activación de Licencia

<!-- TAG: Licencia, Activacion, GitHub, Validacion -->
<!-- AUDIENCE: Administrador, Tecnico -->
<!-- LEVEL: Intermedio -->
<!-- SEARCH: licencia activar validar numero github token -->
<!-- RELACIONADO: 15-Soporte-Tecnico -->

### 4.1 ¿Por qué se requiere una licencia?

FlowControl Print utiliza un sistema de licenciamiento basado en GitHub para validar la autenticidad del software. Cada instalación requiere un **número de licencia único** que se valida en línea contra los servidores del desarrollador.

### 4.2 Proceso de Activación

1. Al hacer clic en **Conectar** por primera vez, se abrirá automáticamente el formulario de licencia.
2. También puede acceder manualmente desde: **Opciones → Licencia**.

**Formulario de Licencia:**

![IMAGEN 2 - Licencia](https://i.postimg.cc/ydt4HDDY/image.png)


3. Ingrese el número de licencia proporcionado por el administrador.
4. Haga clic en **Validar Licencia**.
5. El sistema consultará el repositorio de GitHub para verificar la validez.
6. Si la licencia es válida:
   - Se registrará la fecha de activación.
   - Se creará el archivo `licence.md` en la carpeta del aplicativo.
   - El formulario se cerrará y podrá continuar.

### 4.3 Mensajes de Error

| Mensaje | Causa | Solución |
|---------|-------|----------|
| "Número de licencia invalido contacte al administrador" | Licencia no existe en el repositorio | Verifique el número con el administrador |
| "Debe registrar una licencia valida para continuar" | No se ha activado la licencia | Active la licencia antes de conectar |

> **Importante:** La licencia es **de por vida** y queda registrada bajo su control. No requiere conexión permanente a Internet después de la activación inicial.

---

## 5. Interfaz Principal

### 5.1 Componentes de la Interfaz

La interfaz de FlowControl Print se divide en las siguientes secciones:

#### 5.1.1 Barra de Menú Superior

| Menú | Opciones | Descripción |
|------|----------|-------------|
| **Opciones** | Empresa | Abre el formulario de datos de la empresa |
| | Preferencias | Configuración general (en desarrollo) |
| | Tema → Claro / Oscuro | Cambia el tema visual |
| | Licencia | Abre el formulario de activación de licencia |
| **Logs** | — | Abre el visor de registros del sistema |

#### 5.1.2 Panel de Control Izquierdo

| Control | Función |
|---------|---------|
| **Conectar** | Inicia la sesión con QuickBooks Desktop |
| **Empresas** | Abre el formulario de datos de la empresa emisora |
| **CAI** | Abre el formulario de registro de Código de Autorización de Impresión |
| **Lista de CAI** | Muestra las autorizaciones CAI registradas (selección con doble clic) |
| **Campo de búsqueda** | Filtra transacciones por número de referencia |
| **Buscar** | Ejecuta la búsqueda |
| **Limpiar** | Limpia el filtro y recarga todas las transacciones |
| **Combo de filtros** | Filtros adicionales (Descuentos, Subtotales, Impuestos) |
| **Panel de información** | Muestra detalles de la transacción seleccionada |

#### 5.1.3 Panel de Transacciones (Derecho)

| Control | Función |
|---------|---------|
| **Anterior** | Navega a la página anterior de transacciones |
| **Siguiente** | Carga la siguiente página de transacciones |
| **DataGridView** | Tabla con las transacciones de QuickBooks |
| **Barra de estado** | Muestra el CAI activo, fecha y rango autorizado |

### 5.2 Barra de Estado

La barra de estado inferior muestra información importante en tiempo real:

![IMAGEN 3 - Barra inferior](https://i.postimg.cc/wjTWw6Bm/image.png)

---

## 6. Conexión con QuickBooks

### 6.1 Requisitos Previos

Antes de conectar FlowControl Print con QuickBooks, asegúrese de:

1. ✅ QuickBooks Desktop esté **abierto y con sesión iniciada**.
2. ✅ El archivo de compañía (.QBW) esté **accesible**.
3. ✅ Tenga permisos de administrador en Windows.
4. ✅ La licencia de FlowControl Print esté **activada**.

### 6.2 Proceso de Conexión

1. Haga clic en el botón **Conectar** en el panel izquierdo.

2. El aplicativo verificará si existe una licencia válida. Si no existe, se abrirá el formulario de licencia.

3. Se mostrará un overlay (pantalla de carga) con el mensaje:

![IMAGEN 4 - Overlay](https://i.postimg.cc/13tHpJWY/image.png)


4. El sistema detectará automáticamente si QuickBooks está en ejecución:
   - **Si QBW está abierto:** Intentará establecer la conexión directamente.
   - **Si QBW no está abierto:** Mostrará el mensaje "Debe iniciar sesión en QuickBooks" e intentará reconectar periódicamente.

5. Una vez conectada la sesión, el overlay se cerrará y comenzará la carga de datos:
   - Descuentos y subtotales
   - Códigos de impuestos (SalesTaxCodes)
   - Transacciones (Invoices y SalesReceipts)

### 6.3 Mensajes de Estado

| Estado | Significado |
|--------|-------------|
| "Conectando a QuickBooks…" | Iniciando sesión con QB |
| "QuickBooks esta listo!" | Conexión exitosa |
| "Error de conexión." | No se pudo conectar (QB cerrado o archivo no encontrado) |
| "Cargando datos" | Obteniendo transacciones e ítems |
| "Leyendo Transacciones" | Cargando lista de facturas |
| "Transacciones obtenidas exitosamente!" | Datos cargados correctamente |

### 6.4 Solución de Problemas de Conexión

| Problema | Causa Probable | Solución |
|----------|----------------|----------|
| "No se pudo conectar a QuickBooks" | QB no está abierto | Abra QuickBooks e inicie sesión |
| "Debe iniciar sesión en QuickBooks" | QB cerrado durante el intento | Mantenga QB abierto |
| Error de archivo .QBW | Ruta incorrecta o archivo corrupto | Verifique la ruta del Company File |
| La aplicación se cierra sola | QB no está instalado | Instale QuickBooks Desktop |

---

## 7. Gestión de Empresas

### 7.1 Acceso al Formulario de Empresa

Existen dos formas de acceder al formulario de datos de la empresa:

1. **Botón "Empresas"** en el panel izquierdo.
2. **Menú Opciones → Empresa**.

### 7.2 Formulario de Empresa

---

![IMAGEN 5 - Empresa](https://i.postimg.cc/k4dKhcc5/image.png)

### 7.3 Campos del Formulario

| Campo | Obligatorio | Descripción |
|-------|-------------|-------------|
| **Empresa** | ✅ Sí | Nombre legal de la empresa emisora |
| **RTN** | ✅ Sí | Registro Tributario Nacional (15 dígitos) |
| **Dirección** | ❌ No | Dirección fiscal completa de la empresa |
| **Teléfono** | ❌ No | Número de teléfono de contacto |
| **Correo** | ❌ No | Correo electrónico (valida formato) |
| **FilePath** | ❌ No | Ruta del archivo .QBW (oculto, se gestiona internamente) |

### 7.4 Botones de Acción

| Botón | Función |
|-------|---------|
| **Guardar** | Valida los campos obligatorios y guarda los datos en `Company.md` |
| **Limpiar** | Limpia todos los campos (solicita confirmación) |
| **Cancelar** | Cierra el formulario sin guardar |
| **Sincronizar** | Obtiene los datos directamente desde QuickBooks (CompanyQueryRq) |

### 7.5 Sincronización con QuickBooks

El botón **Sincronizar** permite obtener automáticamente los datos de la empresa desde el archivo de compañía de QuickBooks:

1. Haga clic en **Sincronizar**.
2. Se mostrará un overlay: "Obteniendo datos de QuickBooks..."
3. El sistema ejecutará una consulta `CompanyQueryRq` a QuickBooks.
4. Los campos **Empresa**, **Dirección**, **Teléfono** y **Correo** se llenarán automáticamente.
5. El usuario puede modificar los datos antes de guardar.

> **Nota:** El RTN debe ingresarse manualmente ya que no es un campo estándar de QuickBooks. Se recomienda configurarlo como un campo personalizado (Custom Field) en QuickBooks para futuras versiones.

### 7.6 Validaciones

- **Empresa:** No puede estar vacío.
- **RTN:** No puede estar vacío.
- **Correo:** Si se ingresa, debe tener un formato válido (usuario@dominio.com).

---

## 8. Gestión de CAI

### 8.1 ¿Qué es el CAI?

El **Código de Autorización de Impresión (CAI)** es un código alfanumérico otorgado por el SAR de Honduras que autoriza a una empresa a emitir facturas dentro de un rango específico de correlativos y durante un período determinado.

**Formato del CAI:** `XXXXXX-XXXXXX-XXXXXX-XXXXXX-XXXXXX-XX`

### 8.2 Acceso al Formulario de CAI

1. Haga clic en el botón **CAI** en el panel izquierdo.
2. También puede acceder desde el menú de navegación (en la versión MainMenu).

### 8.3 Formulario de Registro de CAI

---

![IMAGEN 6 - CAI](https://i.postimg.cc/FsqfBpr2/image.png)

### 8.4 Campos del Formulario

| Campo | Obligatorio | Formato | Descripción |
|-------|-------------|---------|-------------|
| **CAI** | ✅ Sí | `XXXXXX-XXXXXX-XXXXXX-XXXXXX-XXXXXX-XX` | Código de autorización del SAR |
| **Fecha Límite de Emisión** | ✅ Sí | Fecha (dd/MM/yyyy) | Fecha máxima para emitir facturas con este CAI |
| **Desde** | ✅ Sí | `000-000-00-00000000` | Correlativo inicial del rango autorizado |
| **Hasta** | ✅ Sí | `000-000-00-00000000` | Correlativo final del rango autorizado |

### 8.5 Validaciones del Formulario

El sistema realiza las siguientes validaciones antes de guardar:

1. **CAI no vacío:** El campo CAI debe contener al menos un carácter.
2. **Desde y Hasta no vacíos:** Ambos campos de rango deben estar completos.
3. **Formato de 16 caracteres:** `Desde` y `Hasta` deben tener exactamente 16 caracteres numéricos (sin contar guiones).
4. **Tercer par = "01":** En ambos campos, el tercer par de números debe ser `01`.
5. **Últimos 8 dígitos > 0:** Los últimos 8 números deben ser mayores a cero.
6. **Hasta > Desde:** El valor de `Hasta` debe ser mayor que el de `Desde`.

### 8.6 Detección de Duplicados

El sistema valida automáticamente que no existan CAI duplicados basándose en:
- El código CAI
- El correlativo Desde
- El correlativo Hasta

Si se detecta un duplicado, se mostrará una alerta.

### 8.7 Selección de CAI Activo

Una vez registrados los CAI, aparecen en la lista del panel izquierdo:

![IMAGEN 7 - Listado de CAI](https://i.postimg.cc/y8cNrzrk/image.png)

**Para seleccionar un CAI activo:**
1. Haga **doble clic** sobre el CAI deseado en la lista.
2. El sistema guardará la selección en `CAI.txt`.
3. La barra de título y la barra de estado se actualizarán con el CAI seleccionado.
4. El título de la ventana mostrará: `Transacciones - [EMPRESA] - [CAI]`

### 8.9 Múltiples CAI

FlowControl Print soporta **múltiples CAI simultáneos**. Cada autorización tiene:
- Su propio rango (Desde/Hasta)
- Su propia fecha límite
- Puede activarse o desactivarse con doble clic
- Controles de correlativos y alertas automáticas

---

## 9. Gestión de Transacciones

### 9.1 Carga de Transacciones

Una vez conectada la sesión con QuickBooks y seleccionado un CAI, el sistema carga automáticamente las transacciones:

1. **Invoices** (Facturas)
2. **SalesReceipts** (Recibos de Venta)

### 9.2 Tabla de Transacciones

La tabla muestra las siguientes columnas:

| Columna | Descripción |
|---------|-------------|
| **Type** | Tipo de transacción (Invoice o SalesReceipt) |
| **Ref #** | Número de referencia de la transacción |
| **Date** | Fecha de la transacción |
| **Customer** | Nombre del cliente |
| **Amount** | Monto total de la transacción |
| **Memo** | Memo o descripción adicional |
| **Exonerado** | Checkbox para marcar facturas exoneradas |
| **Imprimir** | Botón para generar la vista previa e impresión |

### 9.3 Navegación por Páginas

El sistema carga transacciones en lotes de **60 registros** por página:

| Botón | Función |
|-------|---------|
| **Anterior** | Navega a la página anterior de transacciones cargadas |
| **Siguiente** | Carga la siguiente página de transacciones desde QuickBooks |

> **Nota:** Las páginas ya cargadas se almacenan en memoria (`TransactionsHistory`), por lo que navegar hacia atrás es instantáneo.

### 9.4 Búsqueda por Número de Referencia

Para buscar una transacción específica:

1. Ingrese el número de referencia en el campo de búsqueda.
2. Haga clic en **Buscar**.
3. El sistema filtrará las transacciones que coincidan con el número ingresado.
4. Para volver a ver todas las transacciones, haga clic en **Limpiar**.

### 9.5 Checkbox de Exonerado

Cada transacción tiene un checkbox en la columna **Exonerado**:

- **Marcado:** La factura se considera exonerada y requerirá los datos de exoneración al imprimir.
- **Desmarcado:** La factura se imprimirá como normal.

Al marcar/desmarcar, el sistema intercambia los valores entre las columnas ocultas `Exonerado1` y `Exonerado2` para preservar los datos de exoneración previamente ingresados.

### 9.6 Información de la Transacción Seleccionada

Al hacer clic en una fila, el panel de información muestra:

![IMAGEN 8 - Listado de Facturas](https://i.postimg.cc/RFH9q15M/image.png)

---

## 10. Impresión de Facturas

### 10.1 Proceso de Impresión

1. En la tabla de transacciones, localice la factura que desea imprimir.
2. Si es una factura exonerada, marque el checkbox en la columna **Exonerado**.
3. Haga clic en el botón **Imprimir** de la fila correspondiente.
4. Si la factura es exonerada, se abrirá el formulario de datos de exoneración.
5. Se abrirá la **Vista Previa** de la factura.
6. Desde la vista previa, puede:
   - Revisar el formato de la factura
   - Navegar entre páginas (si hay múltiples)
   - Imprimir directamente
   - Cerrar sin imprimir

### 10.2 Formato de la Factura

La factura impresa cumple con todos los requisitos del SAR de Honduras e incluye:

#### 10.2.1 Encabezado

- **Logo de la empresa** (si existe)
- **Nombre de la empresa** emisora
- **RTN** del emisor
- **Dirección** fiscal
- **Teléfono** y **Correo** electrónico
- **Número de factura** (con prefijo del CAI)
- **Fecha de factura** y **Fecha de vencimiento**
- **Dirección del cliente**

#### 10.2.2 Información de Autorización

- **C.A.I:** Código de Autorización de Impresión
- **RANGO AUTORIZADO:** Desde - Hasta
- **Fecha límite de Emisión**

#### 10.2.3 Datos del Cliente

- **Nombre del cliente**
- **RTN del cliente** (obtenido automáticamente de QuickBooks)

#### 10.2.4 Tabla de Ítems

| Columna | Descripción |
|---------|-------------|
| **CANT** | Cantidad |
| **ITEM** | Descripción del producto/servicio |
| **PRECIO UNITARIO** | Precio unitario |
| **DESCT Y REBAJAS** | Descuentos aplicados |
| **ISV %** | Tasa de impuesto (15%, 18%, E, X, -) |
| **SUB-TOTAL** | Subtotal de la línea |
| **PRECIO FINAL** | Precio final de la línea |

#### 10.2.5 Valor en Letras

Campo que muestra el monto total de la factura escrito en letras, con centavos en formato fraccionario:

#### 10.2.6 Información Adicional

- **FACTURA ES BENEFICIO DE TODOS EXIJALA**
- **No. Correlativo de orden de compra exenta**
- **No. Correlativo de constancia de registro exonerado**
- **No. Identificativo del registro de la SAG**
- **Orden de Compra (cliente)**

#### 10.2.7 Totales

| Concepto | Descripción |
|----------|-------------|
| **DESC. Y REBAJAS OTORGADAS** | Total de descuentos |
| **IMPORTE EXONERADO** | Monto exonerado de impuestos |
| **IMPORTE EXENTO** | Monto exento de impuestos |
| **IMPORTE GRAVADO 15%** | Monto gravado al 15% |
| **IMPORTE GRAVADO 18%** | Monto gravado al 18% |
| **I.S.V 15%** | Impuesto sobre ventas al 15% |
| **I.S.V 18%** | Impuesto sobre ventas al 18% |
| **TOTAL A PAGAR** | Total final de la factura |

#### 10.2.8 Pie de Página

Tres copias identificadas:
- **ORIGINAL: CLIENTE**
- **COPIA: OBLIGADO TRIBUTARIO EMISOR**
- **COPIA: CONTABILIDAD**

### 10.3 Paginación Automática

El sistema cuenta con un sistema de **paginación inteligente**:

- Si la factura tiene muchos ítems, se distribuyen automáticamente en varias páginas.
- Se mantienen encabezados, totales y pie de página correctamente en cada página.
- Las páginas intermedias se ajustan según la cantidad de ítems.
- La última página muestra los totales completos.

### 10.4 Vista Previa

La vista previa se muestra en una ventana maximizada con:
- Navegación entre páginas
- Zoom
- Opciones de impresión
- Botón de cierre

---

## 11. Manejo de Facturas Exoneradas

### 11.1 ¿Qué es una Factura Exonerada?

Una factura exonerada es aquella emitida a un cliente que posee una **constancia de exoneración** vigente otorgada por el SAR. Estas facturas no causan Impuesto Sobre Ventas (ISV).

### 11.2 Formulario de Exonerado

Al hacer clic en **Imprimir** en una factura marcada como exonerada, se abre el siguiente formulario:

![IMAGEN 9 - Formulario Exoneración](https://i.postimg.cc/PqtJ9RDv/image.png)

### 11.3 Campos del Formulario

| Campo | Descripción |
|-------|-------------|
| **No. Correlativo de orden de compra exenta** | Número de la orden de compra exenta del cliente |
| **No. Correlativo de constancia de registro exonerado** | Número de la constancia de registro exonerado |
| **No. Identificativo del registro de la SAG** | Número identificativo del registro SAG (Servicio de Administración de Aduanas) |

### 11.4 Comportamiento al Imprimir una Factura Exonerada

Cuando se imprime una factura exonerada:

1. **Todo el importe** se mueve a la casilla **IMPORTE EXONERADO**.
2. Las casillas de **IMPORTE EXENTO**, **IMPORTE GRAVADO 15%**, **IMPORTE GRAVADO 18%**, **I.S.V 15%** e **I.S.V 18%** se limpian para evitar duplicidad.
3. Los **descuentos** se establecen en cero (opcional, configurable).
4. Los tres correlativos de exoneración se reflejan en la sección de **Información Adicional** de la factura.

### 11.5 Persistencia de Datos de Exoneración

Los datos de exoneración ingresados se almacenan de forma persistente en la memoria.

Esto permite que los datos se conserven aunque se desmarque y vuelva a marcar el checkbox de exonerado.

---

## 12. Sistema de Logs

### 12.1 Acceso al Visor de Logs

Desde el menú superior: **Logs** → Se abre el formulario de Logs.

### 12.2 Ubicación de los Archivos de Log

Los logs se almacenan en:

```txt
Logs[timestamp].log
```

Donde `timestamp` es un número Unix correspondiente al día.

### 12.3 Formato de los Logs

Cada entrada de log tiene el siguiente formato:

```txt
[dd-MM-yyyy HH:mm:ss] Mensaje del log
```

**Ejemplo:**

```txt
[03-11-2026 14:32:15] Conectando a QuickBooks…
[03-11-2026 14:32:18] QuickBooks esta listo!
[03-11-2026 14:32:20] <?xml version="1.0" encoding="utf-8"?>...
[03-11-2026 14:32:22] [Taxes] Dictionary no inicializado al procesar tax code 'XYZ'. Se trata como exento.
```

### 12.4 Tipos de Eventos Registrados

| Evento | Descripción |
|--------|-------------|
| Consultas QBXML | Se registran todas las consultas XML enviadas a QuickBooks |
| Respuestas QBXML | Se registran las respuestas recibidas de QuickBooks |
| Errores de conexión | Fallos al conectar con QuickBooks |
| Errores de licencia | Fallos en la validación de licencia |
| Errores de CAI | Problemas al acceder a archivos de CAI |
| Líneas descartadas | Líneas de factura ignoradas por estar vacías o ser subtotales |
| Tax codes huérfanos | Códigos de impuesto no encontrados en el diccionario |

---

## 13. Cumplimiento SAR Honduras

### 13.1 Requisitos del SAR Cumplidos

FlowControl Print cumple con todos los requisitos exigidos por el **Servicio de Administración de Rentas (SAR)** de Honduras para la emisión legal de facturas:

| Requisito SAR | Implementación en FlowControl |
|---------------|-------------------------------|
| CAI válido | ✅ Gestión completa de CAI con validación de formato |
| Rango autorizado | ✅ Control de correlativos Desde/Hasta |
| RTN emisor y cliente | ✅ RTN del emisor en empresa, RTN del cliente desde QuickBooks |
| Valor en letras | ✅ Conversión automática de montos a letras |
| Importes exonerados | ✅ Campo específico para facturas exoneradas |
| Importes exentos | ✅ Campo específico para importes exentos |
| Importes gravados 15% y 18% | ✅ Desglose automático por tasa de impuesto |
| ISV desglosado | ✅ ISV 15% e ISV 18% separados |
| Correlativo de orden de compra exenta | ✅ Campo en formulario de exonerados |
| Constancia de registro exonerado | ✅ Campo en formulario de exonerados |
| Identificativo SAG | ✅ Campo en formulario de exonerados |
| Multi-copia | ✅ Original (cliente), Obligado tributario emisor, Contabilidad |
| Formato exacto | ✅ Sin errores de redondeo ni datos faltantes |

### 13.2 Códigos de Impuesto Soportados

El sistema reconoce los siguientes códigos de impuesto de QuickBooks:

| Código en QuickBooks | Interpretación | Tasa |
|----------------------|----------------|------|
| `IVA15` o `G15` | Gravado al 15% | 15% |
| `IVA18` o `G18` | Gravado al 18% | 18% |
| `EXENTO` o `E` | Exento | 0% |
| `EXONERADO` o `X` | Exonerado | 0% |
| Cualquier otro | No gravado | 0% |

### 13.3 Validación de Estructura del CAI

El sistema valida la estructura del CAI, y la estructura del rango:

```txt
000-000-00-00000000
```

---

## 14. Preguntas Frecuentes

### 14.1 ¿Cómo funciona FlowControl Print?

FlowControl Print está diseñado para ser intuitivo y eficiente, operando en **3 simples pasos**:

1. **Conecta QuickBooks:** Abre tu archivo de compañía (`.QBW`) en QuickBooks Desktop y presiona el botón **"Conectar"** en el panel izquierdo. El aplicativo detectará la sesión activa y sincronizará automáticamente tus clientes, productos, impuestos y transacciones.
2. **Selecciona un CAI:** Registra tu Código de Autorización de Impresión (CAI) con su rango autorizado (Desde/Hasta) y fecha límite. Selecciona la autorización activa desde el panel lateral con un **doble clic**. El sistema valida automáticamente la estructura y detecta duplicados.
3. **Factura e imprime:** Elige la transacción (Factura o Recibo de Venta) desde la lista, marca la casilla de **"Exonerado"** si aplica (para ingresar los correlativos de exención), genera la vista previa y envía a imprimir. El formato generado cumple al 100% con los requisitos fiscales del SAR de Honduras.

### 14.2 ¿Qué versiones de QuickBooks son compatibles?

FlowControl Print utiliza la integración oficial **QBFC16** (QuickBooks Foundation Classes), compatible con todas las versiones de **QuickBooks Desktop**: ediciones **Pro**, **Premier** y **Enterprise**. Ofrece la máxima estabilidad.

### 14.3 ¿Cómo funciona la licencia?

Cada instalación requiere un **número de licencia único** que se valida en línea contra nuestros servidores. Una vez activada, la licencia queda registrada bajo su control **de por vida** y no requiere conexión permanente a internet.

### 14.4 ¿Puedo usar múltiples CAI al mismo tiempo?

**Sí.** FlowControl Print soporta múltiples CAI simultáneos. Cada autorización tiene su propio rango (Desde/Hasta), fecha límite y puede activarse o desactivarse con doble clic. El sistema cuenta con controles de correlativos y alertas automáticas.

### 14.5 ¿Las facturas cumplen con el SAR de Honduras?

**Absolutamente.** El formato incluye CAI, rango autorizado, fecha límite de emisión, valor en letras, RTN del cliente, descuentos, importes exonerados, exentos, gravados al 15% y 18%, y las tres copias requeridas (cliente, obligado tributario emisor, contabilidad). También maneja correlativos de orden de compra exenta, constancia de registro exonerado e identificativo SAG.

### 14.6 ¿Qué pasa si tengo facturas con muchos ítems?

FlowControl Print cuenta con un sistema de **paginación inteligente**. Si la factura tiene muchos ítems, se distribuyen automáticamente en varias páginas, manteniendo encabezados, totales y pie de página correctamente. Las páginas intermedias se ajustan según la cantidad de ítems hasta el final, y la última página muestra los totales completos.

### 14.7 ¿Puedo gestionar datos de varias empresas?

**Sí.** La aplicación permite configurar múltiples empresas con sus propios datos (RTN, dirección, teléfono, correo), cada una conectada a su archivo .QBW de QuickBooks.

### 14.8 ¿Cómo obtengo el RTN del cliente automáticamente?

El RTN del cliente se obtiene automáticamente desde los **campos personalizados (Custom Fields)** del cliente en QuickBooks. Debe configurar un campo personalizado llamado **"RTN"** en el perfil de cada cliente en QuickBooks.

### 14.9 ¿Qué hago si QuickBooks no se conecta?

1. Verifique que QuickBooks Desktop esté **abierto y con sesión iniciada**.
2. Asegúrese de que el archivo de compañía (.QBW) sea accesible.
3. Verifique que tenga permisos de administrador en Windows.
4. Reinicie tanto QuickBooks como FlowControl Print.
5. Si el problema persiste, consulte los logs

### 14.10 ¿Dónde se almacenan los datos?

Todos los datos se almacenan localmente

Los datos y la información son **100% suyos**. No se envía información a servidores externos excepto para la validación inicial de la licencia.

### 14.11 ¿Puedo usar FlowControl Print sin Internet?

**Sí.** Después de la activación inicial de la licencia (que requiere Internet), el aplicativo funciona completamente **sin conexión a Internet**.

---

## 15. Soporte Técnico

### 15.1 Contacto

Para soporte técnico, consultas o reportar errores, contacte al administrador del sistema o al desarrollador a través de los canales oficiales.

### 15.2 Información para Reportar Errores

Al reportar un error, incluya la siguiente información:

1. **Versión del aplicativo:** (Ver en barra de título o About)
2. **Versión de QuickBooks:** (Ayuda → Acerca de QuickBooks)
3. **Versión de Windows:** (Configuración → Sistema → Acerca de)
4. **Archivo de log:** Adjunte el archivo `.log` correspondiente a la fecha del error
5. **Descripción detallada:** Pasos para reproducir el error
6. **Capturas de pantalla:** Si es posible

### 15.3 Archivos de Log

Los archivos de log son la principal herramienta de diagnóstico. Ubique el archivo correspondiente a la fecha del problema en:

```txt
Logs[timestamp].log
```

---

## Apéndice A: Glosario de Términos

| Término | Definición |
|---------|------------|
| **CAI** | Código de Autorización de Impresión. Código otorgado por el SAR para emitir facturas. |
| **SAR** | Servicio de Administración de Rentas de Honduras. |
| **RTN** | Registro Tributario Nacional. Identificador fiscal de 15 dígitos en Honduras. |
| **ISV** | Impuesto Sobre Ventas. Impuesto al consumo en Honduras (15% o 18%). |
| **QBW** | Extensión de archivo de compañía de QuickBooks Desktop. |
| **QBFC** | QuickBooks Foundation Classes. Librería de integración oficial de QuickBooks. |
| **QBXML** | Lenguaje XML utilizado para comunicarse con QuickBooks. |
| **Invoice** | Factura. Documento que registra una venta a crédito. |
| **SalesReceipt** | Recibo de Venta. Documento que registra una venta de contado. |
| **SAG** | Servicio de Administración de Aduanas (Honduras). |
| **Exonerado** | Cliente o transacción exempta del pago de ISV por autorización del SAR. |

---

## Apéndice B: Atajos y Comportamientos

| Acción | Método |
|--------|--------|
| Seleccionar CAI activo | Doble clic en la lista de CAI |
| Buscar transacción | Ingresar Ref# y clic en Buscar |
| Limpiar búsqueda | Clic en Limpiar |
| Navegar páginas | Botones Anterior / Siguiente |
| Ver detalles | Clic en una fila de la tabla |
| Imprimir factura | Clic en botón "Imprimir" de la fila |
| Marcar exonerada | Checkbox en columna Exonerado |
| Cerrar aplicación | Menú Opciones o botón X |

---

## Apéndice C: Notas de Versión

### Versión 1.0.0.0 (2026)

**Características implementadas:**
- Integración completa con QuickBooks Desktop vía QBFC16
- Gestión de CAI con múltiples autorizaciones
- Impresión de facturas con formato SAR Honduras
- Manejo de facturas exoneradas
- RTN automático de clientes desde campos personalizados
- Paginación inteligente para facturas con muchos ítems
- Sistema de licencia basado en GitHub
- Multi-empresa
- Sistema de logs
- Temas Claro/Oscuro (en desarrollo)

---

**© 2026 FlowControl Print. Todos los derechos reservados.**

---

*Fin del Manual de Usuario*
