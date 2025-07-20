
# 📘 Manual de Usuario – Recomendador Inteligente de Negocios Locales en Sabaneta

## 🧠 ¿Qué es?
Es una plataforma digital basada en inteligencia artificial que te ayuda a encontrar comercios y servicios locales en Sabaneta, Antioquia. Solo escribe lo que necesitas, y el sistema te mostrará negocios relacionados. Este sistema combina una base de datos con un modelo de recomendación basado en aprendizaje automático (TF-IDF) aplicado sobre descripciones de productos o servicios.

👉 Sitio desplegado: https://carolina-project-m8si.onrender.com

---

## 🚀 ¿Cómo buscar un negocio?

1. Ingresa al sitio web desde tu navegador.
2. En el campo de búsqueda escribe palabras clave como:
   - Ej: `soporte TV`, `panadería`, `miel`, `ropa deportiva`, `masajes`.
3. Haz clic en el botón **"Buscar"**.
4. Se mostrará una lista de negocios relacionados con tu búsqueda.
5. Haz clic en la dirección del negocio para ver su ubicación embebida en Google Maps directamente en la página.

---

## 🏪 ¿Cómo registrar un nuevo negocio?

1. Da clic en el botón **“Registrar un comercio”**.
2. Completa el formulario con los siguientes campos:
   - Nombre del negocio
   - Sector y Subsector
   - Artículos o servicios que ofrece
   - Dirección
   - Celular y teléfono (opcional)
   - Logo del negocio (opcional)
   - Enlaces de Facebook, Instagram y Google Maps (si están disponibles)
3. Haz clic en **“Registrar”**.
4. Si todo está correcto, verás un mensaje de éxito. En caso de errores, se mostrará una alerta con los campos a corregir.
5. El nuevo negocio se guarda automáticamente en:
   - La base de datos del sistema (SQLite/PostgreSQL).
   - El archivo `data/base_actualizada.xlsx`.

⚠️ **Nota**: El negocio recién ingresado podrá aparecer en futuras recomendaciones si el término buscado coincide con el campo “Artículos” del formulario.

---

## 🗺️ ¿Cómo ver la ubicación de un negocio?

- En los resultados de búsqueda, cada dirección es un enlace.
- Al hacer clic en una dirección, se muestra un mapa de Google Maps debajo de los resultados.
- Esto te permite ubicar el comercio fácilmente sin salir del sitio.

---

## 💡 Recomendaciones de uso

- Sé específico con tus palabras clave para obtener resultados más relevantes.
- Usa descripciones detalladas como "miel orgánica", "ropa infantil", "masajes deportivos", etc.
- Si eres dueño de un negocio, mantén tus datos actualizados para mejorar tu visibilidad.
- Incluye el enlace de Google Maps para facilitar la ubicación del comercio.


