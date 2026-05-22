# 🌐 Power Apps: Environment vs Solution

> Guía conceptual para entender la diferencia entre estos dos pilares del ecosistema Power Platform.

---

## 📦 ¿Qué es un Environment?

Un **Environment** es un **contenedor de infraestructura aislado**. Funciona como un servidor independiente con su propia base de datos, usuarios y configuración.

### Características clave

- Tiene su propia instancia de **Dataverse**
- Tiene sus propios **usuarios y roles de seguridad**
- Tiene sus propias **conexiones y conectores**
- Está **totalmente aislado** de otros environments

### Environments típicos en una organización

| Environment | Propósito |
|---|---|
| `Development` | Construcción y prueba inicial |
| `Test / UAT` | Validación con usuarios |
| `Production` | Versión en uso real |

> ⚠️ Lo que hacés en **Dev** no afecta **Prod**. Son mundos separados.

---

## 🗃️ ¿Qué es una Solution?

Una **Solution** es un **paquete lógico de componentes** que vive *dentro* de un environment. No es infraestructura: es organización y portabilidad.

### ¿Qué puede contener?

- 📱 Apps (Canvas y Model-driven)
- ⚡ Flows de Power Automate
- 🗄️ Tablas de Dataverse
- 🔧 Variables de entorno
- 🔌 Conectores personalizados

### Tipos de Solution

| Tipo | Descripción |
|---|---|
| **Unmanaged** | Editable. Se usa en entornos de desarrollo. |
| **Managed** | Solo lectura. Se despliega en Test y Producción. |

---

## 🔄 La relación entre ambos

La **Solution viaja entre Environments**. El environment es el *lugar*; la solution es la *valija*.

```
ENVIRONMENT: Development
└── Solution "MiApp v1.0"  (unmanaged)
    ├── Canvas App
    ├── Flow de aprobación
    └── Tabla Dataverse

        ⬇  export (.zip)  /  import

ENVIRONMENT: Production
└── Solution "MiApp v1.0"  (managed)
    ├── Canvas App
    ├── Flow de aprobación
    └── Tabla Dataverse
```

---

## ⚖️ Comparativa rápida

| | Environment | Solution |
|---|---|---|
| **¿Qué es?** | Infraestructura aislada | Paquete de componentes |
| **¿Cuántos hay?** | Pocos (Dev / Test / Prod) | Muchos (uno por proyecto) |
| **¿Para qué sirve?** | Aislar entornos | Organizar y transportar |
| **¿Se puede exportar?** | ❌ No | ✅ Sí (.zip) |
| **¿Tiene Dataverse propio?** | ✅ Sí | ❌ No |

---

## ✅ Buenas prácticas

1. **Siempre trabajá dentro de una Solution** — nunca en el Default. Facilita el transporte y el control de cambios.
2. **Usá variables de entorno** dentro de la solution para manejar configuraciones que cambian entre Dev y Prod (URLs, credenciales, etc.).
3. **Exportá como Managed** al desplegar en Producción — evita modificaciones accidentales.
4. **Un proyecto = una solution** — mantené el scope acotado.

---

## 🧠 Resumen en una línea

> El **Environment** es *donde viven* tus apps.  
> La **Solution** es *cómo las empaquetás y movés* de un environment a otro.

---

*Documentación elaborada para capacitaciones de Power Platform — Microsoft Power Apps*
