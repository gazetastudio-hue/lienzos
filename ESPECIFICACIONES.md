# LIENZOS — Especificaciones de generación · Gazeta Studio

**Objetivo:** completar el catálogo a 10 obras por colección (mínimo del brief: 10–15 fijas, 6–12 limitadas).
Este repositorio NO se despliega: es la fábrica de arte fuente. Las imágenes `art-*.jpg` que se suban aquí las integrará después el chat principal en gazeta-studio (recortes de impresión, Stripe, web).

## Reglas técnicas (OBLIGATORIAS en cada imagen)
1. **Una llamada de generación por obra.** Nunca collages, ni rejillas, ni varias obras en una imagen.
2. **Solo la obra** llenando todo el encuadre: plano frontal, sin marco, sin pared, sin mockup, sin firma.
3. **Cero texto, cero letras, cero números, cero marcas de agua** (en Pop Art también: sin onomatopeyas).
4. **Proporción:** la indicada por obra (2:3, 5:7, 4:5, 8:11 o 1:2 vertical). Genera al máximo de resolución disponible.
5. **Nombre EXACTO de archivo:** `art-<id>.jpg` (ej. `art-eclectic-6.jpg`). JPG calidad alta.
6. Iluminación uniforme, color fiel, sin viñetas ni degradados de cámara.
7. **Ritmo:** máximo 10 imágenes por turno (límite de la plataforma). Genera, sube, marca en ESTADO.md y empuja. Continúa en el siguiente turno con las siguientes 10.

## Flujo de trabajo del chat generador
1. Lee `ESTADO.md` y elige el siguiente lote de obras ☐ (respeta el orden: primero completar colecciones más vacías: dimension → ethereum → popart → textures → eclectic/nordic/bauhaus).
2. Genera las imágenes (máx. 10) siguiendo el prompt EXACTO de cada obra + el estilo de su colección + las reglas técnicas. Puedes usar como imagen de referencia la de su colección en `referencias/` para clavar el estilo.
3. `git add art-*.jpg ESTADO.md` → marca ✔ en la tabla → commit `batch: <ids del lote>` → push.
4. Repite en el siguiente turno hasta agotar la tabla. Al terminar: commit final `catalogo completo`.

## Estilo por colección

### ECLECTIC — 5 actuales → objetivo 10 (**faltan 5**)
Pintura contemporánea vibrante y maximalista: coral, ocre, verde azulado y vino; pincelada expresiva; sujetos con vida (mercados, azoteas, bodegones, figuras). Referencia: referencias/eclectic.jpg

### NORDIC — 5 actuales → objetivo 10 (**faltan 5**)
Minimalismo escandinavo sereno: azul polvo, gris perla, crema; mucho espacio negativo; lagos, abedules, dunas, niebla. Referencia: referencias/nordic.jpg

### BAUHAUS — 5 actuales → objetivo 10 (**faltan 5**)
Modernismo geométrico de 1920s: rojo, azul y amarillo primarios + negro sobre crema; círculos, arcos, retículas; color plano preciso. Referencia: referencias/bauhaus.jpg

### ETHEREUM — 4 actuales → objetivo 10 (**faltan 6**)
Futurista oscuro y lujoso: vidrio, humo y nebulosas sobre negro; vetas de luz dorada, turquesa o violeta; brillo y profundidad. Referencia: referencias/ethereum.jpg

### POP ART — 4 actuales → objetivo 10 (**faltan 6**)
Cómic pop: puntos de trama (halftone), contornos negros gruesos, colores planos vivos (fucsia, amarillo, cian, rojo). SIN letras ni onomatopeyas. Referencia: referencias/popart.jpg

### ABSTRACT DIMENSION — 3 actuales → objetivo 10 (**faltan 7**)
Relieve abstracto en capas: papel rasgado o yeso tallado con sombras reales suaves; salvia, crema, terracota y burdeos. Referencia: referencias/dimension.jpg

### TEXTURES (edición limitada) — 6 actuales → objetivo 10 (**faltan 4**)
Minimalismo táctil e íntimo del estudio: burdeos/vino + arena y crema; empaste visible, calma, composiciones sencillas. Son EDICIÓN LIMITADA de 20: merecen el doble de cuidado. Referencia: referencias/textures.jpg


## Prompts unitarios (usar TEXTUALMENTE, añadiendo solo lo que indiquen las reglas)

Cada entrada incluye el uso final que dará el chat principal (tamaño cliente, precio y edición) para que la imagen tenga sentido comercial: obra de «gran formato» = lado mayor ≥ 100 cm.


