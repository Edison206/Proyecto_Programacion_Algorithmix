# 👤 Edison Landeta — Base de Datos y Vistas

## Responsabilidad

Edison Landeta es el responsable del corazón del backend de la aplicación:

- **`models.py`** — Definición de modelos de base de datos (Usuario, Tema, Ejercicio, Intento, Retroalimentacion, Aprender)
- **`views.py`** — Lógica de las vistas (login, registro, listado de temas, ejercicios, resolver, aprender, cerrar sesión, descargar reporte)
- **`utils.py`** — Función auxiliar `obtener_temas_por_unidad()` para agrupar y contar ejercicios por unidad

## Archivos en esta carpeta

```
01_Edison_Landeta_BD_Vistas/
├── models.py     (97 líneas)
├── views.py      (190 líneas)
└── utils.py      (30 líneas)
```

## Commits realizados (referencia)

Edison ya tiene commits anteriores en el repositorio que cubren:

- Diseño de los modelos de base de datos.
- Implementación de las vistas y la lógica del backend.
- Definición de la función `obtener_temas_por_unidad` con filtrado por usuario.
- Corrección del bug de privacidad entre usuarios usando `Prefetch` y `Count` con `Q`.

## Nota

Esta carpeta sirve únicamente como **referencia** del trabajo de Edison para que los demás integrantes entiendan la estructura del backend al desarrollar las plantillas, estilos y configuración.
