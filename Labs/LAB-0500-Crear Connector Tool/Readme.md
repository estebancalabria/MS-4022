# Laboratorio Paso a Paso – Crear una Connector Tool en Microsoft Copilot Studio

## Objetivo del laboratorio

En este laboratorio vas a:

* Agregar una Connector Tool a un agente declarativo.
* Utilizar un conector preconstruido de SharePoint.
* Configurar el conector List Folder.
* Personalizar entradas y parámetros.
* Actualizar instrucciones del agente.
* Probar el uso del conector desde el agente.

---

# Requisitos previos

Antes de comenzar necesitás:

* Acceso a Microsoft Copilot Studio.
* Una cuenta Microsoft 365 corporativa o educativa.
* Haber creado previamente:

  * El agente **Product Support**
* Tener un sitio de Microsoft SharePoint llamado:

  * **Product Support**
* Tener una biblioteca/document library llamada:

  * **Products**
* Tener archivos cargados dentro de Products.

---

# Duración estimada

⏱️ Aproximadamente 15 minutos.

---

# Concepto importante – Connector Tools

## ¿Qué es una Connector Tool?

Una Connector Tool permite que un agente interactúe con servicios externos usando conectores preconstruidos.

Por ejemplo:

* SharePoint
* Outlook
* Teams
* Dynamics
* SQL
* Salesforce

En este laboratorio el agente usará SharePoint para listar archivos disponibles.

---

# Escenario del laboratorio

El agente Product Support podrá:

✅ Consultar SharePoint.
✅ Obtener archivos de soporte técnico.
✅ Mostrar archivos disponibles al usuario.
✅ Informar que utilizó el conector SharePoint.

---

# Parte 1 – Abrir Copilot Studio

## Paso 1 – Abrir Copilot Studio

1. Abrí el navegador web.
2. Ingresá a:

