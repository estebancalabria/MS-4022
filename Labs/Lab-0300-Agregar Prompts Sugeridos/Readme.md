# Laboratorio Paso a Paso – Agregar Suggested Prompts a un agente en Microsoft Copilot Studio

## Objetivo del laboratorio

En este laboratorio vas a:

* Configurar Suggested Prompts personalizados.
* Reemplazar los prompts generados automáticamente.
* Republicar el agente.
* Actualizar el agente en Microsoft 365 Copilot.
* Validar los prompts sugeridos en la interfaz de usuario.

---

# Requisitos previos

Antes de comenzar necesitás:

* Tener acceso a Microsoft Copilot Studio.
* Haber creado previamente el agente:

  * **Product Support**
* Haber publicado el agente anteriormente.
* Tener acceso a Microsoft 365 Copilot.

---

# Duración estimada

⏱️ Aproximadamente 10 minutos.

---

# Concepto importante – Suggested Prompts

## ¿Qué son los Suggested Prompts?

Los Suggested Prompts son preguntas sugeridas que aparecen en la interfaz del agente para ayudar al usuario a comenzar rápidamente una conversación.

Ayudan a:

* Guiar al usuario.
* Mostrar capacidades del agente.
* Mejorar la experiencia de uso.
* Reducir la fricción inicial.

---

# Parte 1 – Abrir el agente

## Paso 1 – Abrir Copilot Studio

1. Abrí el navegador web.
2. Ingresá a:

[Microsoft Copilot Studio](https://copilotstudio.microsoft.com?utm_source=chatgpt.com)

3. Iniciá sesión con tu cuenta Microsoft 365.

---

## Paso 2 – Navegar a Agents

1. En el menú lateral izquierdo:

   * Seleccioná **Agents**

---

## Paso 3 – Abrir Microsoft 365 Copilot

1. Seleccioná:

   * **Copilot for Microsoft 365**

---

## Paso 4 – Abrir el agente Product Support

1. Seleccioná el agente:

   * **Product Support**

Se abrirá la página Overview del agente.

---

# Parte 2 – Editar Suggested Prompts

## Paso 5 – Ubicar Suggested Prompts

1. En la página Overview:

   * Buscá la sección:

     * **Suggested Prompts**

⚠️ Vas a notar que Copilot Studio creó prompts automáticamente durante la creación del agente.

---

## Paso 6 – Editar Suggested Prompts

1. Hacé clic en el ícono:

   * **Edit**

---

## Paso 7 – Reemplazar los prompts existentes

Eliminá TODOS los prompts existentes.

Luego agregá exactamente los siguientes:

---

## Prompt 1

### Título

```text id="3mn0kw"
Eagle Air
```

### Prompt

```text id="t0a2nt"
Tell me about Eagle Air
```

---

## Prompt 2

### Título

```text id="yjlwm6"
Return policy
```

### Prompt

```text id="rj2m3w"
What is the returns policy
```

---

## Prompt 3

### Título

```text id="h4g9wz"
Product information
```

### Prompt

```text id="3gt0qn"
Can you provide information on a specific product?
```

---

## Prompt 4

### Título

```text id="rqpjm4"
Product troubleshooting
```

### Prompt

```text id="jq5yn7"
I'm having trouble with a product. Can you help me troubleshoot the issue?
```

---

## Prompt 5

### Título

```text id="29fdrj"
Repair information
```

### Prompt

```text id="obwn3p"
Can you provide information on how to get a product repaired?
```

---

## Prompt 6

### Título

```text id="m4x2ra"
Contact support
```

### Prompt

```text id="xzt0af"
How can I contact support for help?
```

---

## Paso 8 – Guardar cambios

1. Hacé clic en:

   * **Save**

⏳ Esperá a que los cambios se guarden correctamente.

---

# Parte 3 – Republicar el agente

## Paso 9 – Publicar nuevamente

1. En la esquina superior derecha:

   * Hacé clic en **Publish**

---

## Paso 10 – Confirmar publicación

1. En la ventana modal:

   * Hacé clic nuevamente en:

     * **Publish**

⏳ Esperá unos momentos.

---

# Parte 4 – Copiar Share Link

## Paso 11 – Abrir Availability Options

Cuando finalice la publicación:

1. Aparecerá la ventana:

   * **Availability options**

---

## Paso 12 – Copiar el enlace

1. En la sección:

   * **Share link**

2. Hacé clic en:

   * **Copy**

---

# Parte 5 – Actualizar el agente en Microsoft 365 Copilot

## Paso 13 – Abrir el Share Link

1. Abrí una nueva pestaña del navegador.
2. Pegá el Share Link.
3. Presioná Enter.

---

## Paso 14 – Actualizar el agente

Aparecerá una ventana del agente Product Support.

1. Debajo del nombre del agente:

   * Hacé clic en:

     * **Update now**

⏳ Esperá unos segundos mientras el agente se actualiza.

---

## Paso 15 – Finalizar actualización

Cuando termine:

1. Cerrá la ventana modal.

---

# Parte 6 – Abrir Microsoft 365 Copilot

## Paso 16 – Abrir Copilot

Si no se abre automáticamente:

1. Desde el menú lateral izquierdo:

   * Seleccioná:

     * Microsoft 365 Copilot

También podés abrirlo desde:

* El menú Apps de Microsoft 365.

---

# Parte 7 – Validar Suggested Prompts

## Paso 17 – Abrir el agente

1. En el panel lateral:

   * Buscá:

     * **Product Support**

2. Seleccionalo.

Ahora ingresarás en la experiencia inmersiva del agente.

---

## Paso 18 – Verificar prompts sugeridos

Debajo del cuadro de conversación deberías ver los prompts sugeridos configurados anteriormente.

Deberían aparecer:

* Eagle Air
* Return policy
* Product information
* Product troubleshooting
* Repair information
* Contact support

✅ Esto confirma que los Suggested Prompts fueron publicados correctamente.

---

# Parte 8 – Probar Suggested Prompts

## Paso 19 – Ejecutar un Suggested Prompt

1. Hacé clic sobre cualquiera de los prompts sugeridos.

Por ejemplo:

```text id="c0qwxm"
Tell me about Eagle Air
```

---

## Paso 20 – Revisar la respuesta

El agente debería:

✅ Responder automáticamente.
✅ Utilizar información del grounding.
✅ Mostrar referencias o citas.
✅ Mantener el tono definido en las instrucciones.

---

# Resultado esperado

Al finalizar el laboratorio deberías haber logrado:

✅ Configurar Suggested Prompts personalizados.
✅ Reemplazar prompts automáticos.
✅ Republicar el agente.
✅ Actualizar el agente en Microsoft 365 Copilot.
✅ Validar prompts sugeridos en la interfaz.
✅ Probar conversaciones guiadas mediante prompts.

---

# Conceptos importantes aprendidos

## Suggested Prompts

Preguntas sugeridas visibles para el usuario que facilitan iniciar conversaciones relevantes.

---

## Experiencia inmersiva

Modo donde el usuario conversa directamente con el agente.

---

## Publicación del agente

Proceso mediante el cual los cambios realizados en Copilot Studio se reflejan en Microsoft 365 Copilot.

---

## Share Link

Enlace utilizado para instalar o actualizar agentes publicados.

---

# Buenas prácticas

## Crear prompts concretos

Los Suggested Prompts deben:

✅ Ser claros.
✅ Ser cortos.
✅ Representar capacidades reales del agente.
✅ Guiar conversaciones útiles.

---

## Evitar prompts genéricos

❌ “Help me”
❌ “Tell me something”

✅ “Can you provide repair information?”
✅ “Recommend a product suitable for a farmer”

---

# Fin del laboratorio

Laboratorio completado exitosamente 🚀
