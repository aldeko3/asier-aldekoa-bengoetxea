# Guía de Inicialización del Proyecto Astro

Este documento registra y explica el proceso de configuración inicial para la creación del sitio web basado en **Astro**, utilizando **Node.js** y **pnpm**.

---

## 1. Selección de la Versión de Node.js

El proceso comenzó estableciendo la versión del entorno de ejecución mediante `nvm` (Node Version Manager):

```bash
nvm use 24.22.0
```

* **Resultado**: Se activó **Node.js v24.22.0** junto con el gestor de paquetes **npm v11.19.1**.
* **Motivo**: Asegurar un entorno de ejecución moderno y compatible con las últimas características de Astro.

---

## 2. Creación e Inicialización del Proyecto

Se ejecutó el comando interactivo CLI oficial de Astro especificando la plantilla base:

```bash
pnpm create astro@latest -- --template basics
```

### Opciones de Configuración Seleccionadas:
1. **Directorio del Proyecto (`dir`)**: `./` (Directorio actual).
2. **Plantilla (`tmpl`)**: `basics` (Estructura inicial limpia y mínima).
3. **Instalación de Dependencias (`deps`)**: `Yes` (Instalación automática mediante `pnpm`).
4. **Control de Versiones (`git`)**: Inicializado correctamente.

---

## 3. Resultado del Proceso

El CLI (`create-astro 5.3.0`) completó las siguientes tareas:
* Copia y estructuración de archivos desde la plantilla base.
* Descarga e instalación de dependencias en la tienda virtual de `pnpm`.
* Configuración del repositorio Git local.

---

## 4. Pasos Siguientes

Para iniciar el servidor de desarrollo local y empezar a trabajar en el proyecto:

```bash
# Iniciar el servidor de desarrollo
pnpm dev
```

El servidor estará accesible por defecto en `http://localhost:4321`.

### Integraciones recomendadas
Para añadir soporte para frameworks o utilidades CSS adicionales, se pueden usar las integraciones automáticas de Astro:

```bash
# Añadir Tailwind CSS
pnpm astro add tailwind

# Añadir React
pnpm astro add react
```