[Microsoft Copilot Studio](https://www.copilotstudio.microsoft.com?utm_source=chatgpt.com)

3. Iniciá sesión con tu cuenta Microsoft 365.

---

# Parte 2 – Abrir el agente

## Paso 2 – Ir a Agents

1. En el menú lateral izquierdo:

   * Seleccioná:

     * **Agents**

---

## Paso 3 – Abrir Microsoft 365 Copilot

1. Seleccioná:

   * **Microsoft 365 Copilot**

---

## Paso 4 – Abrir el agente Product Support

1. Dentro de Agents:

   * Seleccioná:

     * **Product Support**

---

# Parte 3 – Agregar Connector Tool

## Paso 5 – Abrir Tools

1. Dentro del agente:

   * Buscá la sección:

     * **Tools**

2. Hacé clic en:

   * **Add tool**

---

## Paso 6 – Filtrar conectores

En la ventana Add tool:

1. Seleccioná:

   * **Connector**

Esto filtrará únicamente herramientas tipo connector.

---

## Paso 7 – Buscar SharePoint

1. En el campo Search:

   * Escribí:

```text id="kt0x5r"
SharePoint
```

2. Hacé clic en:

   * **Search**

⏳ Esperá a que aparezcan los conectores.

---

## Paso 8 – Seleccionar List Folder

1. Buscá y seleccioná:

   * **List Folder SharePoint connector**

⚠️ Asegurate de elegir específicamente:

* List Folder

---

# Parte 4 – Configurar conexión SharePoint

## Paso 9 – Verificar conexión

Aparecerá una ventana mostrando el estado de conexión.

---

## Caso 1 – Ya conectado

Si aparece:

✅ Green checkmark

Podés continuar al siguiente paso.

---

## Caso 2 – Not connected

Si aparece:

❌ Not connected

hacé lo siguiente:

1. Seleccioná el desplegable junto a:

   * **Not connected**

2. Seleccioná:

   * **Create new connection**

---

## Paso 10 – Crear conexión

En la pantalla Connect to SharePoint:

1. Seleccioná:

   * **Connect directly (cloud services)**

2. Hacé clic en:

   * **Create**

---

## Paso 11 – Iniciar sesión

1. Iniciá sesión con tu cuenta Microsoft 365 utilizada para el laboratorio.

⏳ Esperá a que la conexión quede activa.

---

# Parte 5 – Agregar el conector al agente

## Paso 12 – Agregar y configurar

Cuando la conexión esté activa:

1. Hacé clic en:

   * **Add and configure**

⏳ Esperá unos segundos.

---

## Paso 13 – Verificar agregado

El conector debería aparecer en la sección:

* **Tools**

con el nombre:

* List folder - connector tool

---

# Parte 6 – Configurar el conector

## Paso 14 – Abrir configuración del conector

1. Dentro de Tools:

   * Seleccioná:

     * **List folder - connector tool**

---

## Paso 15 – Configurar Name

En el campo Name escribí:

```text id="a4jzv9"
List product support files
```

---

## Paso 16 – Configurar Description

En el campo Description escribí:

```text id="kl7d2n"
List product support files available in the Products folder.
```

---

# Parte 7 – Configurar detalles adicionales

## Paso 17 – Expandir Additional details

1. Activá el toggle:

   * **Additional details**

---

## Paso 18 – Configurar descripción adicional

En el campo Description escribí:

```text id="6xgr4t"
Please log in to access the Product Support SharePoint site.
```

---

# Parte 8 – Configurar Inputs

## Paso 19 – Configurar Site Address

En la sección Inputs:

1. Buscá:

   * **Site Address**

2. En el campo Value ingresá la URL de tu sitio SharePoint.

Formato:

```text id="v2y1kg"
https://DOMAIN.sharepoint.com/sites/ProductSupport
```

⚠️ Reemplazá DOMAIN por tu dominio real de Microsoft 365.

---

## Paso 20 – Configurar File Identifier

1. Buscá:

   * **File Identifier**

2. En el desplegable Fill using:

   * Seleccioná:

     * **Custom value**

---

## Paso 21 – Definir carpeta

En el campo Value escribí:

```text id="m4vrx1"
Products
```

---

# Parte 9 – Guardar cambios

## Paso 22 – Guardar el conector

1. En la parte superior:

   * Hacé clic en:

     * **Save**

---

# Parte 10 – Actualizar instrucciones del agente

## Paso 23 – Editar Details

1. Volvé a la sección:

   * **Details**

2. Hacé clic en:

   * **Edit**

---

## Paso 24 – Agregar instrucciones

En el campo Instructions agregá al final:

```text id="q9m2lh"
When asked about available support resources, use the SharePoint connector to list the files in the Products folder and let the user know the SharePoint Connector was used.
```

---

## Paso 25 – Guardar cambios

1. Hacé clic en:

   * **Save**

---

# Parte 11 – Probar el agente

## Paso 26 – Abrir panel de pruebas

1. Expandí:

   * **Test your agent**

ubicado a la derecha.

---

## Paso 27 – Reiniciar sesión

1. Hacé clic en:

   * **Start new test session**

Esto asegura que el agente utilice la última configuración.

---

# Parte 12 – Ejecutar prueba

## Paso 28 – Realizar consulta

En el cuadro de chat escribí:

```text id="mg4s6v"
What product support files are available?
```

Presioná Enter.

---

# Resultado esperado

El agente debería:

✅ Utilizar el conector SharePoint.
✅ Informar que utilizó el connector.
✅ Listar archivos disponibles dentro de Products.
✅ Obtener datos directamente desde SharePoint.

---

# Conceptos importantes aprendidos

## Connector Tools

Herramientas que permiten integrar servicios externos con agentes.

---

## Prebuilt Connectors

Conectores ya preparados por Microsoft para integraciones comunes.

---

## SharePoint Connectors

Permiten interactuar con:

* archivos,
* carpetas,
* bibliotecas,
* documentos,
* listas.

---

## Tool-enabled Agents

Agentes capaces de utilizar herramientas externas automáticamente.

---

## Dynamic Retrieval

Capacidad de consultar información en tiempo real desde servicios externos.

---

# Buenas prácticas

## Escribir instrucciones claras

El agente necesita instrucciones explícitas para saber:

✅ Cuándo usar la herramienta.
✅ Cómo usarla.
✅ Qué informar al usuario.

---

## Configurar inputs correctamente

Errores comunes:

❌ URL incorrecta
❌ Nombre de carpeta incorrecto
❌ Conector sin autenticación

---

# Troubleshooting

## El conector no responde

Verificá:

* Que SharePoint tenga archivos.
* Que la URL sea correcta.
* Que la conexión esté autenticada.

---

## El agente no usa el connector

Verificá:

* Las instrucciones del agente.
* Que el tool esté agregado.
* Que los cambios hayan sido guardados.

---

# Resultado final esperado

Al finalizar el laboratorio deberías haber logrado:

✅ Crear una Connector Tool.
✅ Configurar un conector SharePoint.
✅ Personalizar propiedades del conector.
✅ Configurar inputs dinámicos.
✅ Actualizar instrucciones del agente.
✅ Validar consultas usando SharePoint.

---

# Fin del laboratorio

Laboratorio completado exitosamente 🚀
