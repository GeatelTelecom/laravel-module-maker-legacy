# GeatelTelecom Internal Install — Laravel Module Maker (Legacy)

## Origen

Este repositorio es una **instalación interna legacy** de `innodite/laravel-module-maker`, mantenida por GeatelTelecom como referencia histórica.

- **Upstream original:** https://github.com/Innodite/laravel-module-maker
- **Versión base:** `v1.0.1` (tag del 2025-08-07)
- **Método de instalación:** descarga directa del ZIP del tag v1.0.1 (sin historial git del upstream)
- **Fecha de instalación:** 2026-04-09
- **Instalado por:** GeatelTelecom

## Motivo

Se preserva la versión legacy v1.0.1 como referencia para:

- Proyectos que aún operan con esta versión y no pueden migrar inmediatamente a v3.5.6
- Auditoría y comparación evolutiva del paquete
- Rollback de emergencia si la versión moderna presenta incompatibilidades

## Diferencias con la versión moderna (v3.5.6)

La v1.0.1 es significativamente más simple:

- **Sin sistema de contextos** (Central/Shared/Tenant no existía)
- **Sin multi-tenancy** — generador de módulos básico
- **Sin middleware** (InnoditeContextBridge no existía)
- **Sin composables Vue 3** ni integración frontend
- **Soporte Laravel:** ^10.0|^11.0|^12.0 (vs ^11.0|^12.0 en v3.5.6)
- **Sin dependencias dev** (sin pest, testbench, phpcs)

## Cambios respecto al upstream

- `composer.json`: nombre del paquete renombrado a `geateltelecom/laravel-module-maker-legacy`.
- `composer.json`: añadido GeatelTelecom como mantenedor interno.
- **Namespace PHP intacto:** `Innodite\LaravelModuleMaker\*` se mantiene para compatibilidad.
- Nuevo archivo `FORK_NOTES.md` (este archivo).

## Política de mantenimiento

- **Congelado permanentemente** en v1.0.1. No se aplicarán parches ni actualizaciones.
- Para nuevos proyectos, usar `geateltelecom/laravel-module-maker` (v3.5.6+).
- Este repositorio existe solo como referencia y soporte a proyectos legacy.

## Uso en proyectos consumidores (solo legacy)

```json
{
    "repositories": [
        {
            "type": "vcs",
            "url": "https://github.com/GeatelTelecom/laravel-module-maker-legacy.git"
        }
    ],
    "require": {
        "geateltelecom/laravel-module-maker-legacy": "v1.0.1"
    }
}
```

```bash
composer remove innodite/laravel-module-maker
composer require geateltelecom/laravel-module-maker-legacy:v1.0.1
```

## Repositorio moderno

Para la versión actual mantenida (v3.5.6), ver:
https://github.com/GeatelTelecom/laravel-module-maker
