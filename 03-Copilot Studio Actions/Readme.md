# MS-4022 – Módulo 3 : Introducción a las acciones para agentes declarativos en Copilot Studio

## Introducción

En este módulo se presenta el concepto de **acciones en Copilot Studio**, una funcionalidad que permite extender y ampliar las capacidades de los agentes declarativos de Microsoft 365 Copilot mediante una experiencia **low-code**.

Las acciones permiten que un agente no solo responda preguntas utilizando información existente, sino también que pueda ejecutar tareas, interactuar con sistemas externos y automatizar procesos empresariales.

---

# Escenario del módulo

Se plantea el caso de un equipo encargado de desarrollar productos dentro de una organización.

El equipo recibe consultas internas de áreas como:

* Ventas
* Marketing
* Soporte interno

Para mejorar los tiempos de respuesta y brindar una mejor experiencia, la organización creó un:

## Agente de soporte técnico de productos

Este agente fue desarrollado para Microsoft 365 Copilot y permite responder preguntas relacionadas con productos.

Posteriormente surge una nueva necesidad:

> Explorar cómo ampliar las funcionalidades del agente mediante acciones.

---

# ¿Qué son las acciones?

Las acciones son capacidades que permiten que un agente pueda:

* Ejecutar procesos
* Interactuar con servicios externos
* Automatizar tareas
* Obtener información dinámica
* Conectarse con APIs y flujos
* Extender el comportamiento del agente más allá de respuestas conversacionales

En otras palabras:

> Las acciones convierten a un agente en algo más que un chatbot.

---

# Acciones y agentes

Las acciones hacen que los agentes sean más capaces porque les permiten:

* Recuperar información
* Ejecutar tareas
* Interactuar con sistemas externos
* Proporcionar funcionalidades avanzadas

---

# ¿Qué es una acción en Copilot Studio?

Una acción es:

> Un fragmento de código reutilizable que realiza una tarea específica o proporciona una característica específica para un agente.

Los agentes utilizan acciones cuando necesitan:

* Entregar resultados
* Ejecutar procesos
* Obtener información
* Responder solicitudes del usuario

Las acciones funcionan en segundo plano gestionando tareas específicas automáticamente.

---

# Reutilización de acciones

En Copilot Studio:

* Una acción puede crearse una sola vez
* Luego reutilizarse en múltiples agentes

Esto facilita:

* La reutilización de lógica
* La estandarización
* El mantenimiento
* La escalabilidad

---

# Registro de acciones

Copilot Studio incluye un:

## Registro de acciones

Este componente se encarga de:

* Almacenar acciones
* Administrar metadatos
* Gestionar información de ejecución
* Centralizar las acciones disponibles

---

# Biblioteca de Copilot Studio

Las acciones pueden administrarse desde la:

## Biblioteca de Copilot Studio

Desde allí es posible:

* Examinar acciones existentes
* Ver agentes disponibles
* Crear nuevas acciones
* Administrar componentes reutilizables

---

# Escenarios de uso de acciones

Es recomendable agregar acciones cuando el agente necesita:

* Interactuar con sistemas externos
* Ejecutar tareas específicas
* Automatizar procesos
* Proporcionar funcionalidades avanzadas

---

# Ejemplos de acciones

## Gestión de incidentes

* Recuperar una lista de incidentes relacionados con un proyecto

## Administración de pedidos

* Buscar pedidos de clientes en sistemas de gestión

## Información externa

* Consultar el clima para un viaje de negocios

## Integración con DevOps

* Crear errores o bugs automáticamente a partir de correos electrónicos

## Automatización con IA

* Generar resúmenes de proyectos siguiendo lineamientos del equipo

---

# Tipos de acciones en Copilot Studio

Copilot Studio permite crear distintos tipos de acciones para ampliar agentes declarativos.

Cada tipo de acción responde a diferentes escenarios empresariales.

---

# Acciones de solicitud (Prompt Actions)

Las acciones de solicitud permiten al agente ejecutar:

* prompts predefinidos
* instrucciones específicas
* generación personalizada de contenido

Estas acciones son ideales cuando se necesita:

> Personalizar respuestas generadas por IA según la entrada del usuario.

