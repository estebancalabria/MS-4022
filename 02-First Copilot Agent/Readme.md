# MS-4022 - Módulo 2

# Crear el primer agente declarativo para Microsoft 365 Copilot mediante Copilot Studio

## 📘 Introducción

Los **agentes declarativos** (*Declarative Agents* o *Copilot Agents*) permiten extender las capacidades de Microsoft 365 Copilot utilizando instrucciones personalizadas, grounding y conocimiento empresarial.

En este módulo se aprende a crear un agente especializado utilizando Microsoft Copilot Studio para responder preguntas basadas en documentos y datos corporativos almacenados en Microsoft 365.

---

# 🎯 Objetivos del módulo

Al finalizar el módulo podrás:

* Crear un agente declarativo
* Configurar instrucciones personalizadas
* Incorporar conocimiento empresarial
* Agregar grounding personalizado
* Definir mensajes sugeridos
* Publicar el agente
* Validar respuestas en Microsoft 365 Copilot

---

# 🧠 ¿Qué es un agente declarativo?

Un agente declarativo es una extensión especializada de Microsoft 365 Copilot que:

* Responde consultas en lenguaje natural
* Usa conocimiento organizacional
* Sigue instrucciones específicas
* Tiene comportamiento personalizado
* Puede conectarse a distintas fuentes de datos

Estos agentes permiten crear asistentes especializados para áreas concretas del negocio.

---

# 🏢 Escenario del módulo

El escenario presentado corresponde a un equipo de soporte de productos.

La organización posee documentos almacenados en SharePoint Online con información como:

* Especificaciones técnicas
* FAQ
* Garantías
* Reparaciones
* Devoluciones

El objetivo es construir un agente capaz de responder preguntas utilizando esta información mediante lenguaje natural.

---

# ⚙️ ¿Qué se construirá?

Se crea un agente declarativo de soporte técnico que:

* Utiliza documentos empresariales
* Responde preguntas en lenguaje natural
* Funciona dentro de Microsoft 365 Copilot
* Puede publicarse en Microsoft Teams

---

# 🛠️ Copilot Studio

## 🖥️ Plataforma no-code

Microsoft Copilot Studio proporciona una experiencia visual sin código para crear agentes basados en IA generativa.

Permite:

* Diseñar agentes
* Configurar instrucciones
* Agregar conocimiento
* Publicar soluciones
* Validar comportamiento

Sin necesidad de programación tradicional.

---

# 📋 Requisitos previos

Para crear agentes declarativos:

## ✅ Licencias

Se requiere licencia de:

* Microsoft 365 Copilot

---

## ✅ Permisos

El creador debe:

* Tener acceso a Copilot Studio
* Poseer permisos para crear agentes
* Contar con un entorno habilitado

---

# 🏗️ Tipos de agentes

## 🔹 Agentes personalizados

Se crean desde:

* Crear → Nuevo agente
* Agentes → Nuevo agente

---

## 🔹 Agentes declarativos

Se crean específicamente para Microsoft 365 Copilot desde:

1. Agentes
2. Microsoft 365 Copilot
3. Agregar agente

---

# 🤖 Creación conversacional mediante IA generativa

Copilot Studio utiliza IA generativa para:

* Crear el agente
* Generar configuración inicial
* Sugerir prompts
* Configurar propiedades

También es posible realizar configuración manual.

---

# 🧪 Test Canvas

Copilot Studio incluye un entorno de prueba que permite:

* Validar comportamiento
* Refinar respuestas
* Ajustar instrucciones
* Probar antes de publicar

Esto facilita un desarrollo iterativo.

---

# 🧠 Instrucciones personalizadas

## 📌 ¿Qué son?

Las instrucciones son directivas que controlan:

* Comportamiento
* Tono
* Restricciones
* Estilo de respuesta
* Funcionalidades

---

# 🎯 Componentes principales de las instrucciones

## ✅ Objetivo

Define:

