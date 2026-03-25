# Configuración de Estilos en Flourish

## Paleta de Colores del Proyecto

### Colores Principales (Identidad One Direction)

| Uso | Color | Hex | RGB |
|-----|-------|-----|-----|
| Primario (fondo oscuro) | Azul marino profundo | `#0A0E27` | 10, 14, 39 |
| Acento principal | Dorado brillante | `#FFD700` | 255, 215, 0 |
| Acento secundario | Azul eléctrico | `#4A90D9` | 74, 144, 217 |
| Spotify | Verde Spotify | `#1DB954` | 29, 185, 84 |
| YouTube | Rojo YouTube | `#FF0000` | 255, 0, 0 |
| Apple Music | Rosa Apple | `#FC3C44` | 252, 60, 68 |
| Texto claro | Blanco roto | `#F5F5F5` | 245, 245, 245 |
| Texto secundario | Gris plateado | `#B0B8C1` | 176, 184, 193 |

### Colores por Álbum

| Álbum | Color | Hex |
|-------|-------|-----|
| Up All Night | Azul celeste | `#87CEEB` |
| Take Me Home | Verde menta | `#98FF98` |
| Midnight Memories | Morado oscuro | `#6A0DAD` |
| Four | Rojo oscuro | `#8B0000` |
| Made in the A.M. | Naranja cálido | `#FF8C00` |

### Colores por Integrante (Carreras Solistas)

| Artista | Color | Hex |
|---------|-------|-----|
| Harry Styles | Rosa watermelon | `#FC6C85` |
| Niall Horan | Azul irlandés | `#1E90FF` |
| Liam Payne | Negro grafito | `#36454F` |
| Louis Tomlinson | Azul celeste | `#4169E1` |
| Zayn Malik | Morado real | `#7851A9` |

---

## Tipografía Recomendada en Flourish

- **Títulos:** Montserrat Bold o Raleway ExtraBold
- **Subtítulos:** Montserrat SemiBold
- **Datos/números:** Roboto Mono o Space Mono (para estética digital)
- **Cuerpo:** Open Sans Regular

**En Flourish:** `Settings > Typography` → Custom font → pegar nombre de Google Font

---

## Configuración General de Estilo

```
Fondo del gráfico:  #0A0E27  (azul marino)
Color de texto:     #F5F5F5  (blanco roto)
Color de grid:      #1A2040  (azul marino suave)
Borde/líneas:       #2A3060
Altura recomendada: 500px
Ancho recomendado:  800px
BorderRadius:       8px
```

---

## Plantilla de Tooltip

Para cada gráfico, configurar el tooltip con este formato HTML en Flourish:

```html
<b>{{Cancion}}</b><br>
Streams: <b>{{Streams_Spotify_Millones}}M</b><br>
Álbum: {{Album}} ({{Año}})
```
