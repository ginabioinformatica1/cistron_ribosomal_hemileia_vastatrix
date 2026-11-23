# Cadenas de búsqueda

Las tres búsquedas se hicieron en NCBI GenBank (Nucleotide). Las cadenas se reproducen tal como se escribieron.

## 1. NCBI GenBank: *Hemileia vastatrix* (alineamiento y conservación)
- URL: https://www.ncbi.nlm.nih.gov/nucleotide/
- Fecha de consulta: 2026-11-12
- Cadena de búsqueda: "Hemileia vastatrix" AND ("18S" OR "SSU" OR "internal transcribed spacer 1" OR "ITS1" OR "5.8S" OR "internal transcribed spacer 2" OR "ITS2" OR "28S" OR "LSU")
- Filtros aplicados: ninguno
- Resultados obtenidos: 490 registros
- Excluidos: 105 registros que no correspondían a secuencias de *H. vastatrix* (otras especies)
- Conservados: 385 secuencias, agrupadas en 22 series (ver `tabla_series_recuperadas.csv`)

## 2. NCBI GenBank: género *Hemileia* (árbol a nivel de género, 28S)
- Fecha de consulta: 2026-11-12
- Cadena de búsqueda: "Hemileia" NOT "Hemileia vastatrix" AND ("18S" OR "SSU" OR "internal transcribed spacer 1" OR "ITS1" OR "5.8S" OR "internal transcribed spacer 2" OR "ITS2" OR "28S" OR "LSU")
- Filtros aplicados: ninguno
- Resultados obtenidos: 191 registros
- Excluidos: 183 registros rotulados como "uncultured fungus isolate"
- Conservados: 8 secuencias de otras especies de *Hemileia* (7 de 28S y 1 de 18S)

## 3. NCBI GenBank: familia Zaghouaniaceae (árbol a nivel de familia, ITS)
- Fecha de consulta: 2026-11-12
- Cadena de búsqueda: "Zaghouaniaceae" NOT "Hemileia vastatrix" AND ("18S" OR "SSU" OR "internal transcribed spacer 1" OR "ITS1" OR "5.8S" OR "internal transcribed spacer 2" OR "ITS2" OR "28S" OR "LSU")
- Filtros aplicados: ninguno
- Resultados obtenidos: 38 registros (ver `tabla_series_familia.csv`)
- Excluidos: secuencias sin el complejo ITS y secuencias de BOLD (*Aecidium*), que no se usaron en el árbol
- Conservados: 17 secuencias de Zaghouaniaceae (10 de otros géneros y 7 de *H. vastatrix*)
- Las 7 secuencias de *H. vastatrix* (EF394122, EF394124, EF394126, KX260247.1, KX260248.1, KX260249.1 y MF417751.1) provienen de la búsqueda 1.
- Grupos externos (4 secuencias): *Melampsora laricis-populina* (EU014067.1, AY646241.1) y *Puccinia graminis* (HQ317538.1, HQ317585.1).
- Matriz final: 21 secuencias (`matriz_arbol_familia_ITS.fasta`)

## 4. BOLD Systems
- URL: https://boldsystems.org/
- Fecha de consulta: 2026-11-12
- Búsqueda realizada: "Hemileia vastatrix"[tax]
- Resultados obtenidos: 16 (las series EF394 y DQ022191 coinciden con registros de NCBI)
- Las series de BOLD que aparecieron en la búsqueda de familia (AB354 y EF635896, *Aecidium*) no se usaron en el árbol.

## Criterios de selección
- Se conservaron únicamente secuencias con información de origen geográfico.
- Se excluyeron secuencias con ambigüedades excesivas, incompletas, con errores en los extremos o de otros genes u otras especies.