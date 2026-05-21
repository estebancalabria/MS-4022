# Laboratorio Paso a Paso – Agregar conocimiento personalizado a un agente en Microsoft Copilot Studio

## Objetivo del laboratorio

En este laboratorio vas a:

* Preparar documentos de productos.
* Crear un sitio de SharePoint.
* Crear una biblioteca de documentos.
* Subir archivos de ejemplo.
* Configurar conocimiento personalizado en un agente.
* Actualizar instrucciones del agente.
* Probar el grounding usando documentos reales.

---

# Requisitos previos

Antes de comenzar necesitás:

* Una cuenta corporativa o educativa de Microsoft 365.
* Permisos para usar Microsoft Copilot Studio.
* Acceso a Microsoft SharePoint.
* Un navegador web actualizado.
* Haber creado previamente el agente:

  * **Product Support**

---

# Duración estimada

⏱️ Aproximadamente 20 minutos.

---

# Concepto importante – Grounding

## ¿Qué es grounding?

Grounding significa que el agente utiliza documentos reales como fuente de información para responder preguntas con mayor precisión.

En este laboratorio el agente utilizará documentos almacenados en SharePoint.

---

# Parte 1 – Descargar los archivos de ejemplo

## Paso 1 – Abrir el repositorio del curso

1. Abrí el navegador web.
2. Ingresá al repositorio GitHub del curso.

---

## Paso 2 – Descargar el archivo ZIP

1. Buscá el archivo:

   * `Products.zip`

2. Hacé clic en:

   * **Download raw file**

Se descargará el archivo ZIP.

---

## Paso 3 – Extraer el contenido

1. Abrí la carpeta descargada.

2. Hacé clic derecho sobre:

   * `Products.zip`

3. Seleccioná:

   * **Extract all**

4. Extraé el contenido en una carpeta llamada:

```text id="ndtq7z"
Products
```

⚠️ Recordá dónde guardaste esta carpeta.

---

# Parte 2 – Crear un sitio de SharePoint

## Paso 4 – Abrir Microsoft 365

1. Abrí el navegador.
2. Ingresá a:

[Microsoft 365 Portal](https://m365.cloud.microsoft?utm_source=chatgpt.com)

3. Iniciá sesión con tu cuenta Microsoft 365.

---

## Paso 5 – Abrir SharePoint

1. En el menú izquierdo:

   * Seleccioná el ícono de aplicaciones (grid).

2. Seleccioná:

   * **All apps**

3. Abrí:

   * Microsoft SharePoint

---

## Paso 6 – Crear un nuevo sitio

1. En el menú izquierdo:

   * Seleccioná **Create site**

---

## Paso 7 – Elegir tipo de sitio

1. Seleccioná:

   * **Team site**

---

## Paso 8 – Seleccionar plantilla

1. En la pantalla de templates:

   * Seleccioná **Standard team**

2. Hacé clic en:

   * **Use template**

---

## Paso 9 – Definir nombre del sitio

En el campo del nombre escribí:

```text id="rk9x6s"
Product support
```

Luego:

1. Hacé clic en:

   * **Next**

---

## Paso 10 – Configurar privacidad

1. Cambiá:

   * **Privacy settings**

2. Seleccioná:

   * **Public**

---

## Paso 11 – Crear el sitio

1. Hacé clic en:

   * **Create site**

⏳ Esperá unos momentos.

Cuando se habilite:

2. Hacé clic en:

   * **Finish**

Ahora estarás dentro del nuevo sitio de SharePoint.

---

# Parte 3 – Crear una biblioteca de documentos

## Paso 12 – Crear biblioteca

1. Dentro del sitio:

   * Hacé clic en **New**

2. Seleccioná:

   * **Document library**

---

## Paso 13 – Elegir biblioteca vacía

1. Seleccioná:

   * **Blank library**

---

## Paso 14 – Asignar nombre

En el campo Name escribí:

```text id="f9g7ry"
Products
```

Luego:

1. Hacé clic en:

   * **Create**

Ahora se abrirá la biblioteca.

---

# Parte 4 – Subir documentos

## Paso 15 – Subir archivos

1. Dentro de la biblioteca Products:

   * Hacé clic en **Upload**

2. Seleccioná:

   * **Files**

---

## Paso 16 – Seleccionar archivos

1. Navegá hasta la carpeta:

   * `Products`

2. Seleccioná todos los archivos.

3. Hacé clic en:

   * **Open**

⏳ Esperá a que termine la carga.

Los archivos aparecerán en SharePoint.

---

# Parte 5 – Obtener la URL de SharePoint

## Paso 17 – Abrir configuración de biblioteca

1. En la parte superior derecha:

   * Hacé clic en el ícono de configuración ⚙️

2. Seleccioná:

   * **Library settings**

3. Luego:

   * **More library settings**

---

## Paso 18 – Copiar la URL

1. Buscá:

   * **Web address**

La URL tendrá un formato similar a:

```text id="srtg8h"
https://DOMAIN.sharepoint.com/sites/ProductSupport/Products
```

⚠️ Importante:

* Copiá solamente hasta `/Products`
* No copies texto adicional.

Guardá la URL porque la usarás más adelante.

---

# Parte 6 – Agregar conocimiento al agente

## Paso 19 – Abrir Copilot Studio

1. Abrí:

[Microsoft Copilot Studio](https://copilotstudio.microsoft.com?utm_source=chatgpt.com)

---

## Paso 20 – Abrir el agente

1. Seleccioná:

   * **Agents**

2. Entrá en:

   * **Copilot for Microsoft 365**

3. Abrí el agente:

   * **Product Support**

---

## Paso 21 – Agregar conocimiento

1. En la sección:

   * **Knowledge**

2. Hacé clic en:

   * **Add Knowledge**

---

## Paso 22 – Seleccionar SharePoint

1. En el asistente:

   * Seleccioná **SharePoint**

---

## Paso 23 – Pegar la URL

1. Pegá la URL de la biblioteca Products.

Ejemplo:

```text id="2xfh7k"
https://DOMAIN.sharepoint.com/sites/ProductSupport/Products
```

2. Hacé clic en:

   * **Add**

---

## Paso 24 – Confirmar agregado

1. Hacé clic en:

   * **Add to agent**

⏳ Esperá aproximadamente un minuto.

Cuando finalice:

* La biblioteca Products aparecerá en la sección Knowledge.

---

# Concepto importante – Seguridad

⚠️ El agente respeta permisos de Microsoft 365.

Esto significa que:

* Los usuarios solo podrán acceder a documentos para los que tengan permisos.

---

# Parte 7 – Actualizar instrucciones del agente

## Paso 25 – Editar detalles

1. Dentro del agente:

   * En la sección **Details**
   * Hacé clic en **Edit**

---

## Paso 26 – Reemplazar instrucciones

Reemplazá TODO el contenido del campo Instructions por este texto:

```text id="6wms0z"
You are an agent tasked with answering questions about Contoso Electronics products. Start every response by enthusiastically thanking the user for their question or comment, then respond to their question or comment. You will use documents from the Products folder in SharePoint as your source of information. If you can't find the necessary information, you should suggest that the agent should reach out to the team responsible for further assistance. Your responses should be concise and always include a cited source.
```

⚠️ Pegá el texto completo exactamente igual.

---

## Paso 27 – Guardar cambios

1. Hacé clic en:

   * **Save**

---

# Parte 8 – Probar el agente

## Paso 28 – Reiniciar sesión de prueba

1. En el panel:

   * **Test your agent**

2. Hacé clic en:

   * **Start new test session**

Esto limpia el contexto anterior.

---

# Parte 9 – Realizar pruebas

## Paso 29 – Preguntar sobre Eagle Air

En el chat escribí:

```text id="kdzjvq"
Tell me about Eagle Air
```

Presioná Enter.

---

## Resultado esperado

La respuesta debería:

✅ Hablar sobre Eagle Air.
✅ Utilizar información de SharePoint.
✅ Mostrar citas o referencias.

---

# Parte 10 – Recomendación de producto

## Paso 30 – Solicitar recomendación

Escribí:

```text id="7pvqol"
Recommend a product suitable for a farmer
```

Presioná Enter.

---

## Resultado esperado

La respuesta debería:

✅ Recomendar Eagle Air.
✅ Explicar por qué es adecuado para agricultores.
✅ Incluir citas.

---

# Parte 11 – Comparación de productos

## Paso 31 – Comparar productos

Escribí:

```text id="jlwm5g"
Explain why the Eagle Air is more suitable than Contoso Quad
```

Presioná Enter.

---

## Resultado esperado

El agente debería:

✅ Comparar ambos productos.
✅ Explicar ventajas de Eagle Air.
✅ Basarse en documentos del grounding.

---

# Parte 12 – Validar fallback

## Paso 32 – Hacer una pregunta sin respuesta

Escribí:

```text id="lnj3gy"
When was Mark8 released?
```

Presioná Enter.

---

## Resultado esperado

El agente debería:

✅ Indicar que no tiene información suficiente.
✅ Recomendar contactar al equipo responsable.

Esto valida el comportamiento definido en las instrucciones.

---

# Resultado final esperado

Al finalizar el laboratorio deberías haber logrado:

✅ Crear un sitio SharePoint.
✅ Crear una biblioteca de documentos.
✅ Subir archivos de grounding.
✅ Conectar SharePoint al agente.
✅ Configurar conocimiento personalizado.
✅ Actualizar instrucciones avanzadas.
✅ Validar respuestas con grounding.
✅ Validar respuestas fallback.

---

# Conceptos clave aprendidos

## Knowledge Sources

Permiten conectar documentos y contenido empresarial al agente.

---

## Grounding Data

Información utilizada por el agente para responder con contexto real.

---

## Citations

Referencias automáticas a documentos utilizados en las respuestas.

---

## Fallback Responses

Respuestas configuradas para casos donde el agente no encuentra información suficiente.

---

# Fin del laboratorio

Laboratorio completado exitosamente 🚀