---

# Funcionamiento de las acciones de solicitud

El agente ejecuta prompts previamente definidos utilizando:

* la entrada del usuario
* instrucciones del agente
* conocimiento disponible

Esto permite generar respuestas dinámicas y contextualizadas.

---

# Ejemplo de acción de solicitud

Ejemplo de prompt:

> “Generar un resumen de estado del proyecto en función de la fecha de finalización objetivo, siguientes acciones, bloqueadores y ayuda necesaria.”

Con este enfoque, el agente puede:

* Crear reportes automáticos
* Generar resúmenes
* Producir contenido estructurado
* Adaptar respuestas al contexto empresarial

---

# AI Builder y acciones de solicitud

Las acciones de solicitud utilizan:

## AI Builder

y la funcionalidad de:

## Prompts personalizados

Esto permite proporcionar instrucciones específicas al modelo de IA.

---

# Escenarios comunes para acciones de solicitud

## Resumen de contenido

* Resumir reuniones
* Resumir proyectos
* Resumir documentos

## Extracción de información

* Extraer entidades
* Detectar sentimientos
* Obtener elementos de acción

## Traducción

* Traducir texto automáticamente

## Generación de contenido

* Crear reportes
* Redactar respuestas
* Generar documentos empresariales

---

# Integración con Dataverse

Las acciones de solicitud pueden utilizar:

## Dataverse

para ampliar el conocimiento disponible del agente.

Esto permite:

* Obtener información empresarial específica
* Personalizar respuestas según datos internos
* Crear experiencias más contextualizadas

---

# Acciones del conector (Connector Actions)

Las acciones del conector permiten al agente:

* Recuperar datos externos
* Actualizar información
* Ejecutar operaciones mediante APIs
* Integrarse con sistemas empresariales

---

# Objetivo de las acciones del conector

Los conectores permiten construir agentes:

* Más dinámicos
* Más útiles
* Más conectados con procesos reales
* Adaptados a necesidades empresariales específicas

---

# Sistemas compatibles mediante conectores

Copilot Studio permite conectarse con plataformas populares como:

* Salesforce
* Zendesk
* MailChimp
* GitHub
* SharePoint
* OneDrive

y muchos otros sistemas empresariales.

---

# Tipos de conectores

## Conectores certificados de Microsoft

Son conectores oficiales ya disponibles en la plataforma.

## Conectores personalizados

Pueden ser creados por la organización para escenarios específicos.

---

# Conectores personalizados

Cuando no existe un conector para un sistema específico:

> Es posible crear un conector personalizado.

Esto permite integrar:

* APIs internas
* Sistemas legacy
* Servicios propios de la organización

---

# Acciones dentro de un conector

Cada conector incluye:

## Acciones específicas

que pueden habilitarse dentro del agente.

Por ejemplo:

* Consultar datos
* Crear registros
* Actualizar información
* Ejecutar procesos

---

# Consideraciones sobre el desarrollo de acciones

Antes de crear acciones en Copilot Studio es importante comprender:

* Requisitos previos
* Entornos
* Soluciones
* Orígenes de conocimiento
* Variables de entrada y salida
* Métodos de autenticación

---

# Requisitos previos

Para ampliar agentes con acciones en Copilot Studio se necesita:

## Cuenta profesional o educativa

Debe tener acceso a:

* Copilot Studio
* Power Platform

En algunos casos se puede utilizar una:

* cuenta de prueba

---

## Licencia de Microsoft 365 Copilot

Es necesaria para trabajar con agentes y acciones.

---

## Credenciales de acceso

Se requieren credenciales válidas para conectarse a:

* APIs
* conectores
* servicios externos
* sistemas empresariales

---

# Estado de versión preliminar pública

En el momento de publicación del módulo:

> Las acciones de Copilot Studio se encuentran en versión preliminar pública.

Esto implica que:

* No están recomendadas para producción
* Pueden tener funcionalidades limitadas
* Microsoft busca obtener feedback temprano

---

# Entornos en Power Platform

Antes de crear acciones se puede:

* Crear un entorno nuevo
* Seleccionar un entorno existente

---

# ¿Qué es un entorno?

