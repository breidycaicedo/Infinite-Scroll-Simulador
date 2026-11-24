# Infinite Scroll — Simulador de cadenas de Markov

Simulador 3D interactivo del proyecto final de **Matemáticas Aplicadas II** (Universidad Icesi). Modela cómo cambian las recomendaciones de un feed de videos entre tres categorías (Humor, Belleza y Educación) usando cadenas de Markov, y compara dos cuentas con patrones de interacción distintos.

**Ver el simulador:** https://breidycaicedo.github.io/Infinite-Scroll-Simulador/

## Qué muestra

- **Esferas:** los estados $H$, $B$ y $E$. Su tamaño es $x_n$, la probabilidad de que el video $n$ sea de esa categoría.
- **Tubos con flecha:** las probabilidades de transición $t_{ij}$ (de la categoría $j$ a la $i$). Más grueso = más probable.
- **Anillos:** $t_{jj}$, quedarse en la misma categoría.
- **Partículas:** el flujo de probabilidad $x_j \, t_{ij}$.
- **Celular:** el feed simulado, video por video, sorteado con la columna de $T$ del video actual.
- **Gráfica:** el modelo $x_n = T^n x_0$ contra la frecuencia observada en la simulación; ambos llegan al estado estacionario $\pi$.
- **Gauss-Jordan:** el estado estacionario resuelto paso a paso a partir de $(T - I)\pi = 0$ y $\pi_H + \pi_B + \pi_E = 1$.

## Cómo usarlo

| Acción | Botón o tecla |
|---|---|
| Scrollear / pausar | **Scrollear** o `Espacio` |
| Un video | **+1 video** o `→` |
| Cambiar de cuenta | **Cuenta A / Cuenta B** o `1` / `2` |
| Reiniciar | **Reiniciar** o `R` |
| Vista para proyectar | **Presentación** o `P` |
| Cargar las secuencias registradas | **Mis datos** |

En **Mis datos** se pega una sesión por renglón, con `H`, `B` o `E` por cada video en orden; el simulador cuenta las transiciones y calcula las matrices.

## Integrantes

Jennifer Bejarano · Breidy Caicedo · Alejandra Mora · Maria Isabel Varona
