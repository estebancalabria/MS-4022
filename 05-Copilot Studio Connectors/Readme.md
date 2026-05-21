# MS-4022 - Extensión de Agentes Declarativos con Acciones de Conector en Copilot Studio

## 📘 Introducción

Los conectores representan una de las capacidades más potentes de Microsoft Copilot Studio, ya que permiten ampliar el conocimiento y las funcionalidades de los agentes mediante la integración con aplicaciones y servicios externos.

Copilot Studio incluye más de **1200 conectores predefinidos** compatibles con servicios populares tanto dentro como fuera del ecosistema Microsoft. Además, es posible crear **conectores personalizados** para integrarse con sistemas internos u orígenes de datos propios de la organización.

Gracias a estos conectores, los agentes pueden:

* Consultar información externa.
* Ejecutar acciones en otros sistemas.
* Automatizar procesos empresariales.
* Acceder a documentos y datos en tiempo real.
* Integrarse con plataformas corporativas existentes.

---

# 🚀 Caso de Uso Empresarial

Se plantea el escenario de un equipo encargado de desarrollar productos dentro de una organización.

Distintas áreas como:

* Ventas
* Marketing
* Servicio al cliente

realizan consultas frecuentes relacionadas con:

* Especificaciones de productos
* Preguntas frecuentes
* Políticas de garantía
* Reparaciones y devoluciones
* Funcionalidades futuras

Toda esta información se encuentra almacenada en una biblioteca de documentos de **SharePoint Online**.

La solución propuesta consiste en crear un **agente de Copilot** capaz de:

* Mejorar los tiempos de respuesta.
* Centralizar el acceso a la información.
* Brindar una experiencia más eficiente a los empleados.
* Leer información desde archivos Excel mediante acciones de conector.
* Obtener detalles sobre funcionalidades futuras de productos.

---

# 🔌 ¿Qué son las Acciones de Conector?

Las acciones del conector permiten que un agente interactúe con servicios externos y orígenes de datos mediante conectores configurados dentro de Copilot Studio.

Estas acciones son especialmente útiles cuando se necesita:

* Consultar datos empresariales.
* Recuperar información en tiempo real.
* Ejecutar operaciones externas.
* Integrar sistemas corporativos.
* Automatizar procesos de negocio.

Las acciones de conector funcionan como un puente entre el agente y distintos servicios externos.

---

# 📌 Escenarios de Uso de Acciones del Conector

Las acciones del conector son ideales para acceder a información almacenada en sistemas empresariales.

## Ejemplos

* Obtener información de inventario desde SAP.
* Consultar datos de ventas desde sistemas CRM.
* Integrarse con Dynamics 365.
* Consultar información desde Salesforce.
* Acceder a datos almacenados fuera de Microsoft 365.

Gracias a estas acciones, los agentes pueden conectarse a múltiples plataformas y utilizar información empresarial en tiempo real.

---

# 🌐 Tipos de Conectores

Copilot Studio permite trabajar con distintos tipos de conectores.

## 🟢 Conectores Standard

Son conectores incluidos en todos los planes de Copilot Studio.

### Ejemplos

* SharePoint
* Office 365
* Microsoft Teams

Estos conectores permiten integraciones rápidas y sencillas con servicios Microsoft comunes.

---

## 🟡 Conectores Premium

Disponibles únicamente en determinados planes de Copilot Studio.

Permiten integraciones más avanzadas con aplicaciones empresariales y servicios especializados.

### Ejemplos

* Salesforce
* Dynamics 365
* SAP
* Servicios empresariales avanzados

---

## 🔧 Conectores Personalizados

Permiten conectarse a cualquier API pública o servicio que no esté cubierto por conectores existentes.

Características principales:

* Se crean manualmente.
* Permiten extender completamente las capacidades del agente.
* Pueden integrarse con sistemas internos.
* Deben publicarse como conectores certificados para utilizarse con Microsoft 365 Copilot.

Esto permite integrar prácticamente cualquier sistema corporativo.

---

# 🛠️ Creación de Acciones del Conector

Copilot Studio permite crear acciones de conector desde la biblioteca del entorno.

## Flujo General

### 1️⃣ Crear una Nueva Acción

Desde la biblioteca de Copilot Studio:

* Seleccionar **Nuevo**.
* Elegir **Conector**.
* Configurar la nueva acción.