Un entorno en Power Platform es un espacio utilizado para:

* Almacenar datos
* Administrar aplicaciones
* Compartir procesos empresariales
* Separar recursos organizacionales

---

# Objetivos de los entornos

Los entornos ayudan a separar aplicaciones según:

* Roles
* Seguridad
* Audiencias
* Procesos empresariales

---

# Dataverse y entornos

Cada entorno puede tener:

## Una base de datos Microsoft Dataverse

Dataverse actúa como almacenamiento empresarial centralizado.

---

# Administración de entornos

La administración de entornos se realiza desde:

## Centro de administración de Power Platform

[Power Platform Admin Center](https://admin.powerplatform.microsoft.com/?utm_source=chatgpt.com)

---

# Roles administrativos necesarios

Para administrar entornos se requieren roles como:

* Administrador de entorno
* Administrador del sistema

---

# Soluciones en Power Platform

Al crear una acción se debe seleccionar una:

## Solución

---

# ¿Qué son las soluciones?

Las soluciones permiten:

* Agrupar componentes
* Transportar aplicaciones entre entornos
* Aplicar personalizaciones

---

# Ventajas de usar soluciones

## Organización

Mantienen componentes agrupados y ordenados.

## Portabilidad

Permiten mover acciones entre entornos fácilmente.

## Administración

Facilitan mantenimiento y despliegue.

---

# Recomendación importante

> Se recomienda utilizar soluciones personalizadas para administrar acciones y componentes.

---

# Orígenes de conocimiento

Los orígenes de conocimiento proporcionan la información que utilizan:

* agentes
* acciones
* prompts

---

# Tipos de orígenes de conocimiento

## Dataverse

* Tablas empresariales

## Archivos cargados

* PDFs
* documentos
* archivos internos

## SharePoint y OneDrive

* Bibliotecas corporativas
* archivos compartidos

## Sitios web públicos

* Información accesible públicamente

## Datos empresariales mediante conectores

* Sistemas externos
* APIs
* plataformas corporativas

---

# APIs como conocimiento

Las APIs también pueden actuar como:

## Orígenes dinámicos de información

permitiendo obtener:

* datos actualizados
* información en tiempo real
* contenido empresarial

---

# Variables de entrada y salida

Las acciones pueden requerir:

* Entradas
* Salidas

---

# Variables de entrada

Las variables de entrada definen:

> La información necesaria para ejecutar una acción.

Ejemplo:

* Una API meteorológica puede requerir:

  * ciudad
  * país
  * unidades de temperatura

---

# Variables de salida

Las variables de salida representan:

> Los resultados generados por la acción.

Estas salidas pueden:

* mostrarse al usuario
* reutilizarse en otras acciones
* alimentar procesos posteriores

---

# Restricciones en parámetros

Algunas acciones poseen:

## Parámetros obligatorios

En ciertos casos:

* no se pueden eliminar
* no se pueden agregar variables nuevas

Sin embargo:

* sí pueden modificarse las descripciones

para mejorar la comprensión.

---

# Autenticación

Muchos conectores y orígenes de datos requieren:

## Autenticación

para acceder a información segura.

---

# Tipos de autenticación

## No autenticado

Ejemplo:

* MSN Weather

Accede a información pública y no requiere credenciales.

---

## Autenticación mediante conectores

Los conectores poseen:

* métodos de autenticación integrados

Por defecto:

> Los usuarios deben iniciar sesión con sus propias credenciales.

---

# Consideración importante sobre permisos

Cuando un conector está disponible:

* Todas sus acciones quedan disponibles para los usuarios autorizados

No existe:

> Seguridad basada en roles por acción individual dentro del mismo conector.

---

# Autenticación en acciones de solicitud

Las acciones de solicitud utilizan:

* identidad de Teams
* identidad de Power Apps

---

# Compartición de prompts

Después de crear prompts personalizados:

> Deben compartirse con los usuarios o grupos adecuados.

---

# Extensión de agentes declarativos con acciones

Una vez creado un agente declarativo en Copilot Studio:

> Es posible ampliar sus capacidades agregando acciones.

Esto transforma al agente en una solución más interactiva y automatizada.

---

# Flujo para extender un agente con acciones

## Paso 1 – Ir a la biblioteca de Copilot Studio

Desde la biblioteca se administran:

* acciones
* agentes
* conectores
* componentes reutilizables

---

## Paso 2 – Crear una nueva acción

La acción puede ser:

* una acción de solicitud
* una acción de conector
* una integración personalizada

---

## Paso 3 – Agregar la acción al agente

Desde la página de información general del agente se puede:

> Asociar la acción al agente declarativo.

---

## Paso 4 – Publicar el agente

Una vez configurado:

> El agente puede publicarse en Microsoft 365 Copilot.

---

# Asistente de configuración

Durante la creación de acciones:

> Copilot Studio proporciona un asistente guiado.

Este asistente ayuda a:

* Configurar parámetros
* Definir conexiones
* Elegir tipos de acciones
* Establecer entradas y salidas
* Configurar autenticación

---

# Objetivo de extender agentes

La extensión mediante acciones permite que los agentes:

* Ejecuten tareas reales
* Interactúen con sistemas empresariales
* Consulten APIs
* Automaticen procesos
* Generen contenido dinámico
* Respondan con información actualizada

---

# Flujo típico de funcionamiento de una acción

## Paso 1 – El usuario realiza una solicitud

Ejemplo:

> “Mostrame los incidentes abiertos del proyecto.”

## Paso 2 – El agente interpreta la intención

El agente determina:

* Qué necesita el usuario
* Qué acción debe ejecutarse
* Qué sistemas deben consultarse

## Paso 3 – Se ejecuta la acción

La acción puede:

* Consultar APIs
* Ejecutar prompts
* Recuperar información
* Actualizar sistemas

## Paso 4 – El agente devuelve la respuesta

El usuario recibe:

* Datos
* Resúmenes
* Confirmaciones
* Resultados procesados

---

# Beneficios empresariales de las acciones

## Automatización de procesos

Reducen trabajo manual y repetitivo.

## Integración corporativa

Permiten conectar Microsoft 365 Copilot con plataformas empresariales.

## Experiencias más inteligentes

Los agentes pueden ejecutar tareas reales y no solo responder preguntas.

## Centralización

Las acciones pueden administrarse desde un único lugar.

## Escalabilidad

La reutilización permite extender múltiples agentes rápidamente.

---

# Casos de uso reales

## Soporte IT

* Crear tickets automáticamente
* Consultar incidentes
* Actualizar estados

## Gestión de proyectos

* Generar reportes
* Obtener estado de tareas
* Detectar bloqueadores

## Recursos Humanos

* Consultar políticas internas
* Automatizar respuestas frecuentes
* Integrarse con sistemas de RRHH

## Ventas

* Consultar CRM
* Buscar oportunidades
* Obtener información de clientes

## Marketing

* Generar resúmenes de campañas
* Extraer insights
* Automatizar contenido

---

# Comparación rápida de tipos de acciones

| Tipo de acción        | Objetivo principal                       | Ejemplos                                                  |
| --------------------- | ---------------------------------------- | --------------------------------------------------------- |
| Acciones de solicitud | Generación de contenido mediante IA      | Resúmenes, traducciones, extracción de sentimientos       |
| Acciones del conector | Integración con APIs y sistemas externos | Consultar Salesforce, crear tickets, acceder a SharePoint |

---

# ¿Cómo elegir el tipo correcto de acción?

Al diseñar acciones es importante preguntarse:

## ¿Qué necesita hacer el usuario?

* Obtener información
* Actualizar datos
* Automatizar procesos
* Generar contenido

## ¿Qué sistemas externos intervienen?

* APIs
* Bases de datos
* Plataformas empresariales
* Servicios externos

## ¿Qué tipo de comportamiento se necesita?

* Recuperar datos
* Modificar datos
* Ejecutar múltiples tareas
* Generar respuestas personalizadas

---

# Resumen del módulo

En este módulo aprendimos que:

* Las acciones amplían las capacidades de los agentes declarativos
* Los agentes pueden interactuar con sistemas externos
* Las acciones son reutilizables
* Existen distintos tipos de acciones en Copilot Studio
* Las acciones permiten automatizar procesos empresariales
* Los conectores permiten integraciones con APIs y plataformas externas
* Los prompts personalizados permiten generar contenido inteligente con IA
* Los entornos y soluciones facilitan la administración y despliegue
* Las variables de entrada y salida permiten intercambiar información entre acciones
* Los agentes pueden publicarse en Microsoft 365 Copilot

---

# Conceptos clave

## Copilot Studio

Herramienta de Microsoft para crear y extender agentes de IA y experiencias conversacionales.

Permite:

* Crear agentes declarativos
* Agregar conocimiento
* Configurar instrucciones
* Incorporar acciones
* Diseñar automatizaciones mediante low-code

---

## Agentes declarativos

Son agentes configurados principalmente mediante:

* instrucciones
* conocimiento
* comportamientos declarativos

Sin necesidad de desarrollar toda la lógica manualmente.

---

## Low-Code

Las acciones se crean utilizando una experiencia visual y simplificada.

Esto permite que:

* desarrolladores
* analistas
* usuarios avanzados

puedan extender agentes sin necesidad de programación compleja.

---

# ¿Por qué son importantes las acciones?

Las acciones permiten pasar de un agente que:

## Solo responde preguntas

a un agente que también puede:

* Crear tickets
* Consultar sistemas externos
* Obtener datos actualizados
* Ejecutar procesos
* Automatizar tareas empresariales
* Integrarse con herramientas corporativas

---

# Beneficios de las acciones

## Reutilización

Una acción puede utilizarse en múltiples agentes.

## Escalabilidad

Permiten ampliar funcionalidades sin rehacer lógica.

## Automatización

Reducen tareas manuales y mejoran procesos.

## Integración

Conectan agentes con servicios y plataformas externas.

## Experiencias más inteligentes

Los agentes dejan de ser simples asistentes conversacionales y pasan a ejecutar tareas reales.

---

# Resultado esperado del módulo

Al finalizar este módulo, el estudiante podrá:

* Comprender qué son las acciones en Copilot Studio
* Entender cómo funcionan
* Reconocer escenarios donde utilizarlas
* Diferenciar tipos de acciones
* Comprender requisitos técnicos y de autenticación
* Entender el uso de entornos y soluciones
* Saber cómo extender agentes declarativos
* Publicar agentes en Microsoft 365 Copilot
* Elegir el tipo de acción adecuado
* Prepararse para crear acciones en Copilot Studio

---

# Idea central del módulo

> Las acciones son el mecanismo principal para ampliar las capacidades de los agentes declarativos en Microsoft 365 Copilot y permitir que interactúen activamente con procesos y sistemas empresariales.

---

# Frases clave del módulo

> “Las acciones permiten que los agentes interactúen con sistemas externos.”

> “Una acción es un fragmento de código reutilizable.”

> “Las acciones transforman agentes conversacionales en asistentes capaces de ejecutar tareas reales.”

> “Los conectores permiten integrar Microsoft 365 Copilot con APIs y plataformas empresariales.”

> “Las acciones de solicitud permiten personalizar respuestas generadas por IA.”

> “Los entornos y soluciones facilitan la administración y despliegue de acciones.”

> “Las variables de entrada y salida permiten intercambiar información entre acciones y usuarios.”

> “Los agentes declarativos pueden ampliarse agregando acciones reutilizables.”

---

# Recursos adicionales

## Extensión de Microsoft 365 Copilot con agentes

[Microsoft Learn – Extensión de Microsoft 365 Copilot con agentes](https://learn.microsoft.com/es-es/microsoft-365-copilot/extensibility/?utm_source=chatgpt.com)

---

## Arquitectura de acciones en Copilot Studio

[Microsoft Learn – Arquitectura de acciones de Copilot Studio](https://learn.microsoft.com/es-es/microsoft-copilot-studio/authoring-actions-overview?utm_source=chatgpt.com)

---


## Recurso oficial del módulo

[Microsoft Learn – Introducción a las acciones para agentes declarativos en Copilot Studio](https://learn.microsoft.com/es-es/training/modules/introduction-actions-declarative-agents-copilot-studio/?utm_source=chatgpt.com)
