# GUIA: Cuál gráfica escoger en Flourish
## Spotify - MBA CESA | Las 7 gráficas con movimiento

---

## GRAFICA 1 - BAR CHART RACE (LA MAS IMPACTANTE)
**Archivo:** `GRAFICA1_bar_chart_race_artistas.csv`
**En Flourish busca:** `Bar chart race`

### Que hace:
Las barras CORREN y se reordenan solas mostrando quién lideró cada año.
Ves como Bad Bunny sube desde cero hasta ser el #1 mundial.

### Configuracion exacta en Flourish:
1. New visualization -> **Bar chart race**
2. Subir CSV
3. **Label** = columna `Artista`
4. **Values** = columnas de años: `2016, 2017, 2018... 2024`
5. **Color** = columna `Color` (ya tiene los colores hex)
6. Speed: **Medium**
7. Título: *"La carrera del streaming: ¿Quién dominó Spotify 2016-2024?"*

### Nivel de impacto: MAXIMO

---

## GRAFICA 2 - LINEA CON ANIMACION (CRECIMIENTO)
**Archivo:** `GRAFICA2_linea_animada_usuarios.csv`
**En Flourish busca:** `Line chart`

### Que hace:
Una línea que se dibuja sola de izquierda a derecha mostrando el crecimiento de Spotify.
Aparece una nota especial en 2020 (COVID).

### Configuracion exacta en Flourish:
1. New visualization -> **Line, Bar and Pie** -> Line
2. Subir CSV
3. **X axis** = columna `Año`
4. **Y values** = `Usuarios_Activos_Mensuales`, `Suscriptores_Premium`
5. **Labels** = columna `Hito` (aparece en los puntos clave)
6. Activar: Settings -> Animate on load -> ON
7. Color linea MAU: `#1DB954` | Color Premium: `#FFFFFF`
8. Fondo: `#191414` (negro Spotify)
9. Título: *"De 75M a 678M usuarios: Spotify no para de crecer"*

### Nivel de impacto: ALTO

---

## GRAFICA 3 - BURBUJAS ANIMADAS (MERCADO)
**Archivo:** `GRAFICA3_burbuja_mercado_streaming.csv`
**En Flourish busca:** `Scatter`

### Que hace:
Burbujas que cambian de tamaño y posicion por año.
Ves cómo Spotify crece mientras sus competidores luchan.

### Configuracion exacta en Flourish:
1. New visualization -> **Scatter**
2. Subir CSV
3. **X** = `Usuarios_Millones`
4. **Y** = `Ingresos_Millones_USD`
5. **Size** = `Cuota_Mercado_Pct`
6. **Name** = `Plataforma`
7. **Time** = `Año` (esto crea la animacion por tiempo)
8. **Color** = columna `Color`
9. Título: *"¿Quién gana la guerra del streaming? Usuarios vs Ingresos"*

### Nivel de impacto: MUY ALTO

---

## GRAFICA 4 - MAPA DE CALOR LATAM
**Archivo:** `GRAFICA4_mapa_latam_usuarios.csv`
**En Flourish busca:** `Projection map`

### Que hace:
Un mapa de América Latina donde cada país cambia de color según los usuarios.
Al pasar el mouse muestra el país, usuarios y género top.

### Configuracion exacta en Flourish:
1. New visualization -> **Projection map**
2. Subir CSV
3. **Region codes** = columna `id` (codigos de 3 letras: BRA, MEX...)
4. **Value** = `Usuarios_2024_M`
5. **Name** = `País`
6. Tooltip: activar `Top_Género` y `Crecimiento_Anual_Pct`
7. Color scale: **Single color** -> verde `#1DB954`
8. Zoom: America del Sur y Central
9. Título: *"LATAM: El mercado de streaming que Spotify no puede ignorar"*

### Nivel de impacto: ALTO

---

## GRAFICA 5 - SLOPE CHART (RANKING GENEROS)
**Archivo:** `GRAFICA5_slope_ranking_generos.csv`
**En Flourish busca:** `Slope chart` o `Bump chart`

### Que hace:
Lineas que suben y bajan mostrando como el Latin/Reggaeton escalo del puesto 4 al 3.
Muy visual para mostrar tendencias de géneros musicales.

### Configuracion exacta en Flourish:
1. New visualization -> **Slope chart** (buscar en templates)
2. Subir CSV
3. **Label** = `Género`
4. **Values** = columnas de años `2019, 2020... 2024`
5. **Color** = columna `Color`
6. Invertir eje Y (1 = arriba = #1 en ranking)
7. Título: *"El Latin conquista Spotify: ascenso imparable del reggaeton"*

### Nivel de impacto: ALTO

---

## GRAFICA 6 - SANKEY (FLUJO DE DINERO)
**Archivo:** `GRAFICA6_sankey_flujo_dinero.csv`
**En Flourish busca:** `Sankey`

### Que hace:
Flujos de dinero animados que muestran a dónde va cada dólar que pagas en Spotify.
Muy impactante para el análisis de negocio en MBA.

### Configuracion exacta en Flourish:
1. New visualization -> **Sankey diagram**
2. Subir CSV
3. **Source** = `Origen`
4. **Target** = `Destino`
5. **Value** = `Valor_Millones_USD`
6. Color: nodo Spotify en `#1DB954`, resto gris
7. Título: *"¿A dónde va tu suscripcion de $10.99? El flujo real del dinero"*

### Nivel de impacto: MUY ALTO (unico y diferenciador)

---

## GRAFICA 7 - COLUMNAS APILADAS ANIMADAS (INGRESOS)
**Archivo:** `GRAFICA7_columnas_ingresos_animado.csv`
**En Flourish busca:** `Bar chart` -> Column

### Que hace:
Columnas que crecen año a año mostrando cómo Spotify finalmente se volvió rentable en 2021.

### Configuracion exacta en Flourish:
1. New visualization -> **Bar, Line and Pie** -> Column
2. Subir CSV
3. **X** = `Año`
4. **Bars (stacked)** = `Ingresos_Premium_USD_M` + `Ingresos_Publicidad_USD_M`
5. **Line (secondary axis)** = `EBITDA_USD_M`
6. Colores: Premium `#1DB954`, Publicidad `#535353`
7. Linea EBITDA: roja `#EF4444` (negativo) -> verde `#1DB954` (positivo desde 2021)
8. Título: *"Spotify: 14 años para ser rentable. ¿Valió la pena?"*

### Nivel de impacto: ALTO

---

## ORDEN RECOMENDADO EN LA INFOGRAFIA

| Posicion | Grafica | Por que aqui |
|----------|---------|-------------|
| 1 | Linea usuarios (G2) | Abre con crecimiento historico |
| 2 | Burbujas mercado (G3) | Muestra el contexto competitivo |
| 3 | Mapa LATAM (G4) | Conecta con la region |
| 4 | Slope generos (G5) | Muestra tendencias de contenido |
| 5 | Sankey dinero (G6) | El mas academico para MBA |
| 6 | Columnas ingresos (G7) | Analisis financiero |
| 7 | **Bar Race artistas (G1)** | CIERRA con lo mas espectacular |

---

## COMO DESCARGAR LOS ARCHIVOS

1. Ir a GitHub -> carpeta `excel_graficas`
2. Click en el archivo CSV que necesitas
3. Click en boton **`Raw`**
4. Click derecho -> **Guardar pagina como** -> guardar como `.csv`
5. Abrir en Excel para verificar los datos
6. Subir directo a Flourish