* Qué hace el agente
* Qué problemas resuelve

---

## ✅ Directrices generales

Incluyen:

* Restricciones
* Reglas
* Tono
* Comportamiento esperado

---

## ✅ Aptitudes

Definen capacidades específicas del agente.

---

# ✍️ Buenas prácticas de Prompt Engineering

Las instrucciones deben responder preguntas como:

## ✅ Funcionalidades

* ¿Qué puede hacer?
* ¿Qué NO puede hacer?

---

## ✅ Tono y personalidad

* ¿Debe ser formal?
* ¿Debe ser técnico?
* ¿Debe ser amigable?

---

## ✅ Fuentes de información

* ¿Qué datos puede utilizar?

---

## ✅ Estrategia de fallback

* ¿Qué hacer si no encuentra información?

---

# 💡 Características de buenas instrucciones

Las instrucciones efectivas deben ser:

* Claras
* Específicas
* Estructuradas
* Precisas

Esto mejora:

* Calidad de respuestas
* Consistencia
* Confiabilidad

---

# 🌍 Grounding personalizado

## 📌 ¿Qué es el grounding?

El grounding conecta el LLM con información real y empresarial.

Permite:

* Mejorar precisión
* Aumentar relevancia
* Reducir alucinaciones
* Incorporar contexto organizacional

---

# 📂 Tipos de grounding soportados

## ✅ SharePoint

El agente puede conectarse a:

* Sitios
* Bibliotecas de SharePoint Online

### Características:

* Hasta 4 rutas
* Respeta permisos del usuario
* Usa seguridad de Microsoft 365

⚠️ No soporta:

* Archivos individuales
* Páginas únicas

---

## ✅ Copilot Connectors

Los conectores de Copilot permiten extender Microsoft Graph con datos empresariales personalizados.

Esto permite:

* Integrar sistemas externos
* Incorporar información corporativa
* Exponer datos personalizados al agente

---

## ✅ Web Search

El agente puede usar búsqueda web pública mediante Bing.

---

# 🔐 Seguridad

El grounding utiliza permisos de Microsoft 365.

El agente:

✅ Solo accede a información permitida para el usuario.

---

# ➕ Agregar conocimiento

El conocimiento se agrega desde:

* Página de información general del agente
* Botón “Agregar conocimiento”

Un agente puede combinar múltiples fuentes.

---

# 💬 Mensajes sugeridos

## 📌 ¿Qué son?

Los mensajes sugeridos (*Starter Prompts* o *Suggested Prompts*) son prompts de ejemplo mostrados al usuario.

Sirven para:

* Iniciar conversaciones rápidamente
* Mostrar capacidades
* Guiar interacciones
* Mejorar adopción

---

# ⚙️ Creación de prompts sugeridos

## 🤖 Generación automática

Copilot Studio puede generarlos automáticamente usando IA generativa.

---

## ✍️ Edición manual

También pueden:

* Editarse
* Crearse manualmente
* Personalizarse

Desde la página de información general del agente.

---

# 📌 Límite de prompts

Un agente puede tener:

* Hasta 6 mensajes sugeridos

---

# 💡 Buenas prácticas para prompts sugeridos

## ✅ Consultas frecuentes

Usar prompts simples como:

* “¿Cuál es la política de garantías?”
* “¿Cómo solicito una devolución?”

---

## ✅ Consultas avanzadas

También es recomendable incluir prompts sofisticados que:

* Muestren potencial del agente
* Aprovechen capacidades del LLM
* Generen respuestas más complejas

---

# 🧪 Uso para testing

Los prompts sugeridos también sirven para:

* Validar comportamiento
* Probar respuestas
* Refinar el agente

---

# 🚀 Publicación del agente

Los agentes pueden publicarse en:

* Microsoft 365 Copilot
* Microsoft Teams

---

# 🌐 Opciones de distribución

## 🔗 Compartir vínculo

Genera un deep link hacia Teams.

---

## 👥 Compartir con usuarios o grupos