También es posible agregar acciones directamente desde la página de información general del agente mediante:

* **Agregar acción**
* **Nueva acción**
* **Conector personalizado**

---

# 🔎 Selección de un Conector

Al crear una acción, Copilot Studio muestra:

* Todos los conectores certificados de Microsoft.
* Conectores personalizados del entorno actual.
* Barra de búsqueda para localizar conectores rápidamente.

Esto facilita encontrar el servicio correcto para integrar.

---

# 🏷️ Definición de la Acción del Conector

Cada acción requiere:

* Nombre
* Descripción
* Solución

---

## 📛 Nombre de la Acción

El nombre:

* Debe ser único.
* Debe describir claramente la funcionalidad.
* Ayuda a los usuarios a identificar fácilmente la acción.

### Ejemplo recomendado

✅ “Servicio de correo: permite recuperar y crear mensajes”

---

## 📝 Descripción de la Acción

La descripción es extremadamente importante porque:

* Ayuda al LLM a comprender cuándo usar la acción.
* Mejora el reconocimiento en lenguaje natural.
* Proporciona contexto funcional.

### Buenas prácticas

* Ser específico.
* Ser detallado.
* Incluir palabras clave funcionales.
* Describir exactamente qué hace la acción.

### Ejemplo

✅ “El servicio de correo proporciona la capacidad de obtener listas de mensajes existentes, recuperar carpetas, enumerar títulos, actualizar mensajes y establecer prioridades.”

Una descripción detallada es mucho mejor que algo genérico como:

❌ “Sales app connector”

---

# 📦 Soluciones en Copilot Studio

Las acciones se almacenan dentro de soluciones.

Beneficios:

* Facilitan mover componentes entre entornos.
* Mejoran la administración.
* Permiten empaquetar configuraciones.
* Ayudan en despliegues empresariales.

Si no se selecciona una solución:

* Copilot Studio crea una automáticamente.

---

# ⚙️ Selección de Acciones del Conector

Cada conector expone múltiples acciones disponibles.

Por ejemplo:

* Obtener datos
* Crear registros
* Actualizar información
* Enumerar elementos

El creador debe seleccionar cuáles estarán habilitadas.

## Importante

* No existe límite en la cantidad de acciones seleccionadas.
* Solo estarán disponibles las acciones configuradas explícitamente.
* No se pueden agregar acciones inexistentes desde el asistente.

---

# 👥 Consideraciones Según el Rol del Usuario

Al seleccionar acciones, es importante pensar:

* ¿Quién usará el agente?
* ¿Qué información tendrá disponible?
* ¿Qué tipo de solicitudes realizará?

Solo deben habilitarse acciones para las cuales:

* Los usuarios puedan proporcionar datos válidos.
* El escenario tenga sentido funcional.

---

# 🧠 Configuración de Cada Acción

Cada acción seleccionada debe configurarse individualmente.

Se debe definir:

* Nombre
* Descripción funcional

La descripción ayuda al LLM a identificar cuándo utilizar la acción correcta.

---

## ✨ Ejemplo de Descripción Inteligente

Para una acción llamada:

“Enumerar carpetas de mensajes”

Se recomienda una descripción como:

✅ “Permite obtener una lista de todas las carpetas disponibles en el servicio de correo y devolverlas en formato de lista.”

Esto agrega contexto semántico como:

* obtener
* recuperar
* listar
* carpetas
* mensajes
* servicio de correo

El LLM usa estas pistas para decidir cuándo ejecutar la acción.

---

# 📥 Configuración de Entradas y Salidas

Cada acción tiene:

* Parámetros de entrada
* Parámetros de salida

Estos parámetros:

* Son definidos por el conector.
* No pueden modificarse estructuralmente.
* Sí pueden documentarse mejor mediante descripciones.

---

# 🤖 Optimización para LLM

Las descripciones de acciones y parámetros son fundamentales para mejorar el comportamiento del modelo.

## Buenas prácticas

* Explicar formatos esperados.
* Incluir ejemplos.
* Detallar tipos de datos.
* Especificar formatos de fecha.

### Ejemplo

✅ “Esta acción devuelve clientes potenciales de Dynamics 365 Sales según un rango de fechas en formato MM/DD/AAAA.”

Esto ayuda al copiloto a:

