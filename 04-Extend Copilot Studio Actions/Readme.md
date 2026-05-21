# MS-4022 – Módulo 4

# Extensión de Agentes Declarativos con Acciones de Solicitud en Copilot Studio

## 📘 Introducción

Las **acciones de solicitud (Prompt Actions)** permiten definir prompts dentro de Copilot Studio para que los agentes generen respuestas personalizadas frente a solicitudes de los usuarios.

Estas acciones permiten extender el comportamiento de los agentes declarativos de Microsoft 365 Copilot, agregando lógica conversacional específica para distintos escenarios empresariales.

---

# 🎯 Objetivo del módulo

En este módulo se aprende a:

* Diseñar acciones de solicitud
* Crear prompts personalizados
* Probar acciones dentro de Copilot Studio
* Publicar acciones para agentes declarativos
* Extender las capacidades de Microsoft 365 Copilot
* Aplicar técnicas de Prompt Engineering
* Configurar entradas y salidas dinámicas
* Utilizar el Prompt Builder de Copilot Studio

---

# 🧠 ¿Qué son las Prompt Actions?

Las Prompt Actions son plantillas de prompts reutilizables que se agregan como acciones dentro de agentes declarativos.

Permiten transformar un modelo GPT en una herramienta especializada para tareas empresariales específicas mediante instrucciones cuidadosamente diseñadas.

Una Prompt Action puede incluir:

* Instrucciones del prompt
* Entradas
* Salidas
* Datos de ejemplo
* Descripción de la acción

---

# 💡 ¿Qué son las indicaciones personalizadas?

Las indicaciones personalizadas permiten indicarle al modelo GPT:

* Cómo debe comportarse
* Qué tarea debe realizar
* Qué formato debe devolver
* Qué reglas debe respetar

Esto convierte al modelo en una herramienta flexible y adaptable a distintos escenarios de negocio.

---

# 💼 Caso de uso del módulo

Se presenta un escenario donde un equipo desarrolla productos para una organización y recibe consultas internas de:

* Ventas
* Marketing
* Servicio al cliente

Para mejorar la experiencia y acelerar tiempos de respuesta, el equipo crea un agente declarativo de soporte técnico de productos usando Microsoft 365 Copilot.

Luego, se agrega una Prompt Action capaz de:

✅ Generar resúmenes de marketing para productos
✅ Ayudar a equipos de ventas y marketing
✅ Automatizar respuestas internas

---

# 📝 Ejemplo de Prompt Action

Ejemplo de acción reutilizable:

> "Analice las notas de reunión proporcionadas y genere un informe de reunión de Contoso. Describa y resuma lo siguiente: objetivo, decisiones clave, elementos de acción y fechas límite. El resumen debe ser conciso, profesional y fácil de compartir con los miembros del equipo."

Este ejemplo muestra cómo un prompt bien diseñado puede automatizar tareas empresariales frecuentes.

---

# 🚀 Escenarios de uso de Prompt Actions

## 🏷️ Clasificación de información

Permite analizar grandes volúmenes de texto y asignar etiquetas predefinidas.

Ejemplo:

* Clasificar tickets
* Categorizar consultas
* Identificar tipos de incidentes

---

## 🔍 Extracción de entidades

Permite extraer información específica desde texto no estructurado.

Ejemplos:

* Nombre del cliente
* Persona de contacto
* Número telefónico
* Datos relevantes

---

## ✍️ Borrador de respuestas

Permite generar respuestas sugeridas para atención al cliente o soporte.

Ejemplo:

* Respuestas automáticas
* Sugerencias de solución
* Asistencia contextual

---

## 📄 Resumen de contenido

Permite resumir información y extraer tareas o acciones importantes.

Ejemplos:

* Resumen de reuniones
* Elementos de acción
* Decisiones tomadas

---

# 🧪 Prompt Engineering

El módulo enfatiza la importancia de aplicar técnicas de ingeniería de prompts para mejorar la calidad de las respuestas generadas por GPT.

La calidad del resultado depende directamente de cómo se redacta el prompt.

---

# ✅ Buenas prácticas para escribir prompts efectivos

## 🎯 Sea específico

Las instrucciones deben ser claras y concretas.

❌ Evitar:

