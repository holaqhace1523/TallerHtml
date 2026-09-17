# Registro de colaboración con IA

## Caso 1 — Sugerencia aceptada después de verificarla

### Herramienta
ChatGPT (GPT-5.6 Luna)

### Objetivo
Organizar las tarjetas de las motos utilizando Flexbox y hacer que fueran reutilizables.

### Prompt
Pregunté cómo aplicar Flexbox a las tarjetas de las diferentes categorías de motos y cómo hacer que se organizaran automáticamente.

### Respuesta obtenida
Se recomendó utilizar un contenedor `.cards` con `display: flex`, `gap` y `flex-wrap`, además de utilizar `flex: 1 1 280px` en `.card`.

### Evaluación
Probé la propuesta en Live Server. También cambié temporalmente el `gap` para comprobar el espacio entre tarjetas y aumenté el `flex-basis` a `500px` para verificar cuándo una tarjeta pasaba a la siguiente fila.

### Decisión
Acepté la sugerencia porque funcionó correctamente y cumplía con el requisito de Flexbox.

### Resultado
Las tarjetas de las categorías Deportivas, Scooter, Enduro y Naked quedaron dentro de contenedores `.cards` y se organizaron mediante Flexbox.

---

## Caso 2 — Sugerencia modificada

### Herramienta
ChatGPT (GPT-5.6 Luna)

### Objetivo
Organizar el menú y la sección principal de inicio para que ocuparan mejor el espacio horizontal.

### Prompt
Pregunté cómo organizar el menú y la sección "Descubre la moto de tus sueños" para que estuvieran en el mismo espacio horizontal.

### Respuesta obtenida
Se propuso utilizar Flexbox en `.inicio-contenedor` y distribuir el espacio utilizando propiedades como `flex` y `width`.

### Evaluación
Probé la propuesta visualmente en Live Server y observé que el resultado se podía mejorar para que la sección de inicio tuviera más espacio.

### Decisión
Modifiqué la propuesta en lugar de utilizarla exactamente como fue dada. Cambié la sección `#Inicio` para utilizar `width: 80%` y mantener el texto centrado.

### Resultado
El menú quedó ubicado a la izquierda y la sección principal ocupó una mayor parte del espacio disponible, manteniendo el contenido centrado.

---

## Caso 3 — Sugerencia rechazada por no ajustarse al requisito

### Herramienta
ChatGPT (GPT-5.6 Luna)

### Objetivo
Adaptar el diseño responsive para dispositivos pequeños.

### Prompt
Pregunté cómo aplicar el código responsive indicado en el ejercicio para que el sitio funcionara correctamente en diferentes tamaños de pantalla.

### Respuesta obtenida
El ejercicio mostraba un ejemplo utilizando `.hero` y `nav ul`, con reglas para modificar esos elementos mediante `@media`.

### Evaluación
Verifiqué mi HTML y observé que mi proyecto no utilizaba una clase `.hero` ni un `ul` dentro del `nav`. Mi estructura utilizaba directamente `#Inicio`, `nav` y enlaces `<a>`.

### Decisión
Rechacé aplicar esas reglas literalmente porque no correspondían a la estructura real de mi proyecto. En su lugar, utilicé `.cards` dentro del `@media` para adaptar las tarjetas.

### Resultado
Se agregó una regla responsive con `@media (max-width: 700px)` y `.cards { flex-direction: column; }`. Después se verificó el sitio a 1200 px, 768 px y 390 px, comprobando que no se perdiera contenido ni apareciera desbordamiento horizontal.