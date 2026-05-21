# Soluciones y Dataverse en Power Platform

> **Audiencia:** Desarrolladores y consultores que inician en Power Platform  
> **Nivel:** Introductorio / Intermedio  
> **Aplica a:** Copilot Studio · Power Apps · Power Automate · Dataverse

---

## ¿Qué es Dataverse?

Dataverse es la **base de datos administrada de Microsoft** que funciona como capa de almacenamiento unificada de toda la Power Platform. No es una base de datos que el desarrollador configura ni mantiene — Microsoft la gestiona de forma transparente.

Cuando se crea un agente en Copilot Studio, un flujo en Power Automate o una aplicación en Power Apps, **todo se persiste en Dataverse**.

```
Power Apps      ──┐
Power Automate  ──┤──► Dataverse  (almacén unificado del tenant)
Copilot Studio  ──┤
Power BI        ──┘
```

Dataverse almacena:

- **Tablas** con datos de negocio (equivalente a tablas relacionales)
- **Componentes** de aplicaciones: agentes, flujos, conectores, configuraciones
- **Metadatos** de todos los artefactos creados en el entorno

### ¿Qué es el Nombre del Esquema?

Cada componente registrado en Dataverse recibe un **identificador técnico único** llamado *nombre del esquema* (schema name). Se genera automáticamente al crear el componente:

```
cr7ee_DemoProductSupportAgent
 ↑        ↑
prefijo   nombre del componente
(publisher)
```

El prefijo lo define el **Publisher** asociado a la solución. Sirve para evitar colisiones entre componentes de distintos fabricantes o equipos dentro del mismo tenant.

> ⚠️ El nombre del esquema **no se puede modificar** una vez creado el componente.

---

## ¿Qué es una Solución?

Una Solución es un **contenedor lógico** que agrupa componentes relacionados de Power Platform. No duplica los componentes — los referencia y los organiza bajo un mismo contexto de proyecto.

Conceptualmente es similar a:

| Tecnología | Equivalente a una Solución |
|---|---|
| Node.js | `package.json` |
| .NET | `.csproj` |
| Java | `pom.xml` |
| Docker | `docker-compose.yml` |

Una solución puede contener:

- Agentes de Copilot Studio
- Flujos de Power Automate
- Aplicaciones de Power Apps
- Tablas y columnas de Dataverse
- Conectores personalizados
- Variables de entorno
- Roles de seguridad

---

## Regla fundamental

> **Siempre crear la solución primero. Luego crear los componentes dentro de ella.**

Es el mismo principio que en desarrollo de software: primero se crea el repositorio, después se escribe el código — nunca al revés.

---

## Por qué importa: el problema de crear fuera de una solución

Cuando un componente se crea fuera de una solución (en la *Default Solution*), queda registrado en Dataverse **sin contexto de transporte**.

```
❌ Flujo incorrecto

Crear el agente fuera de solución
        ↓
Querer moverlo a otro entorno
        ↓
No se puede exportar directamente
        ↓
Hay que recrearlo manualmente en destino
```

```
✅ Flujo correcto

Crear la solución primero
        ↓
Crear el agente DENTRO de la solución
        ↓
Todo queda vinculado y portable
        ↓
Exportar la solución como .zip
        ↓
Importar en cualquier entorno
```

---

## Cómo crear una Solución

### Desde el portal de Power Platform

1. Ir a [make.powerapps.com](https://make.powerapps.com)
2. Seleccionar el entorno correcto (esquina superior derecha)
3. En el menú lateral: **Soluciones → + Nueva solución**
4. Completar los campos:

| Campo | Descripción | Ejemplo |
|---|---|---|
| Nombre para mostrar | Nombre legible del proyecto | `Product Support Solution` |
| Nombre | Identificador sin espacios | `ProductSupportSolution` |
| Publisher | Define el prefijo del schema name | `Contoso` → prefijo `contoso_` |
| Versión | Número de versión semántica | `1.0.0.0` |

> 💡 **Tip:** Crear un Publisher personalizado desde el inicio evita el prefijo aleatorio (`cr7ee_`) que genera la Default Solution.

---

## Cuándo crear una solución propia

| Escenario | ¿Solución propia? |
|---|---|
| Demo o PoC descartable | ❌ Default Solution alcanza |
| Lab de capacitación | ❌ Default Solution alcanza |
| Proyecto de cliente real | ✅ Obligatorio |
| Trabajo en equipo | ✅ Obligatorio |
| Deploy entre entornos (Dev → Test → Prod) | ✅ Obligatorio |
| Producto distribuible a múltiples clientes | ✅ Obligatorio |
| CI/CD con Azure DevOps o GitHub Actions | ✅ Obligatorio |

---

## Casos de uso reales

### Caso 1: Empresa con múltiples entornos

```
Entorno DEV          Entorno TEST         Entorno PROD
┌─────────────┐      ┌─────────────┐      ┌─────────────┐
│ Se desarrolla│─────▶│ QA valida   │─────▶│ Usuarios    │
│ el agente   │export│ el agente   │export│ finales     │
└─────────────┘      └─────────────┘      └─────────────┘
       La solución (.zip) viaja entre entornos de forma controlada
```

### Caso 2: Consultora que entrega a cliente

El consultor construye en su propio tenant, exporta la solución como `.zip` y el cliente la importa en su tenant. Sin solución esto no es posible de forma limpia ni reproducible.

### Caso 3: Producto ISV sobre Power Platform

Una empresa independiente de software construye un agente genérico de atención al cliente, lo empaqueta como solución **managed** y lo distribuye. Los clientes instalan el paquete pero no pueden modificar el código fuente.

---

## Managed vs Unmanaged: diferencia clave

| | Unmanaged | Managed |
|---|---|---|
| **Uso típico** | Entorno de desarrollo | Entornos de test y producción |
| **Se puede editar** | ✅ Sí | ❌ No |
| **Se puede desinstalar de un golpe** | ❌ No (componente a componente) | ✅ Sí |
| **Se puede exportar** | ✅ Sí | ✅ Sí |
| **Cuándo usar** | Mientras se está construyendo | Al entregar al cliente o desplegar a producción |

---

## Resumen: reglas prácticas

1. **Crear la solución antes de crear cualquier componente**
2. **Usar un Publisher con prefijo significativo** (no el aleatorio de Default Solution)
3. **No agregar componentes existentes a una solución como parche** — lo ideal es crearlos dentro desde el inicio
4. **Trabajar en Unmanaged durante el desarrollo, distribuir en Managed**
5. **Versionar la solución** cada vez que se hace un deploy a producción

---

## Relación entre conceptos

```
Tenant de Power Platform
└── Entorno (Environment)
    └── Dataverse
        └── Solución
            ├── Agente (Copilot Studio)  → schema: contoso_NombreAgente
            ├── Flujo (Power Automate)   → schema: contoso_NombreFlujo
            └── App (Power Apps)         → schema: contoso_NombreApp
```

---

## Referencias

- [Descripción general de soluciones - Microsoft Learn](https://learn.microsoft.com/es-es/power-platform/alm/solution-concepts-alm)
- [Introducción a Dataverse - Microsoft Learn](https://learn.microsoft.com/es-es/power-apps/maker/data-platform/data-platform-intro)
- [Crear y administrar soluciones - Microsoft Learn](https://learn.microsoft.com/es-es/power-apps/maker/data-platform/create-solution)
- [ALM con Power Platform - Microsoft Learn](https://learn.microsoft.com/es-es/power-platform/alm/overview-alm)
