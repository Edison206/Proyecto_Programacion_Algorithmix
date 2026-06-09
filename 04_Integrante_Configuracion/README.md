# 👤 Integrante 4 — Configuración Django y Despliegue

## Responsabilidad

Configurar la **arquitectura del proyecto Django** y preparar todo lo necesario para que la aplicación se pueda desplegar en producción (PythonAnywhere). Este es un rol de **DevOps / infraestructura**.

---

## 📦 Tus 3 Commits

### 🔹 Commit 1 — Configuración base del proyecto Django

**Carpeta:** `Commit_1_Setup_Django/`

**Archivos:**
- `settings.py` (139 líneas) — Configuración principal del proyecto Django (apps instaladas, middleware, BD, ALLOWED_HOSTS, STATIC_ROOT, etc.).
- `urls_PROYECTO_RAIZ.py` (28 líneas) — URLs raíz del proyecto Django (renombrar a `urls.py` al copiar).
- `wsgi.py` (16 líneas) — Punto de entrada WSGI para servidores de producción.
- `asgi.py` (16 líneas) — Punto de entrada ASGI para servidores asíncronos.
- `manage.py` — Script de gestión de Django.

**Dónde copiarlos en el proyecto:**
- `settings.py`, `urls.py` (renombrado), `wsgi.py`, `asgi.py` → `algorithmix/Silabo/`
- `manage.py` → `algorithmix/` (raíz)

**Mensaje del commit (copiar y pegar):**
```
Add: configuracion inicial del proyecto Django (settings, urls raiz, wsgi, asgi)
```

---

### 🔹 Commit 2 — URLs de la app, formularios y panel admin

**Carpeta:** `Commit_2_URLs_Forms_Admin/`

**Archivos:**
- `urls_APP.py` (15 líneas) — URLs específicas de la aplicación `estudiantes` (renombrar a `urls.py` al copiar).
- `forms.py` (37 líneas) — Formularios de registro y login con validación.
- `admin.py` (9 líneas) — Configuración del panel de administración de Django.
- `apps.py` (5 líneas) — Configuración de la aplicación `estudiantes`.

**Dónde copiarlos en el proyecto:**
```
algorithmix/estudiantes/
```
(`urls_APP.py` se renombra a `urls.py`)

**Mensaje del commit (copiar y pegar):**
```
Add: URLs de la app estudiantes, formularios y configuracion del admin
```

---

### 🔹 Commit 3 — Despliegue: requirements, gitignore y documentación

**Carpeta:** `Commit_3_Despliegue/`

**Archivos:**
- `requirements.txt` — Lista de dependencias Python del proyecto.
- `.gitignore` — Archivos y carpetas que Git debe ignorar (BD local, cache, etc.).
- `README.md` — Documentación completa del proyecto (instalación, despliegue en PythonAnywhere, estructura).

**Dónde copiarlos en el proyecto:**
```
algorithmix/    (raíz del proyecto)
```

**Mensaje del commit (copiar y pegar):**
```
Add: dependencias, gitignore y documentacion completa de despliegue
```

---

## 🔧 Flujo de trabajo recomendado

### Para CADA commit, sigue estos pasos:

```bash
# 1. Asegúrate de estar en la carpeta del proyecto
cd algorithmix

# 2. Baja los últimos cambios
git pull

# 3. Configura tu identidad de Git (solo la primera vez)
git config user.name "Tu Nombre Apellido"
git config user.email "tu_correo_de_github@ejemplo.com"

# 4. Copia los archivos a sus rutas correspondientes
#    (ver "Dónde copiarlos" en cada commit)

# 5. Verifica los cambios
git status

# 6. Agrega y haz el commit
git add .
git commit -m "Add: configuracion inicial del proyecto Django (settings, urls raiz, wsgi, asgi)"

# 7. Sube al repositorio remoto
git push
```

---

## 📅 Coordinación con otros integrantes

Tu trabajo es la **base de toda la arquitectura**, así que tus dos primeros commits van temprano en el cronograma:

- Tu **Commit 1** (Setup Django) va DESPUÉS de que Edison suba su parte inicial.
- Tu **Commit 2** (URLs + Forms + Admin) va INMEDIATAMENTE después.
- Tu **Commit 3** (Despliegue) va al FINAL, cuando todos los demás ya hayan terminado.

⚠️ **Antes de cada commit:** ejecuta `git pull` para no pisar cambios de otros compañeros.

---

## 📝 Resumen visual

| Commit | Archivos | Líneas totales | Mensaje |
|--------|----------|----------------|---------|
| 1 | settings.py + urls.py raíz + wsgi.py + asgi.py + manage.py | ~199 | `Add: configuracion inicial del proyecto Django (settings, urls raiz, wsgi, asgi)` |
| 2 | urls.py app + forms.py + admin.py + apps.py | ~66 | `Add: URLs de la app estudiantes, formularios y configuracion del admin` |
| 3 | requirements.txt + .gitignore + README.md | documentación | `Add: dependencias, gitignore y documentacion completa de despliegue` |

---

## ⚠️ Notas importantes

1. **El archivo `urls_PROYECTO_RAIZ.py` debe renombrarse a `urls.py`** al copiarlo al proyecto. Lo nombré así para evitar confusión con el `urls.py` de la app.

2. **El archivo `urls_APP.py` debe renombrarse a `urls.py`** al copiarlo a la carpeta `estudiantes/`.

3. **El archivo `settings.py`** tiene configuraciones de producción para PythonAnywhere (`ALLOWED_HOSTS`, `STATIC_ROOT`). No modifiques esos valores sin coordinarlo con Edison.
