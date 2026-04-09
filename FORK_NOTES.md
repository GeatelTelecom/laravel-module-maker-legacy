# GeatelTelecom Internal Install — Laravel Module Maker (Legacy)

## Origen

Este repositorio es una **instalación interna legacy** de `innodite/laravel-module-maker`, mantenida por GeatelTelecom.

- **Upstream original:** https://github.com/Innodite/laravel-module-maker
- **Versión base:** `v2.0.0` (tag del 2025-03-28)
- **Método de instalación:** descarga directa del ZIP del tag v2.0.0 (sin historial git del upstream)
- **Fecha de instalación:** 2026-04-09
- **Instalado por:** GeatelTelecom

## Motivo

Se preserva la versión v2.0.0 como referencia y soporte para:

- Proyectos que operan con esta versión y no pueden migrar inmediatamente a v3.5.6
- Auditoría y comparación evolutiva del paquete
- Rollback de emergencia si la versión moderna presenta incompatibilidades

## Cambios respecto al upstream

- `composer.json`: nombre del paquete renombrado a `geateltelecom/laravel-module-maker-legacy`.
- `composer.json`: añadido GeatelTelecom como mantenedor interno.
- **Namespace PHP intacto:** `Innodite\LaravelModuleMaker\*` se mantiene para compatibilidad.
- Nuevo archivo `FORK_NOTES.md` (este archivo).

## Política de mantenimiento

- **Congelado** en v2.0.0. No se aplicarán parches ni actualizaciones.
- Para nuevos proyectos, usar `geateltelecom/laravel-module-maker` (v3.5.6+).

## Uso en proyectos consumidores

```json
{
    "repositories": [
        {
            "type": "vcs",
            "url": "https://github.com/GeatelTelecom/laravel-module-maker-legacy.git"
        }
    ],
    "require": {
        "geateltelecom/laravel-module-maker-legacy": "v2.0.0"
    }
}
```

```bash
composer remove innodite/laravel-module-maker
composer require geateltelecom/laravel-module-maker-legacy:v2.0.0
```

## Repositorio moderno

Para la versión actual mantenida (v3.5.6), ver:
https://github.com/GeatelTelecom/laravel-module-maker
