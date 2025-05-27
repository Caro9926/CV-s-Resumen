# 📄 Automatizador de Extracción de CVs en PDF

Este repositorio contiene un script en Python que permite **extraer información estructurada desde currículums en PDF** (como nombre, correo, educación, etc.) y consolidarla automáticamente en un archivo de Excel.

---

## 🚀 ¿Qué hace este proyecto?

🔍 Analiza automáticamente cientos de CVs PDF.  
🧠 Identifica y extrae las secciones más relevantes del contenido textual.  
📊 Organiza los datos en un archivo `.xlsx` limpio y exportable.  
🗂️ Permite un análisis fácil y sistemático de postulantes.

---

## 💼 Información extraída

El script identifica las siguientes secciones por cada CV:

| Campo              | Descripción                                                  |
|-------------------|--------------------------------------------------------------|
| `Nombre`          | Primera línea del CV (supuesto nombre del candidato)         |
| `Correo`          | Email (formato estándar `nombre@dominio.com`)                |
| `Teléfono`        | Número telefónico local o internacional                      |
| `LinkedIn`        | Enlace a perfil de LinkedIn (si está presente)               |
| `Educación`       | Sección educativa completa                                   |
| `Experiencia`     | Trayectoria laboral y profesional                            |
| `Idiomas`         | Lenguas o niveles de competencia lingüística                 |
| `Extras`          | Voluntariados, actividades extracurriculares, etc.           |
| `Archivo`         | Nombre del archivo PDF original                              |

---

## 🧩 Requisitos

Instala las dependencias necesarias:

```bash
pip install pymupdf pandas openpyxl
