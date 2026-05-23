# MiRancho
### Sistema de gestión ganadera para el campo mexicano

---

## ¿Qué es MiRancho?

MiRancho es una aplicación web para ranchos ganaderos. Funciona desde el celular, sin necesidad de instalar nada, y opera aunque no haya internet en el campo.

Incluye más de 30 módulos: ganado, vacunas, finanzas, potreros, mapa satelital, asistente con inteligencia artificial, y más.

---

## Archivos del proyecto

| Archivo | Descripción |
|---------|-------------|
| `index.html` | Página de presentación para clientes |
| `MiRancho.html` | La aplicación completa |
| `README.md` | Este archivo |

---

## Cómo publicar en GitHub Pages (paso a paso)

### Paso 1 — Crear cuenta en GitHub
1. Ve a [github.com](https://github.com)
2. Clic en **Sign up**
3. Elige un nombre de usuario (ej: `mirancho-mx`)
4. Completa el registro

### Paso 2 — Crear el repositorio
1. Una vez dentro, clic en el botón verde **New** (o el `+` arriba a la derecha)
2. En **Repository name** escribe: `mirancho`
3. Selecciona **Public**
4. Clic en **Create repository**

### Paso 3 — Subir los archivos
1. En la página del repositorio, clic en **uploading an existing file**
2. Arrastra los tres archivos: `index.html`, `MiRancho.html`, `README.md`
3. En la parte de abajo escribe un mensaje como `Primera versión`
4. Clic en **Commit changes**

### Paso 4 — Activar GitHub Pages
1. Ve a la pestaña **Settings** del repositorio
2. En el menú izquierdo busca **Pages**
3. En **Source** selecciona **Deploy from a branch**
4. En **Branch** selecciona **main** y la carpeta **/ (root)**
5. Clic en **Save**
6. Espera 2-3 minutos

### Paso 5 — Tu URL está lista
Después de unos minutos, GitHub te muestra la URL:
```
https://tunombre.github.io/mirancho
```

Esa URL es la que compartes con tus clientes.

---

## Cómo agregar un dominio propio (opcional)

Si quieres que quede en `mirancho.mx` en lugar de `tunombre.github.io/mirancho`:

### 1. Comprar el dominio
- [namecheap.com](https://namecheap.com) — recomendado, ~$12 USD/año para `.com`
- [godaddy.com](https://godaddy.com) — alternativa conocida
- [akky.mx](https://akky.mx) — para dominios `.mx`, administrado por NIC México

### 2. Apuntar el dominio a GitHub
En el panel de tu proveedor de dominio, agrega estos registros DNS:

**Registros A** (para el dominio raíz `mirancho.mx`):
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

**Registro CNAME** (para `www.mirancho.mx`):
```
www  →  tunombre.github.io
```

### 3. Configurar en GitHub Pages
1. En Settings → Pages, busca **Custom domain**
2. Escribe tu dominio: `mirancho.mx`
3. Clic en Save
4. Activa **Enforce HTTPS** (aparece después de unos minutos)

Los cambios de DNS tardan entre 30 minutos y 24 horas en propagarse.

---

## Cómo actualizar la app

Cuando hagas cambios a `MiRancho.html`:

1. Ve al repositorio en GitHub
2. Clic en el archivo `MiRancho.html`
3. Clic en el ícono de lápiz (✏ Edit)
4. Pega el nuevo contenido (o usa **Upload files** para reemplazar el archivo)
5. Clic en **Commit changes**

Los clientes verán la versión nueva automáticamente la próxima vez que abran la URL.

---

## Cómo instalar la app en el celular (para tus clientes)

Comparte esta instrucción con cada rancho:

**Android (Chrome):**
1. Abre la URL de MiRancho en Chrome
2. Toca el menú ⋮ (tres puntos arriba a la derecha)
3. Toca **"Instalar app"** o **"Agregar a pantalla de inicio"**
4. Confirma tocando **Instalar**

**iPhone (Safari):**
1. Abre la URL en Safari (no en Chrome)
2. Toca el botón compartir (cuadrado con flecha hacia arriba)
3. Baja hasta encontrar **"Agregar a pantalla de inicio"**
4. Toca **Agregar**

Una vez instalada, el ícono aparece en la pantalla principal del celular como cualquier otra app.

---

## Contraseñas iniciales

Cada rancho configura sus propias contraseñas la primera vez que abre la app. El Patrón puede cambiarlas desde **Configuración → Control de acceso**.

Si un cliente olvida su contraseña, la solución es borrar los datos del navegador y volver a configurar la app desde cero. En una versión futura se agregará recuperación de contraseña por teléfono.

---

## Módulos incluidos

Ganado · Ficha por animal · Genealogía · Vacunas · Alertas · Tratamientos · Pesos · Leche · Partos · Finanzas · Escaneo de notas con IA · Insumos · Escaneo de productos con IA · Personal · Potreros · Mapa satelital · Rotación de potreros · Salud del suelo · Lluvia · Clima automático · Tareas del día · Roles de acceso · Costo por animal · Reportes · Comparativo anual · Presupuesto · Calendario · Galería de fotos · Asistente IA por voz · Proyecciones · Exportar a Excel · Reporte PDF · Notificaciones · Historial de cambios · Modo sin internet

---

## Tecnologías utilizadas

- HTML5 + CSS3 + JavaScript puro (sin frameworks)
- [Claude API](https://anthropic.com) — Asistente IA, escaneo de aretes, notas y productos
- [Leaflet.js](https://leafletjs.com) + ESRI — Mapa satelital
- [Open-Meteo](https://open-meteo.com) — Datos de lluvia automáticos
- Web Speech API — Reconocimiento y síntesis de voz
- Service Worker — Modo sin internet (PWA)

---

## Próximas versiones

- [ ] Base de datos en la nube (Supabase) — datos seguros aunque se borre el celular
- [ ] Login con número de teléfono
- [ ] Sistema de suscripción mensual
- [ ] Notificaciones por WhatsApp
- [ ] Pesaje masivo de animales
- [ ] Lotes y grupos de animales

---

## Contacto

Para soporte, reportar errores o solicitar funciones nuevas:
- Email: contacto@mirancho.mx
- WhatsApp: (993) xxx-xxxx

---

*MiRancho — Hecho en Tabasco, México*
