# Tarea 2 — Recargos de Responsabilidad Civil

### Integrantes Equipo 5:

- Avila Padilla Militza Esmeralda
- Contreras Valeria Jade Fátima
- Cruz Rodriguez Avril Azeneth
- Jiménez Jiménez Brisa Yurubi
- Moreno Ventura Miguel Angel
- Ramirez Cabrera Miguel Ángel

Para Responsabilidad Civil propongo **comisiones de 18.4% a 24.7%** y **gastos de 5.5% a 11.5%**, ambos sobre prima emitida.

| Recargo                   | Rango          | Valor central | Base                  | Fuente de los datos                     |
| ------------------------- | -------------- | ------------- | --------------------- | --------------------------------------- |
| Comisiones (Adquisición) | 18.4% – 24.7% | 21.5%         | Prima emitida (Clase) | AXA Seguros 2025 y GNP 2024             |
| Gastos (Operación)       | 5.5% – 11.5%  | 9.0%          | Prima emitida (Clase) | AXA Seguros 2023–2025 y GNP 2022–2024 |

El rango de comisiones descansa en solo dos observaciones (una por aseguradora); el de gastos, en seis. Las salvedades están al final.

## Fuentes

Dos aseguradoras con tres años cada una, todas del Reporte sobre la Solvencia y Condición Financiera (RSCF) de la propia aseguradora.

| Aseguradora                             | Reporte   | Años                            | Dónde está el dato                                               |
| --------------------------------------- | --------- | -------------------------------- | ------------------------------------------------------------------ |
| AXA Seguros, S.A. de C.V.               | RSCF 2025 | Montos 2025; índices 2023–2025 | Tabla D4 (p. 81); Tablas G1 a G5 (pp. 104–108); Tabla G9 (p. 112) |
| Grupo Nacional Provincial, S.A.B. (GNP) | RSCF 2024 | Montos 2024; índices 2022–2024 | Sección D, Tabla D4; Sección G, Tablas G1 a G5                   |