### ECLECTIC

**`eclectic-6` — «Mercado de flores»** · lienzo 140 × 100 cm (ratio 5:7) · 179 € · serie abierta (100) · gran formato: sí

> Vibrant eclectic painting of an overflowing flower-market bouquet wrapped in kraft paper, coral, ochre, teal and wine tones, bold expressive brushstrokes, contemporary maximalist style, artwork only, flat frontal view, no text

**`eclectic-7` — «La cocina roja»** · lienzo 50 × 40 cm (ratio 4:5) · 119 € · serie abierta (100) · gran formato: no

> Vibrant eclectic painting of a warm Mediterranean kitchen still life: tomatoes, ceramic pitcher, hanging peppers, saturated reds and ochres with teal accents, expressive painterly style, artwork only, flat frontal view, no text

**`eclectic-8` — «Danza de sombrillas»** · lienzo 100 × 150 cm (ratio 2:3) · 199 € · serie abierta (100) · gran formato: sí

> Vibrant eclectic painting of beach umbrellas seen from above dancing across warm sand, coral, terracotta, turquoise and cream, playful geometric abstraction, expressive brushwork, artwork only, flat frontal view, no text

**`eclectic-9` — «Jardín nocturno»** · lienzo 55 × 40 cm (ratio 8:11) · 89 € · serie abierta (100) · gran formato: no

> Vibrant eclectic painting of a garden at night, deep wine and indigo foliage with bursts of ochre flowers, moonlit highlights, expressive contemporary brushwork, artwork only, flat frontal view, no text

**`eclectic-10` — «El coleccionista»** · lienzo 150 × 75 cm (ratio 1:2) · 229 € · serie abierta (100) · gran formato: sí

> Vibrant eclectic painting of a collector's wall of small framed abstract pictures above a velvet sofa, layered gallery scene in coral, mustard, teal and wine, maximalist contemporary style, artwork only, flat frontal view, no text


### NORDIC

**`nordic-6` — «Marea baja»** · lienzo 140 × 100 cm (ratio 5:7) · 139 € · serie abierta (100) · gran formato: sí

> Minimalist nordic painting of wet sand at low tide with gentle receding foam lines, powder blue, pearl grey and warm off-white, vast negative space, serene Scandinavian atmosphere, artwork only, flat frontal view, no text

**`nordic-7` — «Hielo»** · lienzo 50 × 40 cm (ratio 4:5) · 79 € · serie abierta (100) · gran formato: no

> Minimalist nordic painting of a single floating ice shape on still pale water, soft grey-blue gradient, enormous calm negative space, subtle paper texture, artwork only, flat frontal view, no text

**`nordic-8` — «Campo de centeno»** · lienzo 100 × 150 cm (ratio 2:3) · 149 € · serie abierta (100) · gran formato: sí

> Minimalist nordic painting of a pale rye field in soft wind, muted sage and cream horizontal bands with one thin dark horizon line, airy Scandinavian minimalism, artwork only, flat frontal view, no text

**`nordic-9` — «Primer tren»** · lienzo 55 × 40 cm (ratio 8:11) · 79 € · serie abierta (100) · gran formato: no

> Minimalist nordic painting of a distant white train crossing a snowy plain, tiny black line on off-white and powder blue, quiet and poetic, huge negative space, artwork only, flat frontal view, no text

**`nordic-10` — «Ventana al fiordo»** · lienzo 150 × 75 cm (ratio 1:2) · 199 € · serie abierta (100) · gran formato: sí

> Minimalist nordic painting of a calm fjord seen through a tall bright window shape, layered pale blues and greys, serene geometric calm, Scandinavian minimalism, artwork only, flat frontal view, no text


### BAUHAUS

**`bauhaus-6` — «Contracomposición»** · lienzo 100 × 150 cm (ratio 2:3) · 189 € · serie abierta (100) · gran formato: sí

> Bauhaus geometric painting of asymmetric circles, diagonal black bars and primary red, blue and yellow planes balancing on cream, precise flat color, 1920s modernism, artwork only, flat frontal view, no text

**`bauhaus-7` — «Tres mástiles»** · lienzo 140 × 100 cm (ratio 5:7) · 169 € · serie abierta (100) · gran formato: sí

> Bauhaus geometric painting of three vertical masts with triangular sails in primary colors over thin black rigging lines on off-white, precise flat shapes, 1920s modernism, artwork only, flat frontal view, no text

