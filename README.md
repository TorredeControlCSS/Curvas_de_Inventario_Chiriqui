# Curvas de Inventario — CEDIS CHIRIQUÍ CSS

Dashboard de inventario para el Centro de Distribución de Chiriquí.

## Configuración del Backend (Google Apps Script)

El frontend consume la siguiente API desplegada:

```
https://script.google.com/macros/s/AKfycbzx223zsutL3agQmJgrZY1IM3aG3GWxnpuPu0lSjgsdaLXXGoCm3Pn0C96xYgyXNY4L/exec
```

## Configuración del CONFIG en el Apps Script

Actualizar el objeto `CONFIG` en el backend con los IDs propios de Chiriquí:

```js
const CONFIG = {
  SPREADSHEET_ID: '← ID de la Google Sheet de Chiriquí',
  FOLDER_ID: '← ID de la carpeta Drive con archivos de inventario de Chiriquí',
  SHEET_NAME: 'SALMI',
  DATA_SHEET: 'Data',
  INDEX_SHEET: 'Index',
  VENC_SHEET: 'DataVenc',
  LEAD: 45, Z: 1.65, WINDOW: 90,
  F8_SPREADSHEET_ID: '← ID del libro F8 (CALENDARIO/RESERVAS/CONSUMOS_UE) de Chiriquí',
  CALENDARIO_SHEET: 'CALENDARIO',
  RESERVAS_SHEET: 'RESERVAS',
  CONSUMO_UE_SHEET: 'CONSUMOS_UE',
  RECEPCION_GRACE_DAYS: 7
};
```

## GitHub Pages

Activar GitHub Pages desde `Settings → Pages → Branch: main / root`.

La app estará disponible en: `https://torrdecontrolcss.github.io/Curvas_de_Inventario_Chiriqui/`
