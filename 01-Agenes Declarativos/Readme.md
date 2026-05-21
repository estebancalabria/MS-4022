# MS-4022 – Introducción a los Agentes Declarativos para Microsoft 365 Copilot

# 📘 Introducción

## ¿Qué es Microsoft 365 Copilot?

Microsoft 365 Copilot es una herramienta de productividad impulsada por Inteligencia Artificial que utiliza:

* **LLM (Large Language Models)**
* **Microsoft Graph**
* **Aplicaciones y servicios de Microsoft 365**

Copilot puede interpretar información empresarial y generar respuestas utilizando los datos disponibles dentro del ecosistema Microsoft 365.

---

# ❓ Problema que resuelven los agentes declarativos

Aunque Microsoft 365 Copilot puede responder preguntas usando información de la organización, este enfoque generalista no siempre es ideal.

## Problemas comunes

* Copilot puede acceder a demasiada información.
* Las respuestas pueden no enfocarse en un dominio específico.
* Puede faltar control sobre:

  * los datos utilizados,
  * el formato de respuesta,
  * las acciones que puede ejecutar.

## Necesidades típicas

* Limitar el contexto a ciertos documentos.
* Especializar Copilot en una tarea concreta.
* Definir reglas específicas de comportamiento.
* Integrar sistemas externos.

---

# 🤖 ¿Qué es un agente?

Un agente es una Inteligencia Artificial conversacional que interactúa con usuarios mediante una interfaz de chat.

Los agentes pueden:

* responder preguntas,
* proporcionar información,
* ejecutar tareas,
* automatizar procesos.

## Casos de uso frecuentes

* Soporte técnico IT
* Atención al cliente
* Recursos Humanos
* Asistentes empresariales
* Automatización interna

---

# 🧠 ¿Qué es un agente declarativo?

Los **agentes declarativos** permiten extender Microsoft 365 Copilot para escenarios específicos.

Permiten:

* definir conocimientos personalizados,
* crear acciones personalizadas,
* controlar el comportamiento del agente,
* especializar las respuestas,
* integrar sistemas externos.

> Un agente declarativo convierte Microsoft 365 Copilot en un asistente especializado para un dominio concreto.

---

# 🔒 Infraestructura compartida con Microsoft 365 Copilot

Los agentes declarativos reutilizan:

* el mismo orquestador,
* los mismos modelos base,
* la misma infraestructura,
* los mismos controles de seguridad,

de Microsoft 365 Copilot.

## Beneficios

* Experiencia consistente
* Seguridad integrada
* Integración nativa
* Menor complejidad
* Menor esfuerzo de implementación

---

# 🧩 Componentes principales

## 1. Conocimientos personalizados (Custom Knowledge)

Permiten definir:

* qué información utilizará el agente,
* sobre qué datos razonará,
* cómo responderá.

---

## 2. Acciones personalizadas (Custom Actions)

Permiten:

* interactuar con sistemas externos,
* ejecutar acciones mediante APIs,
* consultar datos en tiempo real,
* modificar información externa.

---

# ⚙️ Funcionamiento de los agentes declarativos

Los agentes declarativos combinan:

* instrucciones personalizadas,
* grounding,
* acciones personalizadas,
* razonamiento del orquestador,
* modelos LLM,

para generar respuestas contextualizadas y especializadas.

---

# 📚 Conocimientos personalizados

Los conocimientos personalizados agregan:

* contexto,
* reglas,
* comportamiento,
* información empresarial,

adaptados a un escenario específico.

---

# 📝 Instrucciones personalizadas

Las instrucciones son reglas enviadas al modelo para controlar cómo responde el agente.

## Permiten definir

### 📌 Tareas

* responder preguntas,
* resumir información,
* generar contenido,
* administrar tickets.

---

### 🎭 Comportamiento

* tono,
* estilo,
* nivel de detalle,
* lenguaje técnico o no técnico.

---

### 🚫 Restricciones

* contenido prohibido,
* limitaciones legales,
* restricciones de copyright,
* información sensible.

---

### 📄 Formato

* listas,
* viñetas,
* estructura de respuesta,
* longitud de salida.

---

# 🌍 Grounding (Puesta a tierra)

El grounding conecta el LLM con información empresarial real.

Esto mejora:

* precisión,
* relevancia,
* contexto,
* confiabilidad.

---

# 📂 Fuentes de grounding soportadas

Los agentes declarativos pueden usar:

* OneDrive,
* SharePoint Online,
* Copilot Connectors,
* Bing Search.

---

# 📌 Importante

Por defecto:

> Un agente declarativo NO tiene acceso automático a fuentes de datos.

Las fuentes deben configurarse explícitamente.

---

# 🔗 Citas automáticas

Cuando Copilot utiliza grounding:

* muestra referencias,
* cita documentos,
* indica el origen de la información.

Esto mejora:

* transparencia,
* trazabilidad,
* confianza en las respuestas.

---

# ⚡ Acciones personalizadas

Las acciones personalizadas permiten que el agente interactúe con sistemas externos mediante APIs.

## Ejemplos