**`bauhaus-8` — «Círculo roto»** · lienzo 50 × 40 cm (ratio 4:5) · 99 € · serie abierta (100) · gran formato: no

> Bauhaus geometric painting of one large red circle split by a black wedge with a small yellow quarter-circle offset, flat primary color on cream, 1920s modernism, artwork only, flat frontal view, no text

**`bauhaus-9` — «Escalera cromática»** · lienzo 55 × 40 cm (ratio 8:11) · 89 € · serie abierta (100) · gran formato: no

> Bauhaus geometric painting of stepped rectangles ascending like stairs in graded red, blue and yellow with thin black outlines, precise flat composition, 1920s modernism, artwork only, flat frontal view, no text

**`bauhaus-10` — «Metropolitano»** · lienzo 150 × 75 cm (ratio 1:2) · 199 € · serie abierta (100) · gran formato: sí

> Bauhaus geometric painting of a tall modernist city skyline of rectangles and arches in primary colors with black grid lines on cream, 1920s modernism, artwork only, flat frontal view, no text


### ETHEREUM

**`ethereum-5` — «Espejo líquido»** · lienzo 100 × 150 cm (ratio 2:3) · 289 € · serie abierta (100) · gran formato: sí

> Abstract dark futuristic artwork of a mirror-like liquid black surface reflecting thin veins of molten gold light, high gloss depth, luxurious digital aesthetic on deep black, artwork only, flat frontal view, no text

**`ethereum-6` — «Señal»** · lienzo 50 × 40 cm (ratio 4:5) · 129 € · serie abierta (100) · gran formato: no

> Abstract dark futuristic artwork of a single glowing teal light thread cutting through black smoke, minimal and precise, subtle glow gradient, artwork only, flat frontal view, no text

**`ethereum-7` — «Constelación»** · lienzo 140 × 100 cm (ratio 5:7) · 259 € · serie abierta (100) · gran formato: sí

> Abstract dark futuristic artwork of connected glowing nodes of silver and violet light floating in black space like a constellation, delicate glass filaments, artwork only, flat frontal view, no text

**`ethereum-8` — «Abismo dorado»** · lienzo 150 × 75 cm (ratio 1:2) · 199 € · serie abierta (100) · gran formato: sí

> Abstract dark futuristic artwork of a vertical golden abyss: layered black glass planes descending into a glowing amber depth, luxurious and dramatic, artwork only, flat frontal view, no text

**`ethereum-9` — «Latencia»** · lienzo 55 × 40 cm (ratio 8:11) · 119 € · serie abierta (100) · gran formato: no

> Abstract dark futuristic artwork of a paused heartbeat line of gold light across deep black brushed texture, minimal elegant, subtle glow, artwork only, flat frontal view, no text

**`ethereum-10` — «Núcleo»** · lienzo 165 × 120 cm (ratio 8:11) · 289 € · serie abierta (100) · gran formato: sí

> Abstract dark futuristic artwork of a luminous dark orb core surrounded by orbiting rings of smoky glass and teal energy, monumental and serene, artwork only, flat frontal view, no text


### POP ART

**`popart-5` — «Cóctel»** · lienzo 100 × 150 cm (ratio 2:3) · 149 € · serie abierta (100) · gran formato: sí

> Bold pop art painting of a giant retro cocktail glass with pink liquid, olive and striped straw, halftone dot shading, vivid fuchsia, yellow and cyan flat colors, thick black outlines, screen-print texture, artwork only, no text, no letters

**`popart-6` — «Patatas fritas»** · lienzo 50 × 40 cm (ratio 4:5) · 99 € · serie abierta (100) · gran formato: no

> Bold pop art painting of an overflowing red fries box with golden fries flying, halftone dots, thick black outlines, vivid flat colors on turquoise background, screen-print texture, artwork only, no text, no letters

**`popart-7` — «La estrella»** · lienzo 140 × 100 cm (ratio 5:7) · 169 € · serie abierta (100) · gran formato: sí

> Bold pop art painting of a smiling retro film star silhouette with sunglasses against a giant yellow starburst, halftone dots, hot pink and cyan flat colors, thick black outlines, artwork only, no text, no letters

**`popart-8` — «Burbujas»** · lienzo 55 × 40 cm (ratio 8:11) · 89 € · serie abierta (100) · gran formato: no

> Bold pop art painting of floating iridescent soap bubbles with halftone highlights over a pink and orange starburst background, thick black outlines, screen-print texture, artwork only, no text, no letters

