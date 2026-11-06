# PulsoLab · Musicala

Aplicativo web de entrenamiento rítmico con **30 ejercicios interactivos** organizados por fundamentos, coordinación, subdivisiones, pulso interno y desafíos.

## Empezar

- Abre `index.html` en Chrome, Edge, Firefox o Safari. Necesita que el navegador permita el audio tras tocar «Comenzar misión».
- Para publicarlo, sube **todos los archivos de esta carpeta** a la raíz de un repositorio de GitHub Pages o a cualquier hosting de archivos estáticos.
- Si lo sirves en HTTPS, también se puede instalar como aplicación web y funcionar sin conexión después de la primera carga.

## Cómo jugar

1. Elige uno de los 30 ejercicios del catálogo.
2. Ajusta los BPM, la cantidad de compases y el volumen.
3. Presiona «Comenzar misión» y sigue la cuenta inicial.
4. Pulsa el botón central o la **barra espaciadora** para marcar un toque. En ejercicios de coordinación usa **A** para izquierda y **L** para derecha (también puedes tocar los botones laterales).
5. Al terminar, verás puntuación, precisión media, aciertos, toques extra y sugerencias.

**Puntuación:** 70 % depende de cuántos toques coinciden con el patrón, 30 % de la precisión de esos toques. Los toques extra restan 2 puntos. Ventana de acierto adaptable al espacio entre toques. Se considera misión completada desde 60 puntos (2 estrellas desde 65 puntos).

**Importante:** no es un instrumento de medición profesional: la latencia de los audífonos Bluetooth, dispositivos y navegadores puede afectar la precisión en milisegundos. Para entrenamiento preciso, mejor usar altavoces cableados o audífonos con cable. Las figuras rítmicas se generan por Web Audio API, sin archivos de audio externos.

## Estructura

- `index.html`: toda la interfaz, la lógica musical y el motor de ejercicios.
- `manifest.webmanifest`: instalación PWA.
- `sw.js`: caché para modo sin conexión.
- `icon.svg`, `icon-192.png`, `icon-512.png`: íconos de la aplicación.

## Privacidad

No hay cuentas, analíticas ni backend. Los mejores puntajes y la cantidad de prácticas se guardan en `localStorage`, dentro del navegador donde se usa la app. «Reiniciar progreso» elimina esos datos localmente.

© Musicala · Prototipo educativo independiente v1.0.
