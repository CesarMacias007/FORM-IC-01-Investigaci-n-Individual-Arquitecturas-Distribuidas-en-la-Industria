# FORM-IC-01 — Investigación individual: arquitecturas distribuidas en la industria

**Estudiante:** MACIAS VÁSQUEZ CÉSAR ABRAHAN  
**Asignatura:** Aplicaciones Distribuidas — Séptimo Nivel, Paralelo "B"  
**Docente:** Gleiston Cicerón Guerrero Ulloa, PhD  
**Periodo Académico:** SPA 2026–2027  
**Caso analizado:** Amazon (estilo arquitectónico: Microservicios)

## Estructura del repositorio

```text
.
├── README.md                              # Instrucciones de compilación y estructura del proyecto
├── main.tex                               # Documento LaTeX principal (carátula, análisis de 1 página, evidencias y referencias)
├── main.pdf                               # Documento principal compilado
├── referencias.bib                        # Base bibliográfica en formato BibLaTeX (fuentes oficiales de Amazon/AWS y artículos IEEE)
├── img/
│   └── logo_uteq.png                      # Logotipo institucional empleado en la carátula
├── capturas/
│   └── captura_fuente_principal.png       # Captura de la fuente principal con fragmentos subrayados/anotados
└── sga/
    ├── entrega_sga.tex                    # Documento LaTeX de una sola página para la entrega en el SGA
    └── entrega_sga.pdf                    # PDF de una sola página (datos identificativos + URL del repositorio)
```

## Instrucciones de compilación

### 1. Documento principal (`main.tex`)

* **Compilador:** `pdflatex` (distribución TeX Live o MiKTeX)
* **Gestor bibliográfico:** `biber` (backend de `biblatex`, estilo `ieee`)
* **Archivo principal:** `main.tex`
* **Orden de comandos:**

```bash
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

### 2. Documento de entrega en el SGA (`sga/entrega_sga.tex`)

```bash
cd sga
pdflatex entrega_sga.tex
pdflatex entrega_sga.tex
```

### Dependencias de LaTeX requeridas

Los archivos `.tex` utilizan los siguientes paquetes estándar de CTAN:
* `inputenc` (`utf8`), `fontenc` (`T1`), `babel` (`spanish`)
* `mathptmx` (tipografía Times)
* `geometry`, `setspace`, `parskip`, `titlesec`, `enumitem`
* `graphicx`, `float`, `caption`, `xcolor`, `framed`
* `hyperref`, `url`
* `csquotes`, `biblatex` (con `backend=biber` y `style=ieee`)
