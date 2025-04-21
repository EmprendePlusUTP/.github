# 📦 Emprende+ – Plataforma de Gestión para Emprendedores

![alt text](https://github.com/EmprendePlusUTP/.github/blob/d9f593f9832af64222d8a78e9741c506017c1d1b/EmprendePlusLogo.png?raw=true)

**Emprende+** es una plataforma desarrollada por estudiantes de Ingeniería en Sistemas en la Universidad Tecnológica de Panamá. Su objetivo principal es brindar a estudiantes emprendedores una herramienta digital donde puedan:

- Registrar sus productos
- Ingresar manualmente ventas
- Visualizar métricas clave (ventas por mes, productos más vendidos)
- Tener un punto de partida para gestionar su emprendimiento de forma ordenada

---

## 🧭 Organización del Proyecto

Este proyecto está organizado bajo [EmprendePlusUTP](https://github.com/EmprendePlusUTP), y está dividido en dos repositorios principales:

| Repositorio       | Descripción                                       |
|-------------------|---------------------------------------------------|
| [Frontend](https://github.com/EmprendePlusUTP/web-emprendePlus) | Aplicación web construida con React, Vite, Tailwind, D3.js |
| [Backend](https://github.com/EmprendePlusUTP/server-emprendePlus)   | API REST construida con FastAPI y SQLModel usando SQLite  |

---

## ⚙️ Requisitos para ejecutar localmente

### 1. ✅ Instalar Node.js (para el frontend)

- Descargar desde: [https://nodejs.org](https://nodejs.org)
- Verificar instalación:
  ```bash
  node -v
  ```

### 2. ✅ Instalar Python 3.10+ (para el backend)

- Descargar desde: [https://www.python.org/downloads/](https://www.python.org/downloads/)

### 3. ✅ Instalar Git

- Descargar desde: [https://git-scm.com/](https://git-scm.com/)
- Recomendamos **usar [Fork](https://fork.dev/)** como cliente visual para evitar el uso de comandos Git por consola.
  - Permite clonar repos, hacer commits y manejar ramas con interfaz amigable.

---

## 🚀 Instrucciones de instalación y ejecución

### 🔷 Clonar los repositorios

```bash
# Usando Git CLI (opcional si usas Fork)
git clone https://github.com/EmprendePlusUTP/web-emprendePlus
git clone https://github.com/EmprendePlusUTP/server-emprendePlus
```

---

### 🔷 Frontend (`web-emprendePlus`)

```bash
cd web-emprendePlus
npm install
npm run dev
```

Asegúrate de tener el backend corriendo en `http://localhost:8000`.

---

### 🔷 Backend (`server-emprendePlus`)

```bash
cd server-emprendePlus
python -m venv venv
source venv/bin/activate  # o venv\Scripts\activate en Windows
pip install -r requirements.txt
uvicorn main:app --reload
```

---

## 🧩 Extensiones recomendadas para Visual Studio Code

### 🔷 Frontend

- [Tailwind CSS IntelliSense](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss)
- [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
- [Error Lens](https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens)
- [ES7+ React Snippets](https://marketplace.visualstudio.com/items?itemName=dsznajder.es7-react-js-snippets)

### 🔷 Backend

- [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
- [Pylance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance)
- [SQLite Viewer](https://marketplace.visualstudio.com/items?itemName=qwtel.sqlite-viewer)
- [Error Lens](https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens)

---

## 🗃️ Base de datos

El backend usa **SQLite** como motor de base de datos local.

Puedes visualizar el archivo `.db` con:

- [SQLite Viewer (VS Code)](https://marketplace.visualstudio.com/items?itemName=qwtel.sqlite-viewer)
- [DB Browser for SQLite](https://sqlitebrowser.org/)

---

## 🌱 Convención de branches

Para mantener un flujo ordenado:

- La rama principal de desarrollo es `dev`.
- Toda nueva funcionalidad debe crearse desde `dev`:

```bash
git checkout dev
git pull origin dev
git checkout -b feature/nombre-de-la-feature
```

### ✅ Tipos de ramas recomendados:

| Tipo     | Prefijo       | Ejemplo                         |
|----------|---------------|----------------------------------|
| Feature  | `feature/`    | `feature/login-form`             |
| Fix      | `fix/`        | `fix/fetch-sales-error`          |
| Docs     | `docs/`       | `docs/update-readme`             |
| Refactor | `refactor/`   | `refactor/dashboard-logic`       |
| Test     | `test/`       | `test/product-api`               |

---

## 📝 Convención de commits

Usamos el formato:

```bash
<tipo>-<#tarea>-descripción_breve_en_infinitivo
```

### Ejemplos:

- `feat: agregar gráfico de ventas`
- `fix: corregir error al eliminar producto`
- `docs: actualizar README`
- `refactor: mejorar lógica de cálculo total`
- `style: aplicar formato con Prettier`

---

## 📫 Contacto

Este proyecto está gestionado por el equipo de estudiantes de la UTP.  
Más información en la [Organización EmprendePlusUTP](https://github.com/EmprendePlusUTP).
