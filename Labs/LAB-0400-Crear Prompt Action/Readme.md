# Laboratorio Paso a Paso – Crear una Prompt Action en Microsoft Copilot Studio

## Objetivo del laboratorio

En este laboratorio vas a:

* Crear una Prompt Action personalizada.
* Configurar variables de entrada.
* Refinar prompts para obtener mejores respuestas.
* Probar el prompt en Copilot Studio.
* Integrar la Prompt Action dentro de un agente.
* Configurar instrucciones para usar la herramienta automáticamente.

---

# Requisitos previos

Antes de comenzar necesitás:

* Acceso a Microsoft Copilot Studio.
* Cuenta Microsoft 365 corporativa o educativa.
* Haber creado previamente el agente:

  * **Product Support** (opcional para la última parte).

---

# Duración estimada

⏱️ Aproximadamente 15 minutos.

---

# Concepto importante – Prompt Actions

## ¿Qué es una Prompt Action?

Una Prompt Action es una herramienta reutilizable basada en prompts que permite ejecutar tareas específicas usando IA generativa.

Por ejemplo:

* Crear pitches de marketing.
* Resumir texto.
* Generar emails.
* Clasificar contenido.
* Reformular ideas.

Las Prompt Actions pueden ser utilizadas directamente o desde agentes declarativos.

---

# Escenario del laboratorio

Vas a crear una herramienta capaz de:

✅ Recibir ideas desordenadas sobre un producto.
✅ Transformarlas automáticamente en un pitch de marketing profesional.
✅ Aplicar reglas y formato corporativo de Contoso.

---

# Parte 1 – Abrir Copilot Studio

## Paso 1 – Abrir Copilot Studio

1. Abrí el navegador web.
2. Ingresá a:

[Microsoft Copilot Studio](https://copilotstudio.microsoft.com?utm_source=chatgpt.com)

3. Iniciá sesión con tu cuenta Microsoft 365.

---

# Parte 2 – Crear una nueva Prompt Action

## Paso 2 – Abrir la sección Tools

1. En el menú lateral izquierdo:

   * Seleccioná:

     * **Tools**

---

## Paso 3 – Crear nueva herramienta

1. Hacé clic en:

   * **New tool**

---

## Paso 4 – Elegir Prompt

Aparecerá una ventana llamada:

* **New Tool**

1. Seleccioná:

   * **Prompt**

Ahora se abrirá el Prompt Builder.

---

# Parte 3 – Configurar el Prompt

## Paso 5 – Cambiar el nombre

En la parte superior:

1. Seleccioná el nombre generado automáticamente.
2. Reemplazalo por:

```text id="s7n2kc"
Marketing Pitch Prompt
```

---

## Paso 6 – Configurar instrucciones iniciales

En el campo **Instructions** escribí:

```text id="ylm3dv"
Create a marketing pitch for a product based on a
```

⚠️ No agregues punto final adicional.

---

# Parte 4 – Crear variable de entrada

## Paso 7 – Agregar contenido dinámico

1. Colocá el cursor al final de la oración.
2. Hacé clic en:

   * **Add content**

---

## Paso 8 – Elegir Text

1. Seleccioná:

   * **Text**

---

## Paso 9 – Configurar variable

En el campo **Name** escribí:

```text id="jz5m0x"
Draft
```

---

## Paso 10 – Agregar Sample Data

En el campo **Sample data** escribí exactamente:

```text id="9w4a2g"
The Mighty Mechanical Pencil is new, exciting, and useful. It's not only the first of its kind pencil, but it's fun to use.
```

---

## Paso 11 – Confirmar variable

1. Hacé clic en:

   * **Close**

Ahora la variable aparecerá dentro del prompt.

---

# Parte 5 – Probar el Prompt

## Paso 12 – Ejecutar prueba

1. Encima del cuadro Instructions:

   * Hacé clic en:

     * **Test**

Copilot Studio ejecutará el prompt utilizando el texto de ejemplo.

---

## Paso 13 – Revisar la respuesta

En la sección:

* **Model response**

vas a ver el pitch generado automáticamente.

---

# Parte 6 – Refinar el Prompt

## Paso 14 – Mejorar instrucciones

Ahora vas a mejorar la calidad y consistencia del resultado.

En el cuadro **Instructions**, agregá al final del texto existente:

```text id="l8qg1k"
The pitch should follow the following Contoso guidelines:
- Start with a brief hook
- Describe unique value proposition
- End with a call-to-action
- Use an exciting and influential tone
```

---

# Parte 7 – Probar nuevamente

## Paso 15 – Ejecutar nueva prueba

1. Hacé clic nuevamente en:

   * **Test**

---

## Paso 16 – Analizar diferencias

Compará la nueva respuesta con la anterior.

Ahora el pitch debería:

✅ Tener estructura.
✅ Tener un hook inicial.
✅ Explicar valor diferencial.
✅ Finalizar con call-to-action.
✅ Tener tono más comercial.

---

# Concepto importante – Prompt Engineering

## Refinamiento iterativo

Los prompts normalmente se refinan iterativamente para:

* Obtener respuestas más consistentes.
* Controlar tono.
* Controlar formato.
* Reducir ambigüedad.

---

# Parte 8 – Guardar la Prompt Action

## Paso 17 – Guardar el Prompt

1. Hacé clic en:

   * **Save**

La Prompt Action queda creada.

---

# Parte 9 – Agregar la Prompt Action a un agente (Opcional)

⚠️ Esta sección requiere haber creado previamente el agente Product Support.

---

# Parte 10 – Abrir el agente

## Paso 18 – Ir a Agents

1. En el menú lateral:

   * Seleccioná:

     * **Agents**

---

## Paso 19 – Abrir Microsoft 365 Copilot

1. Seleccioná:

   * **Microsoft 365 Copilot**

---

## Paso 20 – Abrir Product Support

1. Seleccioná:

   * **Product Support**

---

# Parte 11 – Agregar la herramienta

## Paso 21 – Abrir sección Tools

1. Dentro del agente:

   * Buscá la sección:

     * **Tools**

2. Hacé clic en:

   * **Add tool**

---

## Paso 22 – Filtrar por Prompt

1. Seleccioná el filtro:

   * **Prompt**

---

## Paso 23 – Seleccionar herramienta

1. Seleccioná:

   * **Marketing Pitch Prompt**

---

## Paso 24 – Agregar herramienta

1. Hacé clic en:

   * **Add and configure**

⏳ Esperá unos segundos.

La herramienta aparecerá dentro de Tools.

---

# Parte 12 – Actualizar instrucciones del agente

## Paso 25 – Editar instrucciones

En el campo **Instructions** agregá al final:

```text id="v5y9pb"
Use the Marketing Pitch Prompt tool to craft pitches for products that follow Contoso guidelines based on users' draft ideas.
```

---

## Paso 26 – Guardar cambios

1. Hacé clic en:

   * **Save**

---

# Parte 13 – Actualizar Suggested Prompts

## Paso 27 – Editar Suggested Prompts

1. Buscá la sección:

   * **Suggested prompts**

2. Reemplazá el prompt:

   * **Eagle Air**

por el siguiente:

---

## Título

```text id="ys7p4m"
Marketing Pitch
```

---

## Prompt

```text id="whm0lr"
Create a marketing pitch following Contoso guidelines based on the following draft:
```

---

## Paso 28 – Guardar Suggested Prompts

1. Hacé clic en:

   * **Save**

---

# Resultado esperado

Al finalizar el laboratorio deberías haber logrado:

✅ Crear una Prompt Action personalizada.
✅ Configurar variables dinámicas.
✅ Refinar prompts usando Prompt Engineering.
✅ Ejecutar pruebas iterativas.
✅ Integrar Prompt Actions en agentes.
✅ Configurar instrucciones para uso automático.
✅ Actualizar Suggested Prompts.

---

# Conceptos importantes aprendidos

## Prompt Builder

Interfaz visual para crear prompts reutilizables.

---

## Input Variables

Variables dinámicas utilizadas dentro del prompt.

---

## Prompt Engineering

Proceso de diseñar y refinar prompts para controlar resultados.

---

## Prompt Actions

Herramientas reutilizables basadas en IA generativa.

---

## Tool-enabled Agents

Agentes capaces de utilizar herramientas automáticamente.

---

# Buenas prácticas

## Escribir instrucciones específicas

✅ Definir formato esperado.
✅ Definir tono.
✅ Definir estructura.
✅ Definir restricciones.

---

## Refinar iterativamente

La calidad mejora significativamente al:

* probar,
* comparar,
* ajustar,
* volver a probar.

---

# Fin del laboratorio

Laboratorio completado exitosamente 🚀