* Interpretar correctamente la intención.
* Mapear entradas del usuario.
* Generar llamadas válidas a la API.

---

# 🔐 Configuración de Conexiones

Antes de usar la acción:

* Debe existir una conexión al sistema externo.

Es posible:

* Seleccionar una conexión existente.
* Crear una nueva conexión.

La creación de conexiones puede requerir:

* Usuario
* Contraseña
* Credenciales
* Autenticación empresarial

---

# ⚠️ Funcionalidades y Limitaciones de la Vista Previa

En el momento del módulo:

* Las acciones de Copilot Studio se encuentran en **Versión preliminar pública**.

Esto implica:

* Funcionalidades limitadas.
* Posibles cambios futuros.
* Restricciones de producción.
* Características aún en evolución.

Microsoft recomienda revisar:

* Funcionalidades soportadas.
* Limitaciones actuales.
* Características no admitidas.

---

# 🧪 Laboratorio Práctico

## 🎯 Objetivo del Ejercicio

En este ejercicio se configura una herramienta de conector para un agente declarativo en Copilot Studio.

Se utilizará el conector:

* **“SharePoint - List folder”**

para recuperar una lista de archivos desde una carpeta llamada:

* **Products**

que contiene archivos de soporte de productos.

---

## 📘 Traducción del Enunciado

> En este ejercicio, configurará una herramienta de conector para un agente declarativo en Copilot Studio. Utilizará el conector “SharePoint - List folder” para recuperar una lista de archivos desde una carpeta Products que contiene archivos de soporte de productos.

---

## 🔗 Laboratorio Oficial

[https://microsoftlearning.github.io/MS-4022-Extend-Microsoft-365-Copilot-in-Copilot-Studio/Instructions/Labs/03-Connector-actions/01-create-connector-action.html](https://microsoftlearning.github.io/MS-4022-Extend-Microsoft-365-Copilot-in-Copilot-Studio/Instructions/Labs/03-Connector-actions/01-create-connector-action.html)

---

# 🧠 Capacidades de los Conectores

Con los conectores en Copilot Studio se pueden realizar tareas como:

* Leer información desde Excel.
* Consultar listas y bibliotecas de SharePoint.
* Integrarse con Dynamics 365.
* Conectarse a Microsoft Teams.
* Consumir APIs externas.
* Automatizar flujos empresariales.
* Integrar sistemas internos mediante conectores personalizados.
* Acceder a datos empresariales en tiempo real.

---

# 🎯 Beneficios para los Agentes

El uso de conectores permite crear agentes más:

* Inteligentes
* Dinámicos
* Contextuales
* Automatizados
* Integrados con procesos empresariales reales

Esto transforma al agente en una herramienta capaz de interactuar activamente con el ecosistema digital de la empresa.

---

# 📚 Más Información

* Uso de conectores de Power Platform en Copilot Studio
* Creación de una acción de inteligencia artificial del conector
* Revisión de la documentación de conectores

---

# 🎯 Objetivos del Módulo

En este módulo se aprendió a:

* Describir los conectores en Power Platform.
* Crear y configurar acciones de conector para agentes declarativos.
* Integrar agentes con aplicaciones y servicios externos.
* Utilizar datos empresariales dentro de los agentes.
* Configurar accesos a información dinámica.
* Extender las capacidades de agentes declarativos.
* Trabajar con conectores estándar, premium y personalizados.
* Configurar parámetros de entrada y salida.
* Optimizar acciones para Large Language Models (LLM).

---

# 🏁 Conclusión Final

Los conectores son una pieza fundamental para construir agentes empresariales avanzados en Copilot Studio.

Gracias a ellos, los agentes pueden:

* Acceder a información en tiempo real.
* Integrarse con sistemas corporativos.
* Automatizar tareas complejas.
* Consultar datos empresariales externos.
* Ejecutar acciones sobre múltiples plataformas.

Las descripciones detalladas, configuraciones correctas y parámetros bien definidos permiten que el LLM seleccione acciones de manera mucho más precisa y natural.

El uso de conectores transforma a los agentes declarativos en asistentes empresariales capaces de interactuar activamente con aplicaciones corporativas, APIs y sistemas externos, ampliando enormemente las posibilidades de automatización e integración dentro de Microsoft 365 Copilot y Copilot Studio.