* Crear tickets
* Actualizar incidencias
* Consultar sistemas empresariales
* Ejecutar procesos
* Leer información externa

---

# 🛠 Escenario de ejemplo – Soporte Técnico IT

## Contexto

El equipo de soporte:

* almacena artículos técnicos en SharePoint Online,
* utiliza PDFs de knowledge base,
* administra tickets en un sistema externo.

---

# 🎯 Objetivo

Crear un asistente de autoservicio que:

* responda preguntas frecuentes,
* use únicamente documentación corporativa,
* reduzca tickets,
* responda con lenguaje simple,
* evite jerga técnica,
* permita crear o actualizar incidencias.

---

# 🧱 Configuración del agente del escenario

## 📌 Instrucciones personalizadas

Definen:

* comportamiento,
* tono,
* claridad para usuarios no técnicos.

---

## 📚 Grounding

Usa:

* documentos de SharePoint,
* artículos técnicos,
* PDFs corporativos.

---

## ⚡ Acción personalizada

Permite:

* conectarse al sistema de tickets,
* consultar incidencias,
* crear o actualizar tickets mediante lenguaje natural.

---

# 🔄 Flujo completo de funcionamiento

## 1. Entrada

El usuario envía un prompt.

Ejemplo:

```txt id="promptvpn"
@No puedo conectarme al VPN
```

---

## 2. Comprobaciones preliminares

Copilot ejecuta:

* controles de seguridad,
* validaciones de IA responsable,
* mitigaciones de riesgo.

---

## 3. Razonamiento

El orquestador analiza:

* intención,
* contexto,
* plan de respuesta.

---

## 4. Recuperación de grounding

Copilot busca información relevante en:

* SharePoint,
* OneDrive,
* conectores,
* Bing.

---

## 5. Ejecución de acciones

El agente puede:

* llamar APIs,
* consultar sistemas externos,
* recuperar datos,
* modificar información.

---

## 6. Recuperación de instrucciones

Se cargan:

* reglas,
* tono,
* restricciones,
* formato.

---

## 7. Generación de respuesta

El orquestador combina:

* prompt,
* grounding,
* instrucciones,
* acciones,

y envía toda la información al LLM para generar la respuesta.

---

## 8. Salida

Copilot:

* responde al usuario,
* actualiza la conversación,
* muestra citas y referencias.

---

# 🧭 Cuándo usar agentes declarativos

Los agentes declarativos son ideales cuando:

* existe un escenario específico,
* se desea reutilizar Microsoft 365 Copilot,
* los datos están en Microsoft 365,
* no se necesita un LLM personalizado,
* se busca reducir complejidad de implementación.

---

# 📋 Criterios de decisión

Microsoft propone evaluar tres factores principales.

---

# 🎯 1. Escenario

## Pregunta clave

> ¿Existe un problema o tarea específica que se desea optimizar?

Los agentes declarativos funcionan mejor cuando:

* el caso de uso es claro,
* el dominio está definido,
* el objetivo es específico.

---

## Escenarios ideales

* Soporte IT
* RRHH
* Atención al cliente
* Consultas documentales
* Automatización empresarial

---

# 🧠 2. Orquestador y modelo

Los agentes declarativos reutilizan:

* el modelo base,
* el orquestador,
* la infraestructura,

de Microsoft 365 Copilot.

---

# ✅ Ventajas

* experiencia consistente,
* menor complejidad,
* integración nativa,
* seguridad integrada.

---

# 🚫 Cuándo NO conviene

No son ideales si se necesita:

* otro LLM,
* orquestación personalizada,
* pipelines IA complejos,
* razonamiento altamente especializado.

En esos casos:

> Conviene evaluar agentes personalizados o motores IA propios.

---

# 📂 3. Orígenes de datos

Funcionan mejor cuando:

* la información está en Microsoft 365,
* los documentos están en SharePoint,
* los archivos están en OneDrive.

---

# 🔌 Integraciones externas

## Copilot Connectors

Permiten incorporar:

* datos externos,
* contenido histórico,
* sistemas empresariales.

---

## Acciones personalizadas

Permiten:

* interacción en tiempo real,
* ejecución de procesos,
* modificación de sistemas externos.

---

# 🛠 Aplicación práctica al escenario IT

Microsoft aplica los criterios al caso del soporte técnico.

---

# 🎯 Escenario

Sí existe un escenario claro:

* soporte técnico autoservicio para empleados.

---

# 🧠 Modelo y orquestador

No se necesita otro modelo.

Microsoft 365 Copilot puede:

* resumir información,
* responder preguntas,
* transformar documentos.

---

# 📂 Datos

Los datos están disponibles en:

* SharePoint Online,
* PDFs corporativos.

---

# ⚡ Sistemas externos

El sistema de tickets está fuera de Microsoft 365.

Solución:

* acciones personalizadas mediante APIs.

---

# ✅ Conclusión del análisis

El escenario es ideal para un agente declarativo porque:

* existe un caso de uso claro,
* Microsoft 365 Copilot cubre las capacidades necesarias,
* los datos ya están en Microsoft 365,
* las integraciones externas pueden resolverse con acciones.