**`popart-9` — «Casete»** · lienzo 150 × 75 cm (ratio 1:2) · 199 € · serie abierta (100) · gran formato: sí

> Bold pop art painting of a giant retro cassette tape with magenta and cyan labels rendered as pure shapes, halftone dots, thick black outlines, vivid flat colors, screen-print texture, artwork only, no text, no letters

**`popart-10` — «Sirena»** · lienzo 165 × 120 cm (ratio 8:11) · 189 € · serie abierta (100) · gran formato: sí

> Bold pop art painting of a comic-style mermaid with flowing teal hair and coral tail on a turquoise wave, halftone dot shading, thick black outlines, vivid flat colors, screen-print texture, artwork only, no text, no letters


### ABSTRACT DIMENSION

**`dimension-4` — «Estratos II»** · lienzo 100 × 150 cm (ratio 2:3) · 169 € · serie abierta (100) · gran formato: sí

> Abstract dimensional artwork of stacked torn-paper strata in charcoal, sand and burgundy casting soft real shadows, deep 3D relief illusion on warm off-white, artwork only, flat frontal view, no text

**`dimension-5` — «Plegado»** · lienzo 50 × 40 cm (ratio 4:5) · 99 € · serie abierta (100) · gran formato: no

> Abstract dimensional artwork of a single elegantly folded cream paper plane casting precise soft shadows over a sage background, minimalist relief, artwork only, flat frontal view, no text

**`dimension-6` — «Duna interior»** · lienzo 140 × 100 cm (ratio 5:7) · 189 € · serie abierta (100) · gran formato: sí

> Abstract dimensional artwork of carved plaster dunes in cream and terracotta with dramatic side light, tactile layered depth, warm minimalist composition, artwork only, flat frontal view, no text

**`dimension-7` — «Fronda»** · lienzo 55 × 40 cm (ratio 8:11) · 89 € · serie abierta (100) · gran formato: no

> Abstract dimensional artwork of a pressed fern leaf embossed in thick cream plaster, delicate real shadow, sage and warm neutrals, minimalist relief, artwork only, flat frontal view, no text

**`dimension-8` — «Marea de papel»** · lienzo 150 × 75 cm (ratio 1:2) · 199 € · serie abierta (100) · gran formato: sí

> Abstract dimensional artwork of undulating layered paper waves in graduated sand to burgundy tones, flowing relief with soft shadows, artwork only, flat frontal view, no text

**`dimension-9` — «Umbral»** · lienzo 60 × 90 cm (ratio 2:3) · 139 € · serie abierta (100) · gran formato: no

> Abstract dimensional artwork of a dark arched doorway shape raised in layered board over warm cream, mysterious soft shadow inside the arch, minimalist, artwork only, flat frontal view, no text

**`dimension-10` — «Vertedera»** · lienzo 165 × 120 cm (ratio 8:11) · 199 € · serie abierta (100) · gran formato: sí

> Abstract dimensional artwork of cascading geometric paper shards falling diagonally in charcoal, sage and burgundy with real soft shadows, dynamic relief composition, artwork only, flat frontal view, no text


### TEXTURES (edición limitada)

**`textures-7` — «Vena»** · lienzo 100 × 150 cm (ratio 2:3) · 289 € · edición limitada de 20 numeradas · gran formato: sí

> Intimate textured minimal painting of a single wine-red pigment vein crossing a field of thick sand-colored impasto strokes, tactile and calm, warm gallery aesthetic, artwork only, flat frontal view, no text

**`textures-8` — «Ceniza»** · lienzo 140 × 100 cm (ratio 5:7) · 259 € · edición limitada de 20 numeradas · gran formato: sí

> Intimate textured minimal painting of soft ash-grey and warm grey impasto bands with one thin burgundy line, tactile calm composition, artwork only, flat frontal view, no text

**`textures-9` — «Atardecer en yeso»** · lienzo 165 × 120 cm (ratio 8:11) · 299 € · edición limitada de 20 numeradas · gran formato: sí

> Intimate textured minimal painting of a setting sun as a raised burgundy semicircle over heavily textured cream plaster ground, warm and serene, artwork only, flat frontal view, no text

**`textures-10` — «Piel»** · lienzo 60 × 90 cm (ratio 2:3) · 189 € · edición limitada de 20 numeradas · gran formato: no

> Intimate textured minimal painting of close-up canvas skin in warm cream with dense wine-colored palette-knife strokes at the lower third, tactile and quiet, artwork only, flat frontal view, no text
