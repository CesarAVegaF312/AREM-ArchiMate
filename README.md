# 🛠️ ArchiMate — Notación Estándar del Curso

Este repositorio contiene la guía de referencia de **ArchiMate**, el estándar principal de modelado del curso Arquitectura Empresarial. Complementa — no reemplaza — a BPMN (Taller 1), ERD (Taller 2), C4 (Taller 3) y las demás herramientas usadas en cada taller.

---

## 🧩 ¿Qué es ArchiMate y por qué es el estándar del curso?

[ArchiMate](https://www.opengroup.org/archimate-forum) es el lenguaje de modelado de arquitectura empresarial del Open Group, el mismo consorcio detrás de TOGAF. Mientras **TOGAF ADM** define el *método* — la secuencia de fases que ya siguen los Talleres 0 a 9 —, **ArchiMate** define el *lenguaje* — la notación común con la que se documenta cada capa (negocio, aplicación, tecnología) para que cualquier persona del comité pueda leerla, sin importar qué taller la produjo.

## 📘 Guía de notación

Revise la [**Guía de Notación ArchiMate**](guia_notacion_archimate.md). Incluye las 5 capas (Motivación, Negocio, Aplicación, Tecnología, Implementación y Migración) con su código de color, los elementos principales de cada una, las relaciones semánticas correctas, una metodología de 4 pasos para construir una vista, un ejemplo completo integrando el caso de la Clínica Salud Viva (Talleres 1 y 2), errores comunes y checklist de autoevaluación.

## 🔗 Cómo se conecta con los demás talleres

Cada guía del curso (Talleres 0 a 9) incluye una sección **"Vista ArchiMate equivalente"** que muestra cómo el diagrama de ese taller (BPMN, ERD, C4, mapa de infraestructura, tabla STRIDE, checklist normativo, matriz de brechas, tablero integrado o roadmap de implementación) se traduce a elementos y relaciones de ArchiMate. Esa sección siempre remite aquí para la notación completa — no la repite.

| Taller | Capa(s) ArchiMate principal(es) |
|---|---|
| 0 — Preliminary y Vision | Motivación |
| 1 — BPMN | Negocio |
| 2 — Modelo de Información | Negocio + Aplicación (datos) |
| 3 — Arquitectura C4 | Aplicación |
| 4 — Infraestructura | Tecnología |
| 5 — STRIDE | Motivación (Requirement) |
| 6 — Normatividad | Motivación (Requirement / Constraint) |
| 7 — Opportunities & Solutions | Implementación y Migración (Plateau / Gap) |
| 8 — Integración de Vistas | Las 4 capas estructurales en una sola vista |
| 9 — Presentación Final | Implementación y Migración (Work Package) |

## 🧰 Herramientas sugeridas

- **[Archi](https://www.archimatetool.com/)** — gratuito, dedicado exclusivamente a ArchiMate.
- **draw.io** — biblioteca de formas "ArchiMate 3" disponible en el panel de formas. Es la que ya usa el resto del curso para BPMN/C4/ERD, así que no exige aprender una herramienta nueva.
- **Astah Archimate** — ver el repositorio [`AREM-astah`](https://github.com/CesarAVegaF312/AREM-astah).

### Ejemplo importable en Archi

El modelo de Clínica Salud Viva de la sección 5 de la guía también está disponible como [`ejemplo-clinica-salud-viva-exchange.xml`](ejemplo-clinica-salud-viva-exchange.xml), en el **formato estándar de intercambio de ArchiMate** (Model Exchange File Format de The Open Group). Para abrirlo:

1. Instale Archi y ábralo.
2. `File → Import → ArchiMate Model Exchange File...`
3. Seleccione el archivo `.xml`.

⚠️ Este archivo se escribió siguiendo el esquema oficial (`archimate3_Model.xsd` de The Open Group) y se corrigió tras una primera prueba de importación real en Archi. Si al importar sigue dando error, es más rápido recrear el modelo a mano (son solo 7 elementos y 6 relaciones, los mismos de la sección 5 de la guía) que seguir depurando el XML.

---

## ✅ Licencia

Este repositorio es de uso académico bajo licencia MIT. Hace parte del curso de Arquitectura Empresarial - Universidad de La Sabana.
