# Calculadora web

Calculadora hecha con HTML, CSS y JavaScript puro, sin librerías.

**Demo:** https://sksan91g-jpg.github.io/Calculadora/

## Funciones

- Operaciones básicas, paréntesis y porcentaje
- Respeta la prioridad de operadores (`2+3*4` da `14`)
- Números negativos (`5*-2`) y decimales sin errores de redondeo (`0.1+0.2` da `0.3`)
- Continúa con el resultado anterior
- Historial de operaciones guardado en el navegador
- Modo claro y oscuro
- Funciona con el teclado del computador

## Cómo funciona el cálculo

No usa `eval()`. La expresión se valida y se divide en piezas (números y operadores permitidos), y luego un parser recursivo la resuelve respetando la prioridad. Si aparece cualquier carácter no permitido, muestra `Error` y no procesa nada.

## Seguridad

- Validación de la entrada antes de calcular
- El historial se dibuja con `textContent` y no con `innerHTML`, para evitar inyección de HTML
- El historial guardado se valida al cargarlo

## Cómo usarla

Abre el archivo `index.html` en cualquier navegador. No requiere instalación.

## Aprendizajes

Proyecto hecho para practicar JavaScript del lado del cliente: eventos, manipulación del DOM, validación con expresiones regulares y `localStorage`.