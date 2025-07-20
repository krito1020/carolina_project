# Recomendador de Comercios Sabaneta 🛍️

Este proyecto es una aplicación web construida con Django y desplegada en [Render](https://render.com), que permite a usuarios buscar recomendaciones de comercios en Sabaneta, Antioquia, y a los propietarios registrar nuevos negocios para visibilizar su oferta.

---

## 🧠 Características

- Motor de recomendación usando TF-IDF + NLP (con `spaCy` y `scikit-learn`)
- Formulario de registro de nuevos comercios con carga de imágenes (logo)
- Guardado automático en base de datos SQLite y Excel (`base_actualizada.xlsx`)
- Diseño responsivo con HTML, CSS y templates de Django
- Deploy automático en Render
- Manejo de archivos estáticos con `Whitenoise`
- Registro de mensajes (éxito / error) en la interfaz de usuario

---

## 🗂 Estructura del proyecto

```
carolina_project/
├── apps/
│   └── recomendador/
│       ├── forms.py
│       ├── models.py
│       ├── recommender.py
│       ├── urls.py
│       ├── views.py
│       └── templates/
│           ├── base.html
│           ├── index.html
│           └── registro.html
├── data/
│   └── base_actualizada.xlsx
├── logos/
├── static/
├── settings.py
├── urls.py
├── wsgi.py
├── manage.py
├── requirements.txt
├── Procfile
├── render.yaml
└── README.md
```

---

## 🚀 Despliegue en Render

### 1. Requisitos

- Cuenta en [Render.com](https://render.com)
- Repositorio conectado en GitHub
- Archivos necesarios:
  - `Procfile`
  - `render.yaml`
  - `requirements.txt`
  - `runtime.txt` (opcional)

### 2. Variables de entorno (opcional)

Si usas un `.env`, asegúrate de definir:

```bash
DEBUG=True
SECRET_KEY=tu_clave_secreta
```

---

## 💻 Uso local

```bash
# Instala dependencias
pip install -r requirements.txt

# Ejecuta migraciones
python manage.py migrate

# Corre el servidor
python manage.py runserver
```

---

## 🤖 Modelo de Recomendación

Se encuentra en `apps/recomendador/recommender.py`. Usa TF-IDF y `cosine_similarity` para calcular similitudes entre los textos de los artículos registrados por los comercios.

---

## 📂 Base de Datos en Excel

Los nuevos registros se almacenan tanto en la base SQLite como en el archivo `data/base_actualizada.xlsx`. El sistema detecta automáticamente si el archivo ya existe y continúa escribiendo en él.

---

## ✨ Créditos

Desarrollado por *Carolina Ospina*

Repositorio: https://github.com/krito1020/carolina_project.git
Deploy en: https://carolina-project-m8si.onrender.com