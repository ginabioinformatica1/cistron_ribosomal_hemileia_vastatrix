# Cistrón ribosomal de *Hemileia vastatrix*

Datos y documentación del análisis bioinformático de las regiones ITS, 18S y 28S de *Hemileia vastatrix* (roya del cafeto) a partir de secuencias públicas (NCBI GenBank y BOLD Systems): curación, alineamiento en MEGA, conservación y filogenia.

Material suplementario de la monografía: **Identificación de regiones ribosomales conservadas en Hemileia vastatrix**, Ginamaria Hernández Ruiz, Instituto Tecnológico Metropolitano, 2026.

## Estructura

| Carpeta | Contenido |
|---|---|
| `01_busqueda/` | Cadenas de búsqueda, series de secuencias recuperadas de *H. vastatrix* (22 series, 385 secuencias) y series de la búsqueda a nivel de familia |
| `02_curacion/` | Secuencias tras la curación (47), matriz final (35) y secuencias excluidas (12) |
| `03_alineamiento/` | Alineamiento múltiple de las 35 secuencias (formato MEGA), región conservada y parámetros de MUSCLE |
| `04_estadisticas/` | Resumen cuantitativo del alineamiento, frecuencias nucleotídicas y matriz de distancias pareadas (*p-distance*) |
| `05_filogenia/` | Matrices de entrada de los árboles de género (28S) y de familia (ITS), lista de secuencias del árbol de familia y figuras |
| `docs/` | Diagrama de flujo del proceso de selección de secuencias (Anexo C) |

## Métodos resumidos

- **Bases de datos:** NCBI GenBank y BOLD Systems. Fecha de consulta: 2026-11-12. Las cadenas de búsqueda están en `01_busqueda/cadenas_de_busqueda.md`.
- **Alineamiento:** MUSCLE en MEGA 12, con Gap Open = −400, Gap Extend = 0, 16 iteraciones máximas y agrupamiento UPGMA (detalle en `03_alineamiento/parametros_MUSCLE.md`).
- **Conservación y variabilidad:** identidad pareada (*p-distance*), sitios conservados, variables y *singletons*, y frecuencias nucleotídicas en MEGA.
- **Filogenia:** Máxima Verosimilitud en MEGA, con modelo de sustitución seleccionado por BIC y 1.000 réplicas de *bootstrap*. Un árbol a nivel de género (región 28S) y otro a nivel de familia (complejo ITS).
- **Visualización del alineamiento:** Jalview.

El detalle completo está en la monografía.

## Notas

- `matriz_distancias_pareadas.xlsx` contiene distancias (*p-distance*) entre las 35 secuencias. La identidad se calcula como 1 − p.
- Las secuencias provienen de GenBank y BOLD; deben citarse por sus números de acceso.
- Los porcentajes de los archivos de Excel pueden aparecer con coma o punto decimal según la configuración regional del programa.

## Licencia

CC0 1.0 Universal (ver `LICENSE`).

## Cómo citar

Ver `CITATION.cff` o citar el archivo depositado en Zenodo:

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24507239.svg)](https://doi.org/10.5281/zenodo.24507239)

Hernández Ruiz G. Cistrón ribosomal de Hemileia vastatrix: datos y documentación del análisis bioinformático [conjunto de datos]. Zenodo; 2026. https://doi.org/10.5281/zenodo.24507239
