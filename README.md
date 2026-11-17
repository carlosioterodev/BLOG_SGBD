# Blog de SGBD

Blog del **Proyecto Final de Gestión de Bases de Datos (GBD)** — Universidad Autónoma de Chiriquí, Departamento de Ciencias Computacionales.

**Grupo:** Aaron Pérez · Carlos Otero · Enrique López · Cristian Carrera
**Sustentación:** 17 de noviembre de 2026

Sitio estático en HTML + CSS (sin frameworks ni pasos de compilación), listo para publicarse en **GitHub Pages**.

## Contenido

| # | Entrada | Archivo |
|---|---------|---------|
| 1 | ¿Qué es un SGBD? | `que-es-un-sgbd.html` |
| 2 | Clasificación de los SGBD | `clasificacion-sgbd.html` |
| 3 | Relacional vs. no relacional | `relacional-vs-no-relacional.html` |
| 4 | DMER vs. Diagrama Modelo Relacional | `dmer-vs-modelo-relacional.html` |
| 5 | PostgreSQL: nombre, siglas y origen | `postgresql-origen.html` |
| 6 | PostgreSQL: qué ofrece y cómo lo hace | `postgresql-que-ofrece.html` |
| 7 | PostgreSQL: características | `postgresql-caracteristicas.html` |
| 8 | PostgreSQL: estructura interna | `postgresql-estructura.html` |
| 9 | PostgreSQL en acción: ejemplo de uso | `postgresql-ejemplo.html` |

La portada (`index.html`) incluye a los **creadores con avatar y descripción profesional**, la **finalidad del blog**, la lista de entradas y las **referencias**.

## Estructura

```
blog-sgbd/
├── index.html              # Portada: finalidad, entradas, equipo, referencias
├── que-es-un-sgbd.html     # Entradas 1–9 (raíz del sitio)
├── ...
├── css/
│   └── style.css           # Sistema de diseño completo
├── .nojekyll               # Evita el procesamiento de Jekyll en GitHub Pages
├── .gitignore
└── README.md
```

## Verlo en local

Doble clic en `index.html`, o con un servidor local:

```powershell
# Python 3
python -m http.server 8000
# luego abre http://localhost:8000
```

## Publicar en GitHub Pages

1. Crear un repositorio público en GitHub (por ejemplo `blog-sgbd`) **sin** README ni .gitignore (ya vienen en este directorio).
2. Desde este directorio:

   ```powershell
   git init
   git add .
   git commit -m "Blog de SGBD — Proyecto Final GBD (UACI)"
   git remote add origin https://github.com/TU-USUARIO/blog-sgbd.git
   git push -u origin main
   ```

3. En el repositorio: **Settings → Pages → Build and deployment → Source: Deploy from a branch** → rama `main`, carpeta `/(root)` → **Save**.
4. En ~1 minuto el sitio quedará en `https://TU-USUARIO.github.io/blog-sgbd/`.

## Diseño

- Fondo blanco, texto gris oscuro, acento azul PostgreSQL (`#336791`).
- Tipografía de sistema (Segoe UI) para máxima legibilidad; cuerpo a 17 px.
- Responsive (móvil/tablet), estilos de impresión y sin dependencias externas.
