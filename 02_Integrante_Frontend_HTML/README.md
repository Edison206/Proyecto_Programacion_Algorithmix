# 👤 Integrante 2 — Frontend / Plantillas HTML

## Responsabilidad

Desarrollar las **6 plantillas HTML** que conforman la interfaz de usuario de la aplicación. Estas plantillas se conectan con las vistas de Django y muestran los datos al estudiante.

---

## 📦 Tus 3 Commits

### 🔹 Commit 1 — Plantillas de autenticación

**Carpeta:** `Commit_1_Auth/`

**Archivos:**
- `login.html` (39 líneas) — Formulario de inicio de sesión.
- `registro.html` (70 líneas) — Formulario de registro de nuevos estudiantes.

**Dónde copiarlos en el proyecto:**
```
algorithmix/estudiantes/templates/estudiantes/
```

**Mensaje del commit (copiar y pegar):**
```
Add: plantillas HTML de autenticacion (login y registro)
```

---

### 🔹 Commit 2 — Plantillas de navegación

**Carpeta:** `Commit_2_Navegacion/`

**Archivos:**
- `temas.html` (89 líneas) — Vista principal con el menú lateral de temas agrupados por unidad.
- `ejercicios.html` (135 líneas) — Listado de ejercicios dentro de un tema.

**Dónde copiarlos en el proyecto:**
```
algorithmix/estudiantes/templates/estudiantes/
```

**Mensaje del commit (copiar y pegar):**
```
Add: plantillas HTML de navegacion (temas y listado de ejercicios)
```

---

### 🔹 Commit 3 — Plantillas de interacción con ejercicios

**Carpeta:** `Commit_3_Interaccion/`

**Archivos:**
- `ejercicio_resolver.html` (139 líneas) — Vista para resolver un ejercicio (incluye editor de respuesta).
- `ejercicio_aprender.html` (97 líneas) — Vista de modo "aprender" con código de ejemplo en C++, Python y Java.

**Dónde copiarlos en el proyecto:**
```
algorithmix/estudiantes/templates/estudiantes/
```

**Mensaje del commit (copiar y pegar):**
```
Add: plantillas HTML de interaccion con ejercicios (resolver y aprender)
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

# 4. Copia los archivos del commit correspondiente
#    Por ejemplo, para Commit 1:
#    De:  02_Integrante_Frontend_HTML/Commit_1_Auth/
#    A:   algorithmix/estudiantes/templates/estudiantes/

# 5. Verifica los cambios
git status

# 6. Agrega y haz el commit
git add .
git commit -m "Add: plantillas HTML de autenticacion (login y registro)"

# 7. Sube al repositorio remoto
git push
```

---

## 📅 Coordinación con otros integrantes

Para evitar conflictos, sigue este **orden recomendado** dentro del flujo general del proyecto:

- Tu **Commit 1** va DESPUÉS de que el Integrante 4 termine su Commit 2 (URLs, Forms, Admin).
- Tu **Commit 2** va DESPUÉS de que el Integrante 3 haga su Commit 1 (Estilos de Auth).
- Tu **Commit 3** va DESPUÉS de que el Integrante 3 haga su Commit 2 (Estilos de Navegación).

⚠️ **Antes de cada commit:** ejecuta `git pull` para no pisar cambios de otros compañeros.

---

## 📝 Resumen visual

| Commit | Archivos | Líneas totales | Mensaje |
|--------|----------|----------------|---------|
| 1 | login.html + registro.html | 109 | `Add: plantillas HTML de autenticacion (login y registro)` |
| 2 | temas.html + ejercicios.html | 224 | `Add: plantillas HTML de navegacion (temas y listado de ejercicios)` |
| 3 | ejercicio_resolver.html + ejercicio_aprender.html | 236 | `Add: plantillas HTML de interaccion con ejercicios (resolver y aprender)` |
