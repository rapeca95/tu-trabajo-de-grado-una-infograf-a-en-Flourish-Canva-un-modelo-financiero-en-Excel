# Guía Flourish: Spotify - Visualización de Datos MBA CESA

## ¿Qué es Flourish?
Flourist (flourish.studio) es una herramienta gratuita de visualización de datos interactiva. Ideal para infografías con gráficas animadas y mapas.

---

## GRÁFICA 1: Crecimiento de Usuarios (Línea animada)
**Archivo:** `data/01_spotify_mau_crecimiento.csv`
**Tipo en Flourish:** Line, Bar and Pie → Line Chart

### Pasos:
1. Ir a flourish.studio → New Visualization → **Line, Bar and Pie**
2. Click en **Data** (pestaña superior)
3. Upload CSV: `01_spotify_mau_crecimiento.csv`
4. Configurar:
   - **Label column:** Año
   - **Value columns:** Usuarios_Activos_Mensuales_Millones, Suscriptores_Premium_Millones
5. En **Preview** → cambiar colores:
   - Línea MAU: `#1DB954` (verde Spotify)
   - Línea Premium: `#191414` (negro Spotify)
6. Título: **"De 75M a 678M: La explosión de Spotify 2015-2024"**
7. Activar animación: Settings → Animation → ON

---

## GRÁFICA 2: Ingresos vs Costos (Barras apiladas)
**Archivo:** `data/02_spotify_ingresos.csv`
**Tipo en Flourish:** Column Chart

### Pasos:
1. New Visualization → **Bar, Line and Pie** → Column Chart
2. Upload CSV: `02_spotify_ingresos.csv`
3. Configurar:
   - **X axis:** Año
   - **Bars:** Ingresos_Premium_Millones_USD, Ingresos_Publicidad_Millones_USD
   - **Stacked:** ON
4. Colores:
   - Premium: `#1DB954`
   - Publicidad: `#535353`
5. Agregar línea de Ganancia_Bruta como línea secundaria
6. Título: **"Modelo Freemium: Premium domina los ingresos de Spotify"**

---

## GRÁFICA 3: Cuota de Mercado (Donut Chart)
**Archivo:** `data/03_spotify_cuota_mercado.csv`
**Tipo en Flourish:** Pie Chart

### Pasos:
1. New Visualization → **Pie, Donut, Waffle**
2. Upload CSV: `03_spotify_cuota_mercado.csv`
3. Configurar:
   - **Label:** Plataforma
   - **Value:** Cuota_Mercado_Porcentaje
4. Tipo: **Donut** (más moderno)
5. Colores destacados:
   - Spotify: `#1DB954`
   - Apple Music: `#FC3C44`
   - Amazon: `#FF9900`
   - YouTube: `#FF0000`
   - Otros: `#535353`
6. Título: **"Spotify lidera con 31.7% del mercado global de streaming"**

---

## GRÁFICA 4: Mapa LATAM (Mapa de calor)
**Archivo:** `data/04_spotify_latam.csv`
**Tipo en Flourish:** Map → Projection Map

### Pasos:
1. New Visualization → **Projection Map**
2. Upload CSV: `04_spotify_latam.csv`
3. Configurar:
   - **Country:** Pais
   - **Value:** Usuarios_Millones_2024
   - **Region:** South America
4. Color scale: monocromático verde `#1DB954` (más oscuro = más usuarios)
5. Agregar tooltip: Pais + Usuarios + Top_Genero
6. Título: **"LATAM: Brasil y México lideran el mercado latino de Spotify"**

---

## GRÁFICA 5: Bar Chart Race - Artistas top
**Archivo:** `data/07_spotify_artistas_top_streams.csv`
**Tipo en Flourish:** Bar Chart Race

### Pasos:
1. New Visualization → **Bar Chart Race**
2. Upload CSV: `07_spotify_artistas_top_streams.csv`
3. Configurar:
   - **Label:** Artista
   - **Value:** Streams_Billones_Acumulados
   - **Color by:** Genero
4. Velocidad: Medium
5. Título: **"Los artistas más escuchados en la historia de Spotify"**

---

## GRÁFICA 6: Pago por Stream (Comparativa de plataformas)
**Archivo:** `data/03_spotify_cuota_mercado.csv`
**Tipo en Flourish:** Bar Chart horizontal

### Pasos:
1. New Visualization → **Bar Chart** → Horizontal
2. Usar columnas: Plataforma + Pago_Por_Stream_USD
3. Ordenar de mayor a menor
4. Destacar Spotify en `#1DB954`, el resto en `#535353`
5. Título: **"¿Cuánto paga cada plataforma por stream? La verdad detrás de las cifras"**

---

## GRÁFICA 7: Crecimiento de Podcasts
**Archivo:** `data/05_spotify_podcasts_crecimiento.csv`
**Tipo en Flourish:** Area Chart

### Pasos:
1. New Visualization → **Line Chart** → Area
2. Upload: `05_spotify_podcasts_crecimiento.csv`
3. Variables: Año + Podcasts_Millones + Oyentes_Podcast_Millones
4. Color área: `#1DB954` con transparencia 40%
5. Título: **"Spotify apuesta al audio: de 700K a 6M podcasts en 5 años"**

---

## Exportar desde Flourish
- Cada gráfica: **Export → PNG** (alta resolución para Canva)
- O usar el **link embed** para incluir en presentación interactiva
- Para la infografía en Canva: exportar como PNG 2x
