# Instrucciones para Compilar en macOS

Este es una copia de seguridad del proyecto preparada específicamente para generar el instalador de Mac (.dmg).

## Requisitos
1. Tener una computadora con **macOS**.
2. Tener **Node.js** instalado (versión 18 o superior recomendada).

## Pasos para generar el DMG

1. **Instalar dependencias** (si no lo hiciste antes):
   ```bash
   npm install
   ```

2. **Compilar la aplicación**:
   ```bash
   npm run electron:build:mac
   ```

## ¿Dónde está mi archivo?
Una vez que el comando termine, busca la carpeta llamada `dist-electron` (se creará automáticamente). Allí encontrarás el archivo **KinetiQ IPTV.dmg**.

## Notas sobre Seguridad (Gatekeeper)
Como esta app no está "firmada" con un certificado de desarrollador de Apple ($99/año), al abrir el DMG en otra Mac verás un aviso de seguridad.
**Solución:**
- Arrastra la app a Aplicaciones.
- Haz clic derecho sobre la app y selecciona "Abrir".
- Confirma que quieres abrirla.