Permite:

* Compartir con compañeros
* Dar acceso a grupos de seguridad

---

## 🏢 Publicar para toda la organización

El administrador puede:

* Agregar el agente al catálogo organizacional
* Distribuirlo masivamente

---

## 📦 Descargar ZIP

Permite:

* Exportar el agente
* Revisarlo
* Cargarlo manualmente

---

# 🔎 Acceso a agentes declarativos

Los agentes aparecen en:

* Microsoft 365 Copilot Agents
* Herramientas

⚠️ No aparecen como agentes personalizados principales.

---

# 🧪 Laboratorios del módulo

## 📎 Laboratorio 1 — Crear el primer agente declarativo

[Laboratorio: Create your first declarative agent](https://microsoftlearning.github.io/MS-4022-Extend-Microsoft-365-Copilot-in-Copilot-Studio/Instructions/Labs/01-Build-your-first-declarative-agent/01-create-declarative-agent.html?utm_source=chatgpt.com)

---

## 📎 Laboratorio 2 — Incorporar conocimiento personalizado

[Laboratorio: Add custom knowledge to a declarative agent](https://microsoftlearning.github.io/MS-4022-Extend-Microsoft-365-Copilot-in-Copilot-Studio/Instructions/Labs/01-Build-your-first-declarative-agent/02-add-custom-knowledge.html?utm_source=chatgpt.com)

---

## 📎 Laboratorio 3 — Agregar mensajes sugeridos

[Laboratorio: Add starter prompts to a declarative agent](https://microsoftlearning.github.io/MS-4022-Extend-Microsoft-365-Copilot-in-Copilot-Studio/Instructions/Labs/01-Build-your-first-declarative-agent/03-add-starter-prompts.html?utm_source=chatgpt.com)

---

# 📚 Resumen final del módulo

En este módulo aprendiste a:

## ✅ Crear agentes declarativos

Utilizando la experiencia conversacional basada en IA generativa de Microsoft Copilot Studio.

---

## ✅ Configurar instrucciones personalizadas

Definiendo:

* Tono
* Restricciones
* Capacidades
* Objetivos
* Comportamiento

---

## ✅ Incorporar grounding y conocimiento empresarial

Conectando el agente a:

* SharePoint
* Copilot Connectors
* Web Search

---

## ✅ Crear mensajes sugeridos

Para:

* Mejorar experiencia de usuario
* Guiar conversaciones
* Mostrar funcionalidades
* Validar comportamiento

---

## ✅ Publicar el agente

Distribuyéndolo en:

* Microsoft 365 Copilot
* Microsoft Teams

---

## ✅ Validar respuestas

Usando el entorno de pruebas de Copilot Studio.

---

# 🧠 Conceptos clave del módulo

## ✅ Declarative Agents

Extensiones especializadas de Microsoft 365 Copilot.

---

## ✅ Prompt Engineering

Diseño efectivo de instrucciones para controlar comportamiento del agente.

---

## ✅ Grounding

Uso de datos empresariales reales para mejorar respuestas.

---

## ✅ Knowledge Sources

Fuentes de datos utilizadas por el agente.

---

## ✅ Starter Prompts

Prompts sugeridos para iniciar conversaciones.

---

## ✅ No-Code AI Development

Creación de agentes mediante herramientas visuales y IA generativa.

---

# 📖 Recursos adicionales

## 📘 Introducción a agentes declarativos para Microsoft 365 Copilot

Microsoft 365 Copilot

---

## 📘 Extensión de Microsoft 365 Copilot con agentes

Microsoft Copilot Studio

---

## 📘 Introducción a Copilot Studio

Microsoft Copilot Studio

---

# 📌 Idea clave final

Los agentes declarativos permiten extender Microsoft 365 Copilot mediante IA generativa, grounding empresarial e instrucciones personalizadas, utilizando una experiencia no-code en Copilot Studio para crear asistentes especializados, seguros y conectados con la información real de la organización.
