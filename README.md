<div align="center">

# 🏍️ RUDOLF MOTOS — Plataforma Oficial Taller BAJAJ

**Sistema integral de gestión de taller, diagnóstico técnico por sistemas, business intelligence y CRM para Servicio Técnico Autorizado BAJAJ / Crosland Perú.**

[![Licencia](https://img.shields.io/badge/licencia-Propietario%20%2F%20Comercial-blue?style=for-the-badge)](LICENSE)
[![Estado](https://img.shields.io/badge/estado-Producción%20v2.4-emerald?style=for-the-badge)](https://github.com/)
[![BAJAJ](https://img.shields.io/badge/Servicio_Oficial-BAJAJ%20%2F%20Crosland-0052CC?style=for-the-badge&logo=motorcycle)](https://www.bajaj.pe)
[![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com)
[![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=for-the-badge&logo=chartdotjs&logoColor=white)](https://www.chartjs.org)

</div>

---

## 🏛️ Identidad & Respaldo Oficial
* **Concesionario:** RUDOLF MOTOS — Servicio Técnico Autorizado BAJAJ
* **RUC:** `10486946003`
* **Representante Legal:** Rodolfo Alfaro Huaman Huillca
* **Contacto / WhatsApp:** [+51 913 223 471](https://wa.me/51913223471)
* **Red Oficial:** Crosland Automotriz Perú / Bajaj Motorcycles
* **Modelos Homologados:** *Pulsar NS200, Pulsar N160, Dominar 400, Dominar 250, Boxer 150, Avenger 220 y Torito*.

---

## ⚡ Características Principales

### 📋 1. Hoja de Cálculo Interactiva (Grid Excel / Airtable)
- **Edición en celda:** Doble clic sobre Placa, Cliente, Modelo o Estado con guardado reactivo instantáneo.
- **Buscador en vivo:** Filtrado instantáneo por placa peruana (`5421-8B`), DNI, cliente o N° de orden.
- **Exportación masiva:** Descarga en 1 clic de reportes en **Microsoft Excel (.xlsx)** y **CSV** con SheetJS.
- **Totales en tiempo real:** Sumatorias automáticas de facturación, adelantos cobrados y saldos pendientes.

### 🔧 2. Orden Técnica Oficial de 7 Sistemas Clave
- Checklist estructurado idéntico a la cartilla física de taller:
  1. **Transmisión:** Cadena, piñón, embrague, corona.
  2. **Frenos:** Pastillas Bybre, discos, caliper, líquido DOT4, ABS.
  3. **Suspensión:** Horquilla telescópica, monoshock Nitrox.
  4. **Chasis:** Cunas de dirección, basculante, rodamientos.
  5. **Motor DTS-i:** Calibración de válvulas, afinamiento, aceite Motul.
  6. **Sistema Eléctrico:** Batería, bujías triple chispa, inyección EFI.
  7. **Servicios Terceros:** Torno, rectificación de discos y cilindro, pintura.
- **Liquidación financiera cuádruple:** Mano de obra + Repuestos Crosland + Terceros = Total (S/.) con cálculo de saldo y adelantos.
- **Lienzo de firmas táctiles HTML5 Canvas:** Firma digital del cliente y del mecánico jefe.
- **Impresión PDF:** Formato membretado listo para imprimir o enviar por WhatsApp.

### 📷 3. Motor OCR / Escáner Multimodal
- Escaneo de Tarjetas de Propiedad SUNARP y DNI mediante cámara o arrastre de imagen.
- Extracción local con **Tesseract.js** (sin costos de API externa).
- Autocompletado inteligente en 3 niveles: Historial Local → API K1.pe → OCR en Navegador.

### 📊 4. Dashboard BI & CRM de Fidelización
- **Evaluación Gerencial:** Facturación diaria, mensual y anual consolidada.
- **Productividad:** Rendimiento y volumen de motos atendidas por cada mecánico.
- **CRM WhatsApp:** Alertas automáticas a clientes para mantenimientos de 5,000 km y 10,000 km en 1 clic.

---

## 🛠️ Stack Tecnológico

| Capa | Tecnología |
| :--- | :--- |
| **Frontend** | HTML5 Semántico, Vanilla JavaScript (ES6+ modular) |
| **Estilos** | Tailwind CSS (Dark Cockpit Bajaj theme), Glassmorphism, CSS Custom Properties |
| **Visualización** | Chart.js 4.4 |
| **Motor OCR** | Tesseract.js v5 (procesamiento en cliente vía WebAssembly) |
| **Hojas de Cálculo** | SheetJS (xlsx v0.18.5) |
| **Persistencia** | IndexedDB v3 + LocalStorage con soporte Firebase Firestore |
| **Iconografía** | Lucide Icons |

---

## 🚀 Despliegue Rápido

### Opción 1: En Línea (Vercel / Netlify / GitHub Pages)
La plataforma no requiere compilación previa (Zero Build Step).

* **Vercel:** Sube el proyecto o conéctalo a este repositorio. Incluye `vercel.json` preconfigurado.
* **GitHub Pages:**
  1. Ve a **Settings** > **Pages** en tu repositorio de GitHub.
  2. En **Branch**, selecciona `main` y carpeta `/ (root)`.
  3. Guarda y accede en segundos a tu URL pública.

### Opción 2: Ejecución Local en Windows
Haz doble clic sobre el archivo ejecutable:
```cmd
start.bat
