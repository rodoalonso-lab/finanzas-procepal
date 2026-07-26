# Finanzas — Procepal

Aplicación web progresiva (PWA) para el control financiero de obras: ingresos, gastos y presupuesto por obra, con reportes y estado de cuenta.

## Estructura

- `index.html` — aplicación completa (interfaz, lógica y estilos en un único archivo).
- `manifest.json` — manifiesto PWA (nombre, iconos, colores de tema).
- `sw.js` — service worker para caché offline de los recursos estáticos.
- `icon-192.png`, `icon-512.png` — iconos de la aplicación.

## Uso local

Al ser una PWA estática, no requiere build ni dependencias. Basta con servir la carpeta con cualquier servidor HTTP, por ejemplo:

```bash
npx serve .
```

o con Python:

```bash
python -m http.server 8000
```

Luego abre el navegador en la URL indicada por el servidor.

## Datos

La aplicación guarda su información en el almacenamiento local del navegador (`localStorage`), por lo que los datos persisten por dispositivo/navegador y no se sincronizan entre equipos.
