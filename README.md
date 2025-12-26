# Project Hub

Welcome 👋  
This repository serves as the **central landing page and documentation hub** for my projects.

It is built using **MkDocs** with the **Material theme** and deployed via **GitHub Pages**, making all project information and documentation publicly accessible in a simple and structured way.

🌐 **Live Site**  
https://muslim-hyperjump.github.io/

---

## 🚀 Purpose

This repository is designed to:

- Act as a **landing page** for all projects
- Provide **clear documentation** and user guides
- Share **technical architecture and implementation details**
- Serve as a **single source of truth** for project references

---

## 🛠️ Local Development Setup

### Prerequisites

Before running this project locally, ensure you have the following installed:

- **Python 3.8+** (check with `python --version` or `python3 --version`)
- **pip** (Python package manager)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/muslim-hyperjump/muslim-hyperjump.github.io.git
   cd muslim-hyperjump.github.io
   ```

2. **Create a virtual environment** (recommended)
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install mkdocs-material
   ```

### Running Locally

To start the local development server:

```bash
mkdocs serve
```

This will start a local server at `http://127.0.0.1:8000/`. The site will automatically reload when you make changes to the documentation files.

### Common Commands

- **Start dev server**: `mkdocs serve`
- **Build static site**: `mkdocs build`
- **Deploy to GitHub Pages**: `mkdocs gh-deploy`
- **Clean build directory**: `rm -rf site/`

### Project Structure

```text
.
├── docs/                  # Documentation source files
│   ├── index.md          # Homepage
│   ├── projects.md       # Projects overview
│   └── stylesheets/      # Custom CSS
├── mkdocs.yml            # MkDocs configuration
├── venv/                 # Python virtual environment
└── README.md             # This file
```

---

## 📦 Projects

### 1️⃣ Project Name
**Short description of the project in one sentence.**

- 🌐 Landing Page: `/projects/project-name`
- 📘 Documentation: `/docs/project-name`
- 💻 Repository: https://github.com/<org>/<repo>

**Key Features**
- Feature A
- Feature B
- Feature C

---

### 2️⃣ Project Name
**Short description of the project in one sentence.**

- 🌐 Landing Page: `/projects/project-name`
- 📘 Documentation: `/docs/project-name`
- 💻 Repository: https://github.com/<org>/<repo>

---

## 📚 Documentation Structure

All documentation is written in **Markdown** and organized as follows:

```text
/docs
  ├── index.md               # Documentation homepage
  ├── projects
  │   ├── project-a
  │   │   ├── index.md
  │   │   ├── getting-started.md
  │   │   ├── architecture.md
  │   │   └── api.md
  │   └── project-b
  │       └── index.md
  └── shared
      ├── deployment.md
      └── conventions.md