* Lenguaje ambiguo
* Instrucciones vagas

✅ Preferir:

* Objetivos claros
* Formato definido
* Resultado esperado explícito

---

## 📚 Use ejemplos

Los ejemplos ayudan al modelo a entender:

* El formato esperado
* El estilo deseado
* El tipo de respuesta correcta

---

## ✨ Manténgalo simple

Evitar:

* Lógica excesivamente compleja
* Instrucciones demasiado largas
* Sobrecarga de contexto innecesario

Las instrucciones simples suelen producir mejores resultados.

---

## 🚧 Defina una salida alternativa

Es recomendable indicar qué debe hacer el modelo si no encuentra información.

Ejemplo:

> "Responder con 'no encontrado' si la respuesta no está presente."

Esto ayuda a reducir alucinaciones y respuestas incorrectas.

---

# 🔄 Iteración y refinamiento

El módulo destaca la importancia de:

* Probar prompts
* Refinarlos
* Ajustarlos según los resultados

Si la respuesta:

* Es demasiado larga
* Contiene información irrelevante
* No es precisa

… entonces el prompt debe modificarse y optimizarse.

---

# 🛠️ Creación de una Prompt Action en Copilot Studio

Copilot Studio incluye un **Prompt Builder** que permite crear prompts personalizados con contenido dinámico que se completa en runtime.

Además, el builder permite:

* Probar prompts
* Validar precisión
* Refinar resultados
* Configurar entradas y salidas
* Guardar acciones reutilizables

---

# ⚠️ Estado Preview

## 📌 Importante

Al momento de publicación del módulo:

* Las acciones de Copilot Studio están en **Public Preview**
* No están pensadas para producción
* Pueden tener limitaciones funcionales
* Microsoft las publica anticipadamente para obtener feedback de clientes

---

# 🛠️ Pasos para crear una nueva Prompt Action

## 1️⃣ Iniciar sesión en Copilot Studio

Ingresar al entorno de Copilot Studio.

---

## 2️⃣ Ir a la biblioteca

Desde la biblioteca se administran las acciones disponibles.

---

## 3️⃣ Seleccionar “Agregar nuevo”

Se presentan varias opciones de creación.

---

## 4️⃣ Seleccionar “Preguntar”

Esto abre el **AI Builder Prompt Builder**.

También es posible crear una acción desde:

* La pantalla de detalles de un agente declarativo
* La opción “Agregar acción”

---

# ⚙️ Configuración del Prompt

El asistente guía el proceso de configuración.

---

## 🏷️ Nombre y descripción

Se debe definir:

* Nombre de la acción
* Descripción clara y precisa

La descripción debe indicar:

* Qué hace la acción
* Cuándo es útil
* Qué tipo de resultado genera

---

# ✍️ Uso del Prompt Builder

Dentro del Prompt Builder se puede:

## ✅ Escribir o pegar instrucciones

El prompt principal se define en la sección de instrucciones.

---

## 🤖 Generar prompts con IA

Copilot Studio puede ayudar a redactar prompts usando IA generativa.

También existen botones rápidos para:

* Resumir texto
* Extraer información
* Generar prompts automáticamente

---

## 📚 Explorar biblioteca de prompts

Se pueden reutilizar prompts de ejemplo disponibles en la biblioteca.

---

## ➕ Agregar entradas dinámicas

La opción **Agregar contenido** permite incorporar variables de entrada.

Estas entradas:

* Funcionan como placeholders
* Se completan en tiempo de ejecución
* Permiten prompts dinámicos

Las variables pueden insertarse usando `/` dentro de las instrucciones.

---

## 🧪 Probar el prompt

El Prompt Builder permite ejecutar pruebas usando datos de ejemplo.

---

## 📊 Revisar respuestas del modelo

Durante las pruebas se analiza:

* Precisión
* Relevancia
* Calidad de la salida

Luego se ajusta el prompt según los resultados.

---

## 💾 Guardar el prompt

Una vez validado, el prompt personalizado se guarda como acción reutilizable.

---

# 🔌 Entradas y salidas

Después de guardar el prompt se configuran:

## 📥 Variables de entrada

Funcionan como datos dinámicos que se completan en runtime.

Cada variable debe tener:

* Nombre
* Descripción

---

