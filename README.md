# One Direction: Infografía de Carrera en Streaming

Proyecto de infografía interactiva que visualiza la trayectoria musical del grupo de pop británico **One Direction** a través de datos de streaming en plataformas digitales (Spotify, Apple Music, YouTube).

## Herramientas Utilizadas

| Herramienta | Propósito |
|-------------|----------|
| **Flourish** | Gráficos interactivos de streaming por año, álbum y canción |
| **Canva** | Diseño visual de la infografía final y maquetación |

## Estructura del Proyecto

```
📁 data/                    # Datasets CSV listos para importar a Flourish
   ├── streaming_anual.csv        # Streams totales por año (2010–2024)
   ├── albumes_streams.csv        # Streams por álbum
   ├── top10_canciones.csv        # Top 10 canciones más escuchadas
   ├── plataformas_comparativa.csv # Comparativa entre plataformas
   └── carreras_solistas.csv      # Streams post-separación (carreras en solitario)
📁 flourish/                # Guías de configuración para Flourish
   ├── guia_visualizaciones.md    # Paso a paso para cada gráfico
   └── plantillas_config.md      # Configuración de colores y tipografía
📁 canva/                   # Recursos para el diseño en Canva
   ├── guia_diseno.md             # Guía de diseño de la infografía
   ├── paleta_colores.md          # Paleta de colores oficial del proyecto
   └── estructura_infografia.md   # Layout y secciones de la infografía
📁 assets/                  # Recursos gráficos
   └── notas_iconografia.md       # Iconos y recursos visuales sugeridos
```

## Secciones de la Infografía

1. **Portada** — Identidad visual del grupo y concepto
2. **Línea de Tiempo** — Hitos de la carrera (2010–2015)
3. **Evolución en Streaming** — Gráfico de líneas por año
4. **Discografía** — Comparativa de álbumes por streams
5. **Top 10 Canciones** — Ranking de las más escuchadas
6. **Plataformas** — Distribución entre Spotify, YouTube, Apple Music
7. **Legado** — Carreras solistas y herencia musical

## Cómo Usar los Datos

1. Descarga los archivos `.csv` de la carpeta `data/`
2. Accede a [Flourish](https://flourish.studio) y crea una cuenta gratuita
3. Sigue la guía en `flourish/guia_visualizaciones.md`
4. Exporta los gráficos como imágenes o iframes
5. Importa a [Canva](https://canva.com) siguiendo `canva/guia_diseno.md`

## Grupo: One Direction

- **Formación:** 2010 (The X Factor UK)
- **Integrantes:** Harry Styles, Niall Horan, Liam Payne, Louis Tomlinson, Zayn Malik
- **Discografía:** 5 álbumes de estudio (2011–2015)
- **Pausa:** Desde marzo 2016
- **Origen:** Múltiples ciudades del Reino Unido e Irlanda
