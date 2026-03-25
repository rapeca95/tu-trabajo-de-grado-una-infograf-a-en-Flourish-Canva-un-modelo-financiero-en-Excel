# Guía de Visualizaciones en Flourish

## One Direction — Infografía de Streaming

---

## Visualización 1: Línea de Tiempo de Streams por Año
**Tipo:** Line Chart  
**Archivo CSV:** `data/streaming_anual.csv`

### Pasos en Flourish:
1. Ir a `New Visualization` → seleccionar **Line, Bar, Pie**
2. Subir `streaming_anual.csv`
3. Configurar:
   - **X axis:** columna `Año`
   - **Y values:** `Streams_Spotify_Millones`, `Streams_YouTube_Millones`, `Streams_AppleMusic_Millones`
   - **Labels:** activar en puntos clave (2013 pico, 2016 pausa, 2024 tributo)
4. En **Annotations** → añadir texto en:
   - 2013: *"Midnight Memories #1 Global"*
   - 2015: *"Zayn se va"*
   - 2016: *"Pausa oficial"*
   - 2024: *"Tributo Liam Payne"*
5. Paleta de colores: ver `plantillas_config.md`

---

## Visualización 2: Ranking de Álbumes por Streams
**Tipo:** Bar Chart Race o Bar Chart horizontal  
**Archivo CSV:** `data/albumes_streams.csv`

### Pasos en Flourish:
1. `New Visualization` → **Bar Chart Race** (para efecto animado) o **Bar, Line and Pie** modo horizontal
2. Subir `albumes_streams.csv`
3. Configurar:
   - **Labels:** columna `Album`
   - **Values:** `Streams_Spotify_Millones`
   - **Color by:** columna `Año_Lanzamiento`
4. Ordenar de mayor a menor
5. Añadir imagen de portada de cada álbum en columna de iconos (opcional con URL)

---

## Visualización 3: Top 10 Canciones
**Tipo:** Bar Chart horizontal (Lollipop)
**Archivo CSV:** `data/top10_canciones.csv`

### Pasos en Flourish:
1. `New Visualization` → **Bar, Line and Pie** → modo **Lollipop**
2. Subir `top10_canciones.csv`
3. Configurar:
   - **Labels:** `Cancion`
   - **Values:** `Streams_Spotify_Millones`
   - **Color:** una tonalidad por álbum (`Album`)
4. Ordenar descendente por streams
5. Activar **tooltips** con: `Album`, `Año`, `Pico_Charts_Global`

---

## Visualización 4: Comparativa de Plataformas
**Tipo:** Stacked Area Chart  
**Archivo CSV:** `data/plataformas_comparativa.csv`

### Pasos en Flourish:
1. `New Visualization` → **Line, Bar, Pie** → tipo **Area**
2. Subir `plataformas_comparativa.csv`
3. Configurar modo **Stacked** para ver el total acumulado
4. Usar colores de cada plataforma (columna `Color_Hex`):
   - Spotify: `#1DB954`
   - YouTube: `#FF0000`
   - Apple Music: `#FC3C44`

---

## Visualización 5: Carreras Solistas — Spider/Radar Chart
**Tipo:** Radar / Spider Chart  
**Archivo CSV:** `data/carreras_solistas.csv`

### Pasos en Flourish:
1. `New Visualization` → buscar **Radar** en la galería
2. Subir `carreras_solistas.csv`
3. Variables a comparar:
   - Streams mensuales
   - Total catálogo
   - Seguidores Spotify
4. Un color distinto por artista
5. Título: *"¿Quién triunfó más en solitario?"*

---

## Visualización 6: Línea de Tiempo Interactiva
**Tipo:** Timeline  
**Archivo CSV:** `data/hitos_timeline.csv`

### Pasos en Flourish:
1. `New Visualization` → **Timeline**
2. Subir `hitos_timeline.csv`
3. Configurar:
   - **Date:** columna `Fecha`
   - **Text:** columna `Evento`
   - **Category/Color:** columna `Categoria`
4. Categorías y colores sugeridos:
   - Origen: `#4A90D9`
   - Discografía: `#7B68EE`
   - Giras: `#50C878`
   - Pausa: `#FF6B6B`
   - Legado: `#FFD700`

---

## Exportar Visualizaciones

1. **Embed (iframe):** para incrustar en web — botón `Export & publish` → `Publish` → copiar iframe
2. **Imagen PNG/SVG:** botón `Export & publish` → `Download image` (plan de pago)
3. **Captura de pantalla:** usar herramienta del sistema para captura de alta resolución

> **Tip:** Con cuenta gratuita de Flourish puedes publicar visualizaciones públicas y copiar la URL para incrustarlas en Canva mediante el elemento "Embed".
