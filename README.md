# 📦 Laravel Module Maker

Genera módulos y componentes para Laravel de forma rápida, limpia y estructurada, siguiendo buenas prácticas de desarrollo.

## 🚀 Instalación

### 1. Instala el paquete vía Composer

```
composer require innodite/laravel-module-maker
```

### 2. Configura el paquete y publica los stubs

* Después de la instalación, es crucial ejecutar el comando de configuración del paquete. 
* Esto publicará los archivos de configuración de ejemplo y los "stubs" (plantillas) que el paquete utiliza para generar los diferentes componentes. 
* Publicar los stubs te permite personalizarlos si deseas modificar la estructura o el contenido por defecto de los archivos generados.

Ejecuta el siguiente comando:

```
php artisan innodite:module-setup
```

- Modificar el composer.json y agregar esta linea 

`"autoload": {
        "psr-4": {
            "Modules\\": "Modules/"
        }
    },`
Visita la documentacion para que visualices toda la pontencialidad del paquete!!!.

### [Documentacion](https://github.com/Innodite/laravel-module-maker/wiki)

Laravel Module Maker acelera tu desarrollo y mantiene tu código modular, limpio y profesional. ¡A crear sin límites!


