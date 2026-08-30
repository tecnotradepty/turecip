# 📱 Mobile Fix & Invoice Manager

Sistema ligero de gestión de reparaciones y facturación para talleres de celulares. Funciona sin servidores dedicados, alojado en GitHub Pages e integrado con Google Sheets.

## 🚀 Características Principales

1. **Panel de Administración (`index.html`)**
   - Registro de nuevas reparaciones e ingresos.
   - Generación automática de ID único por cliente/orden.
   - Modificación de estado del equipo en tiempo real.

2. **Módulo de Facturación e Impresión (`factura.html`)**
   - Formato optimizado para impresoras térmicas (80mm/58mm) o PDF estándar.
   - Pautas explícitas de garantía, términos y condiciones del servicio.
   - Canvas para firma digital del cliente al recibir o entregar el equipo.
   - Código QR o enlace directo generado a `consulta.html?id=ID_ORDEN`.

3. **Consulta de Estado Pública (`consulta.html`)**
   - Permite al cliente rastrear la reparación desde su propio celular usando el enlace de la factura.
   - Muestra el estado actual del dispositivo, detalles del trabajo y costos.

4. **Sin Costo de Hosting ni Base de Datos**
   - Frontend en HTML5, CSS y JavaScript.
   - Backend basado en API REST montada sobre Google Apps Script + Google Sheets.

## ⚙️ Configuración Rápida

1. Clona el repositorio.
2. Crea una hoja en Google Sheets con los encabezados correspondientes.
3. Despliega el script `script.gs` en Google Apps Script como **Web App** (Acceso: *Cualquier persona*).
4. Copia la URL del despliegue en `js/config.js`.
