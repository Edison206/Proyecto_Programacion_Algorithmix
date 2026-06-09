# 👤 Integrante 3 — Estilos visuales (CSS + JavaScript)

## Responsabilidad

Desarrollar **todo el diseño visual** de la aplicación: hojas de estilo CSS y scripts JavaScript que dan vida e interactividad a la interfaz. El tema visual usa **estilo oscuro tipo GitHub** (fondo `#0d1117`).

---

## 📦 Tus 3 Commits

### 🔹 Commit 1 — Estilos y JS de autenticación

**Carpeta:** `Commit_1_Auth/`

**Archivos:**
- `loginestilo.css` (75 líneas) — Estilos del formulario de login y registro.
- `login.js` (23 líneas) — Lógica de envío y validación del formulario de login.

**Dónde copiarlos en el proyecto:**
- `loginestilo.css` → `algorithmix/static/css/`
- `login.js` → `algorithmix/static/js/`

**Mensaje del commit (copiar y pegar):**
```
Add: estilos CSS y JS para pantallas de autenticacion
```

---

### 🔹 Commit 2 — Estilos y JS de navegación principal

**Carpeta:** `Commit_2_Navegacion/`

**Archivos:**
- `temasestilo.css` (217 líneas) — Estilos del menú lateral, tarjetas de temas, agrupación por unidad.
- `temas.js` (2 líneas) — Script de inicialización del menú lateral.

**Dónde copiarlos en el proyecto:**
- `temasestilo.css` → `algorithmix/static/css/`
- `temas.js` → `algorithmix/static/js/`

**Mensaje del commit (copiar y pegar):**
```
Add: estilos CSS y JS para pantalla principal de temas
```

---

### 🔹 Commit 3 — Estilos y JS de la sección de ejercicios

**Carpeta:** `Commit_3_Ejercicios/`

**Archivos:**
- `ejercicios.css` (294 líneas) — Estilos de las tarjetas de ejercicios, badges de dificultad y categorías.
- `ejercicioresolverestilo.css` (358 líneas) — Estilos del editor de código, bloques de enunciado y retroalimentación.
- `respuesta.js` (87 líneas) — Lógica para enviar respuestas de ejercicios al backend vía AJAX.

**Dónde copiarlos en el proyecto:**
- Los dos `.css` → `algorithmix/static/css/`
- `respuesta.js` → `algorithmix/static/js/`

**Mensaje del commit (copiar y pegar):**
```
Add: estilos CSS y JS para vistas de listado y resolucion de ejercicios
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

# 4. Copia los archivos del commit correspondiente a sus carpetas
#    Por ejemplo, para Commit 1:
#    - loginestilo.css va a → algorithmix/static/css/
#    - login.js va a → algorithmix/static/js/

# 5. Verifica los cambios
git status

# 6. Agrega y haz el commit
git add .
git commit -m "Add: estilos CSS y JS para pantallas de autenticacion"

# 7. Sube al repositorio remoto
git push
```

---

## 📅 Coordinación con otros integrantes

Para que tus estilos tengan sentido visual, deben aplicarse a plantillas que ya existan. Por eso el orden recomendado es:

- Tu **Commit 1** (Auth) va DESPUÉS del Commit 1 del Integrante 2 (login.html y registro.html).
- Tu **Commit 2** (Navegación) va DESPUÉS del Commit 2 del Integrante 2 (temas.html y ejercicios.html).
- Tu **Commit 3** (Ejercicios) va DESPUÉS del Commit 3 del Integrante 2 (ejercicio_resolver.html y ejercicio_aprender.html).

⚠️ **Antes de cada commit:** ejecuta `git pull` para no pisar cambios de otros compañeros.

---

## 📝 Resumen visual

| Commit | Archivos | Líneas totales | Mensaje |
|--------|----------|----------------|---------|
| 1 | loginestilo.css + login.js | 98 | `Add: estilos CSS y JS para pantallas de autenticacion` |
| 2 | temasestilo.css + temas.js | 219 | `Add: estilos CSS y JS para pantalla principal de temas` |
| 3 | ejercicios.css + ejercicioresolverestilo.css + respuesta.js | 739 | `Add: estilos CSS y JS para vistas de listado y resolucion de ejercicios` |

---

## 🎨 Paleta de colores del proyecto

Para mantener consistencia visual con el resto del equipo:

- **Fondo principal:** `#0d1117` (negro estilo GitHub)
- **Color de acento:** `#2f81f7` (azul)
- **Color secundario:** `#7c3aed` (violeta)
- **Éxito:** `#238636` (verde)
- **Error:** `#da3633` (rojo)
- **Gris texto:** `#8b949e`
