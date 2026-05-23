# MiRancho
### Sistema de gestión ganadera para el campo mexicano

---

## Archivos del proyecto

| Archivo | Descripción |
|---------|-------------|
| `index.html` | Página de presentación — la ven los clientes antes de entrar |
| `MiRancho.html` | La aplicación completa |
| `README.md` | Este archivo |

La URL de la app queda así:
- Página principal: `tunombre.github.io/mirancho`
- App directa: `tunombre.github.io/mirancho/MiRancho.html`

---

## Cómo actualizar la app

Cuando haya una versión nueva de `MiRancho.html`:

1. Ve al repositorio en GitHub
2. Clic en el archivo `MiRancho.html`
3. Clic en el ícono de lápiz ✏ (arriba a la derecha)
4. Selecciona **Upload files** para reemplazar el archivo
5. Clic en **Commit changes**

Todos los clientes ven la versión nueva automáticamente la próxima vez que abran la app.

---

## Cómo actualizar la página de presentación

Mismo proceso que arriba pero con `index.html`.

Cosas que puedes cambiar fácilmente:
- El correo de contacto (busca `contacto@mirancho.mx`)
- El número de WhatsApp
- Los precios si decides cobrar
- La lista de módulos

---

## Cómo agregar un dominio propio

Si quieres que quede en `mirancho.mx` en lugar de `tunombre.github.io/mirancho`:

### 1. Compra el dominio
- [namecheap.com](https://namecheap.com) — recomendado (~$12 USD/año para `.com`)
- [akky.mx](https://akky.mx) — para `.mx`, administrado por NIC México

### 2. Agrega estos registros DNS en tu proveedor

**Registros tipo A** (dominio raíz):
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

**Registro tipo CNAME** (para www):
```
www  →  tunombre.github.io
```

### 3. Configura en GitHub Pages
- Settings → Pages → Custom domain → escribe `mirancho.mx` → Save
- Activa **Enforce HTTPS**

Los cambios DNS tardan entre 30 minutos y 24 horas.

---

## Qué hacer si un cliente pierde su contraseña

Las contraseñas viven en el navegador del cliente. No hay recuperación remota en esta versión.

**Solución:**
1. El cliente abre la app en su celular
2. Va a Configuración del navegador → Borrar datos del sitio
3. Recarga la app — aparece el setup de primer uso
4. Configura de nuevo con nuevas contraseñas

> ⚠️ Al borrar los datos del navegador también se borran los datos del rancho si no están sincronizados con la nube. Avisar al cliente antes.

---

## Datos de los clientes

En esta versión los datos viven en el navegador del cliente (`localStorage` / `window.storage`). Esto significa:

- ✅ No hay servidor que mantener
- ✅ Cero costo de infraestructura
- ⚠️ Si el cliente borra el caché, pierde los datos
- ⚠️ Los datos no se comparten entre dispositivos

**Recomendación para clientes:** usar siempre el mismo celular y no borrar datos del navegador.

---

## Módulos incluidos (v1.0)

Ganado · Ficha por animal · Genealogía · Vacunas · Alertas · Tratamientos · Pesos · Leche · Partos · Finanzas · Escaneo de notas con IA · Insumos · Escaneo de productos con IA · Personal · Potreros · Mapa satelital · Rotación · Salud del suelo · Lluvia · Clima automático · Tareas del día · Roles de acceso · Costo por animal · Reportes · Comparativo anual · Presupuesto · Calendario · Galería · Asistente IA por voz · Proyecciones · Exportar Excel/PDF · Notificaciones · Historial de cambios · Modo sin internet (PWA)

---

## Próximas versiones

- [ ] Base de datos en la nube (Supabase) — datos seguros en servidor
- [ ] Login con número de teléfono
- [ ] Sistema de suscripción mensual
- [ ] Notificaciones por WhatsApp
- [ ] Pesaje masivo de animales
- [ ] Lotes y grupos de animales
- [ ] App nativa (iOS / Android)

---

## Tecnologías

- HTML5 + CSS3 + JavaScript — sin frameworks, un solo archivo
- [Claude API](https://anthropic.com) — IA para asistente, escaneo de aretes, notas y productos
- [Leaflet.js](https://leafletjs.com) + ESRI — Mapa satelital gratuito
- [Open-Meteo](https://open-meteo.com) — Datos de lluvia sin API key
- Web Speech API — Voz (dictado y lectura de respuestas)
- Service Worker — Modo sin internet

---

## Contacto y soporte

- Email: contacto@mirancho.mx
- WhatsApp: (993) xxx-xxxx

---

*MiRancho — Hecho en Tabasco, México*