---

# 🧭 Resumen visual convertido a texto

## Paso 1 – Definir el escenario

La primera pregunta es:

> ¿Existe un escenario específico que se desea optimizar?

### Si la respuesta es NO

Conviene usar directamente:

* Microsoft 365 Copilot BizChat.

### Si la respuesta es SÍ

Se continúa evaluando el resto de criterios.

---

# 🧠 Paso 2 – Evaluar el modelo y orquestador

La siguiente pregunta es:

> ¿Se necesita un LLM o un orquestador personalizado?

### Si la respuesta es SÍ

Los agentes declarativos probablemente no sean la mejor opción.

Se debería considerar:

* agentes personalizados,
* motores IA propios,
* orquestación avanzada.

### Si la respuesta es NO

Se puede continuar evaluando agentes declarativos.

---

# 📂 Paso 3 – Evaluar los datos

La siguiente pregunta es:

> ¿Los datos de grounding están en Microsoft 365?

### Si la respuesta es SÍ

El escenario encaja muy bien con agentes declarativos.

### Si la respuesta es NO

Se debe evaluar si:

* un Copilot Connector puede resolver el problema,
* o si es posible crear un conector personalizado.

---

# 🔌 Paso 4 – Evaluar conectores

Pregunta:

> ¿Un Copilot Connector es suficiente?

### Si la respuesta es SÍ

Se puede continuar utilizando agentes declarativos.

### Si la respuesta es NO

Debe evaluarse:

* crear un conector personalizado,
* o buscar otra arquitectura.

---

# ⚡ Paso 5 – Evaluar interacción con sistemas externos

Pregunta:

> ¿Es necesario interactuar en tiempo real con sistemas externos?

### Si la respuesta es NO

Los agentes declarativos son una muy buena opción.

### Si la respuesta es SÍ

Debe evaluarse:

* crear acciones personalizadas,
* integrar APIs externas.

---

# 🛠 Paso 6 – Evaluar acciones personalizadas

Pregunta:

> ¿Es posible crear acciones personalizadas?

### Si la respuesta es SÍ

El escenario sigue siendo ideal para agentes declarativos.

### Si la respuesta es NO

Puede ser necesario:

* investigar otras soluciones,
* utilizar arquitecturas más personalizadas.

---

# 🚫 Cuándo NO conviene usar agentes declarativos

No son ideales cuando:

* se necesitan modelos IA diferentes,
* se requiere control total del pipeline,
* se necesita orquestación avanzada,
* los datos no pueden integrarse fácilmente,
* no se desea implementar conectores ni acciones.

---

# 🧱 Formas de crear agentes declarativos

## Low-Code

Herramientas disponibles:

* Microsoft Copilot Studio
* SharePoint Online
* Centro de administración de Microsoft

---

## Pro-Code

También pueden desarrollarse con:

* Visual Studio Code

---

# 👥 Cómo usan los usuarios los agentes

## 1. En contexto

Dentro de BizChat usando `@`.

Ejemplo:

```txt id="bizctx"
@ITSupport ¿Cómo configuro el VPN?
```

---

## 2. Experiencia inmersiva

Conversación dedicada 1 a 1 con el agente.

Incluye:

* starters personalizados,
* experiencia tipo chatbot.

---

# 🧾 Resumen final del módulo

El objetivo del módulo fue ayudar a determinar cuándo un agente declarativo es la mejor opción para extender Microsoft 365 Copilot.

Microsoft propone analizar tres criterios:

* 🎯 Escenario
* 🧠 Orquestador y modelo
* 📂 Orígenes de datos

---

# 📌 ¿Qué permite este análisis?

Permite:

* evaluar viabilidad,
* estimar esfuerzo,
* comprender limitaciones,
* determinar si Microsoft 365 Copilot cubre las necesidades del escenario.

---

# 🛠 Resultado del escenario IT

El escenario de soporte técnico era ideal porque:

* el caso de uso estaba claramente definido,
* los datos estaban en SharePoint,
* el modelo de Copilot era suficiente,
* las integraciones externas podían resolverse con acciones personalizadas.

---

# ⚡ Trabajo adicional requerido

La integración con el sistema de tickets requería:

* crear acciones personalizadas,
* integrar APIs externas.

---

# 💡 Idea clave del módulo

## Microsoft 365 Copilot proporciona la base.

## Los agentes declarativos permiten especializarla.

Esto permite construir asistentes empresariales capaces de:

* usar conocimiento corporativo,
* responder con contexto,
* aplicar reglas específicas,
* interactuar con sistemas externos,
* automatizar procesos reales.

---

# 🎯 Conclusión

Los agentes declarativos son ideales cuando:

* existe un escenario concreto,
* Microsoft 365 Copilot cubre las capacidades necesarias,
* los datos están en Microsoft 365,
* las integraciones externas pueden resolverse mediante conectores o acciones.

En esos casos:

> Los agentes declarativos permiten construir asistentes empresariales especializados de forma rápida, segura y reutilizando toda la infraestructura de Microsoft 365 Copilot.
