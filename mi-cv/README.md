# 📄 Mi CV — LaTeX + GitHub Actions

CV profesional escrito en LaTeX que se **compila automáticamente a PDF** cada vez que haces `push` a `main`.

## ⚡ ¿Cómo funciona?

```
Editas cv.tex → Push a GitHub → GitHub Actions compila → PDF listo para descargar
```

## 🚀 Cómo usarlo (sin instalar nada)

### 1. Crear repositorio en GitHub
- Ve a [github.com/new](https://github.com/new)
- Nombre: `mi-cv`
- Marca **Public** y **Add a README file**
- Clic en **Create repository**

### 2. Subir los archivos
- En tu repo, clic en **Add file** → **Upload files**
- Arrastra los 3 archivos: `cv.tex`, `.github/workflows/compilar-cv.yml` y este `README.md`
- Clic en **Commit changes**

### 3. Editar tu CV
- Haz clic en `cv.tex` dentro del repositorio
- Clic en el ícono de lápiz ✏️ para editar
- Cambia los datos por los tuyos
- Clic en **Commit changes**

### 4. Descargar tu PDF
Después de cada commit, GitHub Actions compilará tu CV. Para descargar el PDF:

- **Opción A — Releases**: Ve a la pestaña **Releases** (barra lateral derecha) y descarga el PDF
- **Opción B — Actions**: Ve a **Actions** → clic en el último workflow → sección **Artifacts** → descarga `cv-pdf`

## 📁 Estructura

```
mi-cv/
├── cv.tex                              ← Tu CV (edita este archivo)
├── .github/
│   └── workflows/
│       └── compilar-cv.yml             ← Workflow de compilación
└── README.md
```

## ✏️ Personalización

Abre `cv.tex` y edita las secciones que necesites. El archivo está organizado y comentado para que sea fácil de modificar:

| Sección | Qué cambiar |
|---------|-------------|
| **Encabezado** | Nombre, título, contacto, links |
| **Perfil** | Tu resumen profesional |
| **Experiencia** | Empresas, puestos, logros |
| **Educación** | Universidad, carrera, fechas |
| **Habilidades** | Tecnologías y porcentajes |
| **Certificaciones** | Cursos y certificados |
| **Proyectos** | Repos destacados |

## 🎨 Cambiar colores

Al inicio de `cv.tex` encontrarás:

```latex
\definecolor{accent}{HTML}{B71C1C}    % rojo — color principal
\definecolor{darktext}{HTML}{1A1A2E}  % texto oscuro
\definecolor{graytext}{HTML}{555555}  % texto secundario
```

Cambia los códigos hex por los colores que prefieras.