## 📤 Variables de salida

Definen el contenido generado por la acción.

También requieren:

* Nombre
* Descripción

---

# 🧱 Acceso y edición de Prompt Actions

Una vez guardada, la acción:

✅ Aparece en la biblioteca
✅ Puede agregarse a agentes declarativos
✅ Puede editarse posteriormente
✅ Está disponible desde “Agregar acción”

---

# 🧪 Laboratorio del módulo

## 🎯 Objetivo del ejercicio

En este laboratorio se crea una Prompt Action, se prueba el prompt dentro de Copilot Studio y posteriormente se prueba la acción dentro de un agente de Copilot.

El ejercicio consiste en desarrollar una Prompt Action que ayude a los usuarios a transformar ideas iniciales o desordenadas en propuestas de marketing organizadas siguiendo un formato y lineamientos específicos.

---

## 🛠️ Actividades realizadas

Durante el laboratorio se trabaja con:

* Creación de Prompt Actions
* Uso del Prompt Builder
* Configuración de entradas y salidas
* Pruebas de prompts
* Refinamiento de respuestas
* Integración de la acción dentro de un agente declarativo

---

## 🔗 Laboratorio oficial

[Laboratorio - Crear una Prompt Action](https://microsoftlearning.github.io/MS-4022-Extend-Microsoft-365-Copilot-in-Copilot-Studio/Instructions/Labs/02-Prompt-actions/01-create-prompt-action.html?utm_source=chatgpt.com)

---

# 🛠️ Recursos y ejemplos

Microsoft proporciona prompts de ejemplo para comenzar rápidamente.

## 🔗 Recurso oficial

[https://aka.ms/power-prompts](https://aka.ms/power-prompts?utm_source=chatgpt.com)

También se puede usar IA generativa dentro de Copilot Studio para diseñar prompts usando lenguaje natural.

---

# 🎁 Beneficios de las Prompt Actions

## ✅ Personalización

Permiten adaptar las respuestas del agente a necesidades específicas del negocio.

## ✅ Reutilización

Los prompts pueden reutilizarse en múltiples escenarios.

## ✅ Productividad

Reducen el tiempo necesario para responder consultas repetitivas.

## ✅ Mejor experiencia de usuario

Las respuestas son más relevantes, consistentes y contextualizadas.

## ✅ Flexibilidad dinámica

Permiten incorporar entradas dinámicas y respuestas adaptadas al contexto.

---

# 🛠️ Conceptos clave

| Concepto             | Descripción                                    |
| -------------------- | ---------------------------------------------- |
| Prompt Action        | Acción reutilizable basada en prompts          |
| Prompt Engineering   | Técnicas para diseñar prompts efectivos        |
| Prompt Builder       | Herramienta visual para crear prompts          |
| Variables de entrada | Datos dinámicos usados en runtime              |
| Variables de salida  | Respuesta generada por la acción               |
| Agente declarativo   | Agente que amplía Microsoft 365 Copilot        |
| GPT                  | Modelo generativo utilizado por Copilot        |
| Contexto empresarial | Información usada para personalizar respuestas |

---

# 📚 Resumen del módulo

En este módulo se aprendió sobre:

* Acciones de solicitud de AI Builder
* Uso de prompts personalizados para:

  * Clasificar información
  * Extraer entidades
  * Redactar respuestas
  * Resumir contenido
* Buenas prácticas de Prompt Engineering
* Importancia de crear prompts:

  * Claros
  * Concisos
  * Específicos
  * Contextuales
  * Relevantes
* Uso del Prompt Builder en Copilot Studio
* Creación de Prompt Actions reutilizables
* Configuración de entradas y salidas dinámicas
* Importancia de probar y refinar prompts
* Integración de Prompt Actions dentro de agentes declarativos

---

# 🔗 Recursos adicionales

* Información general de prompts
* Creación de prompts
* Galería de soluciones de ejemplo
* Distribución de prompts mediante soluciones

---

# 📌 Idea central del módulo

Las Prompt Actions permiten transformar agentes declarativos en asistentes especializados capaces de automatizar tareas empresariales mediante instrucciones inteligentes, reutilizables y optimizadas usando Prompt Engineering y entradas dinámicas configuradas en Copilot Studio.
