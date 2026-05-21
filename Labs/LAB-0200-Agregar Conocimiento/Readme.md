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
* Haber creado previamente el agente **Product Support**.

> ⚠️ **Importante para instructores:** Creá el sitio de SharePoint y subí los archivos **al menos 30 minutos antes** de comenzar la clase. SharePoint necesita tiempo para indexar el contenido antes de que Copilot Studio pueda acceder a él.

---

# Duración estimada

⏱️ Aproximadamente 20 minutos (sin contar el tiempo de preparación previa).

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

1. Buscá el archivo `Products.zip`.
2. Hacé clic en **Download raw file**.

Se descargará el archivo ZIP.

---

## Paso 3 – Extraer el contenido

1. Abrí la carpeta descargada.
2. Hacé clic derecho sobre `Products.zip`.
3. Seleccioná **Extract all**.
4. Extraé el contenido en una carpeta llamada:

```
Products
```

⚠️ Recordá dónde guardaste esta carpeta.

---

# Parte 2 – Crear un sitio de SharePoint

## Paso 4 – Abrir Microsoft 365

1. Abrí el navegador.
2. Ingresá a [Microsoft 365 Portal](https://m365.cloud.microsoft).
3. Iniciá sesión con tu cuenta Microsoft 365.

---

## Paso 5 – Abrir SharePoint

1. En el menú izquierdo seleccioná el ícono de aplicaciones (grid).
2. Seleccioná **All apps**.
3. Abrí **Microsoft SharePoint**.

---

## Paso 6 – Crear un nuevo sitio

1. En el menú izquierdo seleccioná **Compilar** (o **Create site**).
2. Seleccioná **Nuevo sitio** (o **New site**).

---

## Paso 7 – Elegir tipo de sitio

1. Seleccioná **Team site**.

---

## Paso 8 – Seleccionar plantilla

1. Seleccioná **Standard team**.
2. Hacé clic en **Use template**.

---

## Paso 9 – Definir nombre del sitio

En el campo del nombre escribí:

```
Product support
```

Luego hacé clic en **Next**.

---

## Paso 10 – Configurar privacidad

1. Cambiá **Privacy settings** a **Public**.

---

## Paso 11 – Crear el sitio

1. Hacé clic en **Create site**.
2. Esperá unos momentos hasta que se habilite el botón **Finish**.
3. Hacé clic en **Finish**.

Ahora estarás dentro del nuevo sitio de SharePoint.

---

# Parte 3 – Crear una biblioteca de documentos

## Paso 12 – Acceder al contenido del sitio

1. En el menú izquierdo seleccioná **Contenido del sitio**.
2. Hacé clic en **+ Nuevo** (o **New**).
3. Seleccioná **Biblioteca de documentos** (Document library).

> 💡 **Nota:** En la versión moderna de SharePoint en español, el botón **New** puede aparecer como **+ Nuevo** dentro de **Contenido del sitio**, no en la página de inicio del sitio.

---

## Paso 13 – Elegir biblioteca vacía

1. Seleccioná **Blank library**.

---

## Paso 14 – Asignar nombre

En el campo Name escribí:

```
Products
```

Luego hacé clic en **Create**.

Ahora se abrirá la biblioteca Products.

---

# Parte 4 – Subir documentos

## Paso 15 – Subir archivos

1. Dentro de la biblioteca Products hacé clic en **Upload** (o **Cargar**).
2. Seleccioná **Files** (Archivos).

---

## Paso 16 – Seleccionar archivos

1. Navegá hasta la carpeta `Products`.
2. Seleccioná todos los archivos.
3. Hacé clic en **Open**.

⏳ Esperá a que termine la carga. Los archivos aparecerán en SharePoint.

---

# Parte 5 – Obtener la URL de SharePoint

## Paso 17 – Copiar la URL desde la barra del navegador

1. Asegurate de estar dentro de la biblioteca **Products**.
2. Mirá la barra de direcciones del navegador. Verás una URL similar a:

```
https://TUDOMINIO.sharepoint.com/sites/DemoProductSupport/Products/Forms/AllItems.aspx
```

3. Copiá **únicamente** la parte hasta `/Products`, sin incluir nada después:

```
https://TUDOMINIO.sharepoint.com/sites/DemoProductSupport/Products
```

⚠️ No copies `/Forms/AllItems.aspx` ni ningún parámetro adicional.

Guardá esta URL porque la usarás en el siguiente paso.

---

# Parte 6 – Agregar conocimiento al agente

## Paso 18 – Abrir Copilot Studio

1. Abrí [Microsoft Copilot Studio](https://copilotstudio.microsoft.com).

---

## Paso 19 – Abrir el agente

1. Seleccioná **Agents**.
2. Entrá en **Copilot for Microsoft 365**.
3. Abrí el agente **Product Support**.

---

## Paso 20 – Agregar conocimiento

1. En la sección **Knowledge** hacé clic en **Add Knowledge**.

---

## Paso 21 – Seleccionar SharePoint

1. En el asistente seleccioná **SharePoint**.

> ⚠️ **Atención:** Existen dos opciones de SharePoint en el diálogo. Seleccioná la opción que dice **"SharePoint solo estará disponible para los usuarios finales autenticados"**, **no** la que menciona que los archivos se cargarán a Dataverse.

---

## Paso 22 – Pegar la URL y confirmar

1. Pegá la URL de la biblioteca Products. Ejemplo:

```
https://TUDOMINIO.sharepoint.com/sites/DemoProductSupport/Products
```

2. Hacé clic en **Add** (Agregar).

> ⚠️ **Comportamiento esperado:** Es posible que aparezca el mensaje **"Este elemento no se admite actualmente"** junto a un link que dice **"¿Desea agregarlos de todos modos?"**. Esto es normal. Hacé clic en ese link para continuar.

---

## Paso 23 – Confirmar agregado

1. Hacé clic en **Add to agent**.
2. Esperá aproximadamente un minuto.

Cuando finalice, la biblioteca Products aparecerá en la sección **Knowledge**.

---

# Concepto importante – Seguridad

⚠️ El agente respeta permisos de Microsoft 365. Los usuarios solo podrán acceder a documentos para los que tengan permisos.

---

# Parte 7 – Actualizar instrucciones del agente

## Paso 24 – Editar detalles

1. Dentro del agente, en la sección **Details**, hacé clic en **Edit**.

---

## Paso 25 – Reemplazar instrucciones

Reemplazá **todo** el contenido del campo Instructions por este texto:

```
You are an agent tasked with answering questions about Contoso Electronics products. Start every response by enthusiastically thanking the user for their question or comment, then respond to their question or comment. You will use documents from the Products folder in SharePoint as your source of information. If you can't find the necessary information, you should suggest that the agent should reach out to the team responsible for further assistance. Your responses should be concise and always include a cited source.
```

⚠️ Pegá el texto completo exactamente igual.

---

## Paso 26 – Guardar cambios

1. Hacé clic en **Save**.

---

# Parte 8 – Probar el agente

## Paso 27 – Reiniciar sesión de prueba

1. En el panel **Test your agent** hacé clic en **Start new test session**.

Esto limpia el contexto anterior.

---

# Parte 9 – Realizar pruebas

## Paso 28 – Preguntar sobre Eagle Air

En el chat escribí:

```
Tell me about Eagle Air
```

**Resultado esperado:**

✅ El agente habla sobre Eagle Air.  
✅ Utiliza información de SharePoint.  
✅ Muestra citas o referencias.

---

# Parte 10 – Recomendación de producto

## Paso 29 – Solicitar recomendación

Escribí:

```
Recommend a product suitable for a farmer
```

**Resultado esperado:**

✅ Recomienda Eagle Air.  
✅ Explica por qué es adecuado para agricultores.  
✅ Incluye citas.

---

# Parte 11 – Comparación de productos

## Paso 30 – Comparar productos

Escribí:

```
Explain why the Eagle Air is more suitable than Contoso Quad
```

**Resultado esperado:**

✅ Compara ambos productos.  
✅ Explica ventajas de Eagle Air.  
✅ Se basa en documentos del grounding.

---

# Parte 12 – Validar fallback

## Paso 31 – Hacer una pregunta sin respuesta

Escribí:

```
When was Mark8 released?
```

**Resultado esperado:**

✅ Indica que no tiene información suficiente.  
✅ Recomienda contactar al equipo responsable.

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

## Grounding Data
Información utilizada por el agente para responder con contexto real.

## Citations
Referencias automáticas a documentos utilizados en las respuestas.

## Fallback Responses
Respuestas configuradas para casos donde el agente no encuentra información suficiente.

---

# Notas para el instructor

| Situación | Causa | Solución |
|---|---|---|
| "Este elemento no se admite actualmente" | URL de biblioteca no estándar | Hacer clic en "¿Desea agregarlos de todos modos?" |
| Error al crear el knowledge source | Sitio recién creado, aún no indexado | Crear el sitio con al menos 30 min de anticipación |
| No aparece la opción "Document library" en New | Estás dentro de la biblioteca, no en el sitio | Ir a Contenido del sitio → + Nuevo |
| Dos opciones de SharePoint en Add Knowledge | Son opciones distintas | Usar la que NO menciona Dataverse |

---

# Fin del laboratorio

Laboratorio completado exitosamente 🚀
