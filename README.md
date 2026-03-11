# Ciencia de Datos y Políticas Públicas — Versión Web Interactiva

&gt; **Recurso de capacitación técnica** para equipos de gobierno, orientado al análisis de datos con R aplicado a la gestión pública territorial.

[![GCBA](https://img.shields.io/badge/GCBA-Ciudad%20de%20Buenos%20Aires-003366?style=flat-square)](https://buenosaires.gob.ar)
[![Licencia](https://img.shields.io/badge/Licencia-CC%20BY--SA%204.0-00f0ff?style=flat-square)](LICENSE)
[![R](https://img.shields.io/badge/R-%3E%3D%204.0-276DC3?style=flat-square&logo=r)](https://r-project.org)

---

## 📋 Índice

- [Propósito institucional](#propósito-institucional)
- [Público objetivo](#público-objetivo)
- [Estructura del contenido](#estructura-del-contenido)
- [Requisitos técnicos](#requisitos-técnicos)
- [Implementación en otras jurisdicciones](#implementación-en-otras-jurisdicciones)
- [Créditos y atribución](#créditos-y-atribución)
- [Contacto](#contacto)

---

## 🎯 Propósito institucional

Este recurso digitaliza y amplía el manual *"Ciencia de Datos y Políticas Públicas"* de Antonio Vázquez Brust, adaptándolo como **plataforma de autoaprendizaje interactiva** para:

| Objetivo | Descripción |
|----------|-------------|
| **Capacitar** | Formar funcionarios en herramientas de análisis de datos sin requerir background técnico previo |
| **Estandarizar** | Homogeneizar metodologías de análisis entre distintas áreas de gobierno |
| **Transparentar** | Democratizar el acceso a técnicas antes reservadas a especialistas externos |
| **Optimizar** | Reducir tiempos de procesamiento de información ciudadana (reclamos, censos, geolocalización) |

&gt; *"La mayor parte del tiempo en ciencia de datos se insume en la poco glamorosa tarea de recopilar, limpiar y combinar registros. Este manual acorta esa curva de aprendizaje."* — Capítulo 2

---

## 👥 Público objetivo

**Perfiles prioritarios dentro de la AGC:**

- **Analistas de políticas públicas** que procesan datos de encuestas, censos o registros administrativos
- **Equipos de atención ciudadana** (SUACI/similares) que necesitan visualizar patrones territoriales de demandas
- **Áreas de planificación urbana** que trabajan con información georreferenciada
- **Direcciones de estadística** que migran desde Excel hacia herramientas reproducibles
- **Unidades de datos** que requieren capacitar a áreas descentralizadas sin presencialidad

**Nivel de entrada:** No se requiere conocimiento previo de programación. Solo computadora con acceso a internet (para versión web) o RStudio Desktop instalado (para práctica local).

---

## 📚 Estructura del contenido

| Módulo | Competencia desarrollada | Dataset de práctica CABA |
|--------|--------------------------|--------------------------|
| **1. Fundamentos** | Entender el rol del científico de datos en gobierno | — |
| **2. Primeros pasos en R** | Instalación, sintaxis básica, carga de datos | SUACI 2018 (contactos por barrio) |
| **3. Data Wrangling** | Limpiar, filtrar, agrupar y cruzar tablas | SUACI 2013-2015 (series temporales) |
| **4. Visualización** | Crear gráficos institucionales para informes | Comunas CABA (población vs. contactos) |
| **5. Modelado estadístico** | Regresiones lineares para proyecciones | Gapminder Argentina (tendencias históricas) |
| **6. Información geográfica** | Mapas temáticos con límites administrativos | Radios censales, barrios, SUBTE |

**Metodología pedagógica:**
- Ejemplos con datos reales del portal de datos abiertos de CABA
- Código ejecutable copiable con un clic
- Alternancia entre explicación conceptual y práctica inmediata
- Visualizaciones interactivas que simulan salidas de R

---

## 💻 Requisitos técnicos

### Para visualización web (autoaprendizaje)
- Navegador moderno (Chrome, Firefox, Edge, Safari)
- Conexión a internet para cargar CDN de Tailwind, Prism y Chart.js

### Para práctica local (recomendado)
- **R** ≥ 4.0 ([descargar](https://cloud.r-project.org/))
- **RStudio Desktop** ([descargar](https://posit.co/download/rstudio-desktop/))
- Paquetes a instalar:
  ```r
  install.packages(c("tidyverse", "sf", "ggplot2", "dplyr", "readr"))