Archivos: [github.com/VenturaMiguel20/MASDFR_20271/tree/db378880f9361df6dc7a78d424e9ce704851ee22/clases/clase_12/Fuentes](https://github.com/VenturaMiguel20/MASDFR_20271/tree/db378880f9361df6dc7a78d424e9ce704851ee22/clases/clase_12/Fuentes)

## Índices calculados

Sobre prima emitida, la adquisición directa de RC es 24.7% en AXA (2025) y 18.4% en GNP (2024). La operación va de 2.6% a 21.1% en seis observaciones.

**Montos de RC en el estado de resultados (Tabla D4, millones de pesos)**

| Concepto                                     | AXA Seguros 2025 |     GNP 2024 |
| -------------------------------------------- | ---------------: | -----------: |
| Prima emitida                                |            1,412 |          849 |
| Prima cedida (% de la emitida)               |        722 (51%) |    639 (75%) |
| Prima retenida                               |              690 |          210 |
| Prima de retención devengada                |              679 |          254 |
| Comisiones a agentes                         |              154 |           96 |
| Compensaciones adicionales a agentes (bonos) |               55 |           28 |
| Otros gastos de adquisición                 |              139 |           32 |
| Comisiones por reaseguro tomado              |               12 |            0 |
| (-) Comisiones por reaseguro cedido          |             -193 |         -145 |
| Cobertura de exceso de pérdida              |               64 |            9 |
| **Costo neto de adquisición**         |    **231** | **20** |
| Siniestros netos                             |              316 |           83 |

**Índices con la base de la guía**

| Índice                                                 | Cálculo                                      | AXA Seguros 2025 |        GNP 2024 |
| ------------------------------------------------------- | --------------------------------------------- | ---------------: | --------------: |
| Adquisición neta ÷ emitida (método dado en la guía) | costo neto ÷ prima emitida                   |            16.4% |            2.4% |
| Comisiones y bonos ÷ emitida                           | (comisiones + bonos) ÷ prima emitida         |            14.8% |           14.6% |
| **Adquisición directa ÷ emitida**               | (comisiones + bonos + otros) ÷ prima emitida |  **24.7%** | **18.4%** |
| Operación ÷ emitida (Tabla G4)                        | reportado, ya sobre prima emitida             |            21.1% |             12% |
| Siniestralidad (Tabla G2)                               | reportado, sobre devengada retenida           |            46.6% |             33% |
| Combinado (método dado en la guía)                   | G2 + adquisición neta ÷ emitida + G4        |            84.0% |           47.4% |
| Combinado oficial (Tabla G5)                            | reportado por la aseguradora                  |           101.1% |             52% |

La adquisición neta sale baja porque RC cede mucha prima y el reasegurador paga comisiones (-193 y -145 millones) que restan al costo. Por eso la adquisición directa, antes de reaseguro, es la cifra útil para la tarifa. El combinado oficial es mayor porque la CNSF divide la adquisición entre prima retenida, no emitida.

**Series oficiales de RC en las Tablas G1 a G5**

| Fuente y año | Prima emitida (millones) | Siniestralidad (G2) | Adquisición (G3) | Operación (G4) | Combinado (G5) |
| ------------- | -----------------------: | ------------------: | ----------------: | --------------: | -------------: |
| AXA 2025      |                    1,412 |              46.58% |            33.45% |          21.10% |        101.13% |
| AXA 2024      |                    1,188 |              40.03% |            43.14% |           2.62% |         85.78% |
| AXA 2023      |                    1,141 |              61.76% |            36.08% |           4.65% |        102.49% |
| GNP 2024      |                      849 |                 33% |                8% |             12% |            52% |
| GNP 2023      |                      874 |                 20% |               -1% |              8% |            29% |
| GNP 2022      |                      774 |                 49% |               -1% |             10% |            58% |

La columna G3 usa prima retenida (AXA) y prima retenida devengada (GNP), no prima emitida; se muestra solo como contexto. GNP reporta porcentajes enteros, así que cada cifra tiene un margen de ±0.5 puntos.

## Rango propuesto y justificación

Comisiones de 18.4% a 24.7% (central 21.5%) y gastos de 5.5% a 11.5% (central 9.0%), ambos sobre prima emitida.

**Comisiones (adquisición): 18.4% – 24.7%, central 21.5%**

1. Uso el costo directo, antes de reaseguro, porque la tarifa se aplica a la prima emitida y el reaseguro se modela aparte, en el esquema de reaseguro del proyecto.
2. El mínimo es GNP 2024 (18.4%) y el máximo AXA 2025 (24.7%); el valor central es su promedio.
3. Comisiones y bonos son casi iguales en las dos (14.6% y 14.8%). La diferencia está en otros gastos de adquisición: 3.8% en GNP y 9.8% en AXA.
4. Solo hay dos observaciones: en los demás años el reporte trae únicamente el índice oficial neto, que no permite separar el costo directo.

**Gastos (operación): 5.5% – 11.5%, central 9.0%**

1. Son los cuartiles 1 y 3 y la mediana de seis observaciones de la Tabla G4: 2.6%, 4.7%, 8%, 10%, 12% y 21.1%.
2. Uso cuartiles y no mínimo–máximo porque AXA pasa de 2.6% en 2024 a 21.1% en 2025, mientras su operación de Daños completo casi no cambia (5.6% a 5.7%). Podría ser un cambio en cómo AXA reparte gastos entre ramos; el reporte no lo confirma.
3. GNP se mueve entre 8% y 12% en tres años, y AXA 2023–2024 está entre 2.6% y 4.7%. El rango intercuartílico queda entre ambos grupos.

## Comparación con autos

RC gasta más que autos en operación (5.5%–11.5% frente a 4%–5.3%) y paga más comisiones y bonos (cerca de 15% frente a 7%–11%); la adquisición total es parecida (18%–25% frente a 21%–27%).

| Ramo y fuente                                | Adquisición neta ÷ emitida | Adquisición directa ÷ emitida | Comisiones y bonos ÷ emitida | Operación ÷ emitida | Combinado oficial |
| -------------------------------------------- | ---------------------------: | ------------------------------: | ----------------------------: | --------------------: | ----------------: |
| Autos, Quálitas 2025 (guía de la clase 12) |                        23.1% |                       Sin datos |                     Sin datos |                  5.3% |             94.1% |
| Autos, AXA Seguros 2025                      |                        20.9% |                           21.1% |                         11.2% |                  4.4% |            102.8% |
| Autos, GNP 2024                              |                        26.8% |                           26.5% |                          7.0% |                    4% |              102% |
| RC, AXA Seguros 2025                         |                        16.4% |                           24.7% |                         14.8% |                 21.1% |            101.1% |
| RC, GNP 2024                                 |                         2.4% |                           18.4% |                         14.6% |                   12% |               52% |

Lo que pudimos observar es que en el caso de RC es un ramo chico (en AXA 2025, 1,412 millones frente a 15,393 de autos), así que sus gastos de suscripción y atención se reparten en menos prima. Además, RC se coloca más por agentes y bonos, mientras que en autos pesa más el rubro "otros" (9.9% en AXA y 19.5% en GNP).
