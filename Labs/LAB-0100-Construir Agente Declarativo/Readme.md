# Laboratorio Paso a Paso – Crear un Agente Declarativo en Microsoft Copilot Studio

## Objetivo del laboratorio

En este laboratorio vas a:

* Crear un agente declarativo en Microsoft Copilot Studio.
* Configurar instrucciones personalizadas.
* Probar el agente dentro de Copilot Studio.
* Publicar el agente en Microsoft 365 Copilot.
* Probar el agente en la experiencia inmersiva y contextual.

---

# Requisitos previos

Antes de comenzar asegurate de tener:

* Una cuenta corporativa o educativa de Microsoft 365.
* Permisos para usar Microsoft Copilot Studio.
* Licencia de Microsoft 365 Copilot habilitada.
* Acceso a Internet.
* Navegador web actualizado (Microsoft Edge o Google Chrome recomendado).

---

# Duración estimada

⏱️ Aproximadamente 20 minutos.

---

# Parte 1 – Ingresar a Microsoft Copilot Studio

## Paso 1 – Abrir Copilot Studio

1. Abrí tu navegador web.
2. Ingresá a:

[Microsoft Copilot Studio](https://copilotstudio.microsoft.com?utm_source=chatgpt.com)

3. Iniciá sesión con tu cuenta corporativa o educativa.

---

## Paso 2 – Configuración inicial (si aparece)

Es posible que aparezcan algunas pantallas iniciales.

### Si aparece “Welcome to Microsoft Copilot Studio”

1. Seleccioná tu país o región.
2. Hacé clic en **Get Started**.

---

### Si aparece “Welcome to Copilot Studio!”

1. Hacé clic en **Skip**.

---

# Parte 2 – Crear un agente declarativo

## Paso 3 – Ir a la sección Agents

1. En el menú lateral izquierdo buscá y seleccioná:

* **Agents**

---

## Paso 4 – Entrar a Microsoft 365 Copilot

1. Dentro de la pantalla de agentes:

   * Seleccioná **Microsoft 365 Copilot**.

---

## Paso 5 – Crear un nuevo agente

1. En la sección **Agents**:

   * Hacé clic en **Add**.

Ahora se abrirá la pantalla de creación del agente.

---

# Parte 3 – Configurar el agente

## Paso 6 – Completar el nombre del agente

En el campo **Name** escribí exactamente:

```text
Product support
```

---

## Paso 7 – Completar la descripción

En el campo **Description** escribí exactamente:

```text
A product support agent that can answer queries about Contoso Electronics products.
```

---

## Paso 8 – Configurar las instrucciones del agente

En el cuadro **Instructions** pegá exactamente el siguiente contenido:

```text
- You are an agent tasked with answering questions about Contoso Electronics products.
- Start every response to the user with "Thanks for using a Copilot agent!\n\n" and then answer the questions and help the user.
- Do not answer questions unrelated to Contoso Electronics products.
- Maintain a helpful and approachable tone throughout interactions.
```

⚠️ Importante:

* Respetá los guiones.
* Respetá las comillas.
* Pegá el texto completo.

---

## Paso 9 – Crear el agente

1. En la parte superior de la pantalla:

   * Hacé clic en **Create**.

⏳ Esperá unos segundos.

Luego se abrirá la página principal del agente.

---

# Parte 4 – Probar el agente en Copilot Studio

## Paso 10 – Verificar el estado de publicación

En la pantalla principal del agente:

1. Buscá la sección:

   * **Publish details**

2. Verificá que indique que el agente:

   * **No está publicado**.

---

## Paso 11 – Abrir el panel de pruebas

Si no aparece el panel lateral derecho:

1. Hacé clic en el botón:

   * **Test**

Este botón está cerca de **Publish**.

---

## Paso 12 – Probar el agente

En el cuadro de chat del panel de prueba:

1. Escribí:

```text
What can you do?
```

2. Presioná Enter.

---

## Paso 13 – Analizar la respuesta

Esperá la respuesta del agente.

La respuesta debería comenzar con:

```text
Thanks for using a Copilot agent!
```

✅ Esto confirma que las instrucciones fueron configuradas correctamente.

---

# Parte 5 – Publicar el agente

## Paso 14 – Iniciar publicación

1. En la parte superior:

   * Hacé clic en **Publish**.

---

## Paso 15 – Completar información de publicación

Aparecerá una ventana de configuración.

En el campo **Short description** reemplazá el contenido por:

```text
Answers questions about Contoso Electronics products
```

---

## Paso 16 – Mantener el resto de opciones

1. Dejá los valores predeterminados del resto de los campos.
2. Hacé clic nuevamente en:

   * **Publish**

---

## Paso 17 – Esperar la publicación

⏳ Esperá unos minutos.

⚠️ Muy importante:

* NO cierres la ventana.
* NO actualices la página.

---

# Parte 6 – Obtener el enlace del agente

## Paso 18 – Copiar el Share Link

Cuando finalice la publicación:

1. Aparecerá la ventana:

   * **Availability options**

2. En la sección:

   * **Share link**

3. Hacé clic en:

   * **Copy**

4. Luego hacé clic en:

   * **Done**

---

# Parte 7 – Abrir el agente en Microsoft 365 Copilot

## Paso 19 – Abrir el enlace compartido

1. Abrí una nueva pestaña del navegador.
2. Pegá el enlace copiado.
3. Presioná Enter.

---

## Paso 20 – Agregar el agente

Aparecerá una ventana con información del agente.

1. Hacé clic en:

   * **Add**

⏳ Esperá unos segundos.

El agente se abrirá dentro de Microsoft 365 Copilot.

---

# Parte 8 – Probar el agente en Microsoft 365 Copilot

## Paso 21 – Verificar experiencia inmersiva

En el panel lateral deberías ver:

* **Product Support** seleccionado.

Esto significa que estás hablando directamente con el agente.

---

## Paso 22 – Realizar una prueba

En el chat escribí:

```text
What can you do?
```

Presioná Enter.

---

## Paso 23 – Validar la respuesta

La respuesta debería comenzar con:

```text
Thanks for using a Copilot agent!
```

✅ Esto confirma que el agente funciona correctamente en Microsoft 365 Copilot.

---

# Parte 9 – Probar el modo contextual (in-context)

## Paso 24 – Crear un nuevo chat

1. En la barra lateral:

   * Hacé clic en **New chat**.

Esto sale del chat inmersivo del agente.

---

## Paso 25 – Invocar el agente usando @

En el cuadro de mensaje:

1. Escribí:

```text
@
```

Aparecerá una lista de agentes disponibles.

---

## Paso 26 – Seleccionar el agente

1. Seleccioná:

   * **Product Support**

Debería aparecer el mensaje:

```text
Chatting with Product Support
```

✅ Esto significa que el agente está funcionando en modo contextual.

---

## Paso 27 – Probar nuevamente

Escribí:

```text
What can you do?
```

y enviá el mensaje.

---

## Paso 28 – Verificar el comportamiento

Esperá la respuesta.

El agente debería respetar nuevamente las instrucciones configuradas.

---

# Parte 10 – Salir del modo contextual

## Paso 29 – Finalizar conversación contextual

1. En el mensaje:

   * **Chatting with Product Support**

2. Hacé clic en:

   * **X**

Ahora volvés a conversar directamente con Copilot.

---

# Resultado esperado

Al finalizar este laboratorio deberías haber logrado:

✅ Crear un agente declarativo.
✅ Configurar instrucciones personalizadas.
✅ Probar el agente en Copilot Studio.
✅ Publicar el agente en Microsoft 365 Copilot.
✅ Utilizar el agente en experiencia inmersiva.
✅ Utilizar el agente en experiencia contextual usando @.

---

# Conceptos importantes aprendidos

## Agente declarativo

Un agente declarativo permite extender Microsoft 365 Copilot utilizando instrucciones, conocimiento y acciones sin necesidad de desarrollar una aplicación compleja.

---

## Experiencia inmersiva

El usuario conversa directamente con el agente.

---

## Experiencia contextual (In-context)

El agente participa dentro de una conversación normal con Copilot utilizando `@`.

---

# Fin del laboratorio

Laboratorio completado exitosamente 🚀
