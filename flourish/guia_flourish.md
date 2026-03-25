# Guía Completa: Visualizaciones en Flourish
## One Direction – Infografía de Streaming

---

## ¿Qué es Flourish?

[Flourish](https://flourish.studio) es una plataforma online para crear visualizaciones de datos interactivas y animadas sin necesidad de programar. Es ideal para infografías académicas y periodísticas.

**Registro:** Ve a https://flourish.studio → crea cuenta gratuita (soporta proyectos públicos ilimitados).

---

## Visualización 1: Bar Chart Race – Evolución de Streams por Año

### Archivo de datos a usar
`data/streaming_por_plataforma_anual.csv`

### Pasos en Flourish

1. Haz clic en **"New visualization"**
2. Selecciona la plantilla **"Bar chart race"**
3. En la pestaña **Data**, haz clic en **"Upload data"** y sube `streaming_por_plataforma_anual.csv`
4. Configura las columnas:
   - **Label column:** `Año`
   - **Values:** selecciona `Spotify_M`, `YouTube_M`, `Apple_Music_M`, `Amazon_Music_M`, `Deezer_M`, `Tidal_M`
5. En la pestaña **Preview**, ajusta:
   - **Duration:** 8000ms (para una animación fluida de 8 segundos)
   - **Bars to show:** 6
   - **Title:** "Evolución de Streams de One Direction por Plataforma (2011–2024)"
6. En **Colours**, asigna:
   - Spotify → `#1DB954`
   - YouTube → `#FF0000`
   - Apple Music → `#FC3C44`
   - Amazon → `#25D1DA`
   - Deezer → `#EF5466`
   - Tidal → `#00FFFF`
7. Haz clic en **"Export & publish"** → copia el código iframe

### Código iframe de ejemplo
```html
<div class="flourish-embed flourish-bar-chart-race" data-src="visualisation/TU_ID">
  <script src="https://public.flourish.studio/resources/embed.js"></script>
</div>
```

---

## Visualización 2: Timeline Interactivo de la Carrera

### Archivo de datos a usar
`data/timeline_carrera.csv`

### Pasos en Flourish

1. Haz clic en **"New visualization"**
2. Selecciona la plantilla **"Timeline"** (en la sección Stories)
3. Sube `timeline_carrera.csv`
4. Mapea las columnas:
   - **Date:** `Año` + `Mes` (combina como columna fecha: `2010-07`)
   - **Title:** `Evento`
   - **Text:** `Descripcion_Detallada`
   - **Category:** `Categoria`
5. Habilita el filtro por **Categoria** para que el usuario pueda filtrar por:
   - Origen / Éxito Musical / Giras / Reconocimiento / Hito Digital / Pausa / Regreso
6. Colores sugeridos por categoría:
   - Origen → `#C8102E`
   - Éxito Musical → `#1DB954`
   - Giras → `#00AEEF`
   - Reconocimiento → `#FFD700`
   - Cambio/Pausa → `#FF6B35`
   - Tragedia → `#8888AA`

---

## Visualización 3: Mapa Mundial de Audiencia

### Archivo de datos a usar
`data/audiencia_global.csv`

### Pasos en Flourish

1. Selecciona la plantilla **"Projection map"**
2. Sube `audiencia_global.csv`
3. Configura:
   - **Region:** `Pais`
   - **Value (colour):** `Streams_M`
   - **Popup:** `Pais`, `Streams_M`, `Porcentaje`
4. Escala de color:
   - Mínimo → `#1a0a2e` (violeta oscuro)
   - Máximo → `#C8102E` (rojo UK)
5. Título: "Distribución Global de Oyentes – One Direction"

---

## Visualización 4: Comparación de Álbumes

### Archivo de datos a usar
`data/evolucion_albums.csv`

### Pasos en Flourish

1. Selecciona la plantilla **"Bar, line and pie charts"**
2. Sube `evolucion_albums.csv`
3. Tipo de gráfico: **Grouped bars**
4. Columnas:
   - **X axis:** `Album`
   - **Values:** `Ventas_Mundiales_M`, `Streams_Total_M` (escala doble)
5. Añade línea de tendencia para `Ingresos_M_USD`

---

## Visualización 5: Scatter Plot – Canciones por Streams y Año

### Archivo de datos a usar
`data/top_canciones_streaming.csv`

### Pasos en Flourish

1. Selecciona la plantilla **"Scatter"**
2. Configura:
   - **X:** `Año`
   - **Y:** `Streams_Spotify_M`
   - **Size:** `Total_Streams_M`
   - **Colour:** `Album`
   - **Label:** `Cancion`
3. Activa el modo **"Annotate"** para destacar "What Makes You Beautiful" y "Story of My Life"

---

## Exportar e Integrar en Canva

1. En Flourish: **"Export & publish"** → **"Publish"** → activa visibilidad pública
2. Copia el link o el código iframe
3. En Canva: usa el elemento **"Embed"** para pegar el iframe de Flourish
4. Ajusta el tamaño del frame al layout de tu presentación

---

## Consejos de Diseño en Flourish

| Aspecto | Recomendación |
|---------|--------------|
| Fuente | Use "Helvetica Neue" o "Inter" para consistencia con Canva |
| Fondo | `#0D0D1A` (oscuro) o `#FFFFFF` (claro) según tu plantilla Canva |
| Paleta | `#C8102E` (rojo UK), `#1DB954` (Spotify), `#00AEEF` (azul) |
| Animación | 6–10 segundos para gráficos de carrera; 0.3s para barras |
| Accesibilidad | Siempre añade tooltips con los valores exactos |

