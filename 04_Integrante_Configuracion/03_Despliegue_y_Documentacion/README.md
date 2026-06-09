# Guía de Despliegue — Algorithmix (Silabo)

Aplicación web educativa desarrollada en Django para el aprendizaje de algoritmos y lógica de programación.

## Stack Tecnológico

- **Backend:** Django 6.0.3
- **Base de datos:** SQLite 3
- **Frontend:** HTML5, CSS3, JavaScript vanilla
- **Hosting:** PythonAnywhere (plan gratuito)
- **Lenguaje:** Python 3.13

## Requisitos

- Python 3.13 o superior
- pip
- Git

## Instalación local

```bash
# 1. Clonar el repositorio
git clone https://github.com/Edison206/algorithmix.git
cd algorithmix

# 2. Crear entorno virtual
python -m venv venv

# 3. Activar entorno virtual
# Windows:
venv\Scripts\activate
# Linux/Mac:
source venv/bin/activate

# 4. Instalar dependencias
pip install -r requirements.txt

# 5. Aplicar migraciones
python manage.py migrate

# 6. Crear superusuario (opcional)
python manage.py createsuperuser

# 7. Ejecutar servidor de desarrollo
python manage.py runserver
```

La aplicación estará disponible en `http://127.0.0.1:8000/`.

## Despliegue en PythonAnywhere

### 1. Subir el código
```bash
cd ~
git clone https://github.com/Edison206/algorithmix.git
```

### 2. Crear el entorno virtual
```bash
mkvirtualenv silabo_env --python=python3.13
pip install -r requirements.txt
```

### 3. Configurar la Web App
- En el panel **Web** de PythonAnywhere, crear una nueva web app con configuración manual.
- Python 3.13
- Source code: `/home/<usuario>/algorithmix`
- Working directory: `/home/<usuario>/algorithmix`
- Virtualenv: `/home/<usuario>/.virtualenvs/silabo_env`

### 4. Editar el archivo WSGI
Reemplazar el contenido por:
```python
import os, sys
path = '/home/<usuario>/algorithmix'
if path not in sys.path:
    sys.path.insert(0, path)
os.environ['DJANGO_SETTINGS_MODULE'] = 'Silabo.settings'
from django.core.wsgi import get_wsgi_application
application = get_wsgi_application()
```

### 5. Configurar archivos estáticos
En la sección **Static Files**:
- URL: `/static/` → Directory: `/home/<usuario>/algorithmix/static`
- URL: `/media/` → Directory: `/home/<usuario>/algorithmix/media`

### 6. Reload
Pulsar el botón **Reload** verde en el panel Web.

## Estructura del proyecto

```
algorithmix/
├── Silabo/                  # Configuración del proyecto Django
│   ├── settings.py
│   ├── urls.py
│   ├── asgi.py
│   └── wsgi.py
├── estudiantes/             # Aplicación principal
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│   ├── forms.py
│   ├── admin.py
│   ├── reportes.py
│   ├── utils.py
│   ├── migrations/
│   └── templates/
├── static/                  # CSS y JavaScript
│   ├── css/
│   └── js/
├── media/                   # PDFs de APEs (no en git)
├── db.sqlite3              # Base de datos (no en git)
├── manage.py
└── requirements.txt
```

## Autores

- **Edison Landeta** — Modelos de base de datos y vistas
- **Integrante 2** — Plantillas HTML
- **Integrante 3** — Estilos CSS y JavaScript
- **Integrante 4** — Configuración Django y despliegue
- **Integrante 5** — Sistema de reportes PDF, migraciones y contenido

Universidad Técnica de Ambato — FISEI — Carrera de Software
Algoritmos y Lógica de Programación — Ciclo Enero - Julio 2026
