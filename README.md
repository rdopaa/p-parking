# 🅿️ P-Parking — Sistema de Gestión de Estacionamiento (Windows)

P-Parking es una aplicación de escritorio moderna para la operación diaria de un estacionamiento.  
Diseñada para trabajar con **rapidez y mínima fricción**, con tarjetas claras, acciones a un clic, modo oscuro por defecto y un flujo de trabajo optimizado tanto para teclado como para mouse.  

---
https://post.spmailtechn.com/f/a/Y1jcAKr9HlDdbQQLCof3jg~~/AAHBshA~/O7gJGZSayxLnAjdn-lscBtWhTGUcC7YK4qsvNO8kwR1wwHxLzx474ZCpZkTuOLQUkEE5hzW0E0DaJHZVfvfs0AnEQ2EMrF7DReML8vNzSS-cqH-d1JAccCnIgeREAD-bkO-3qxGX2Bnr87eiKc91jLusUK5bTTn5gx--9e7HNRrK8gRwu1yGIBYXlCsGi6IP
## ✨ Características principales

### 🚗 Entrada y salida en 1 clic
- Registro de **ENTRADA** con impresión opcional de ticket.  
- Registro de **SALIDA** con cálculo automático del monto y confirmación/edición del total.  
- Edición rápida de **piso, modelo y patente**.  

### 🗂️ Historial en tarjetas
- **Filtros** por piso, tipo, estado y orden.  
- **Búsqueda incremental** por patente (prefijo).  
- Botones rápidos: `Finalizar`, `Eliminar`, `Imprimir ticket`, `Editar piso/registro`.  
- “Cargar más” para listas largas.  

### ⚙️ Ajustes completos
- Impresora predeterminada y **auto-impresión** en entrada/salida.  
- Idioma: 🇪🇸 Español | 🇬🇧 Inglés.  
- **Tarifas y promociones** por tipo de vehículo (Auto, SUV, Camioneta, Facultad).  
- Configuración del ticket (título/dirección) con **vistas previas**.  
- **Estadísticas** con filtros rápidos (Hoy, Semana, Mes, Mes anterior) y exportación a CSV.  

### 💾 Persistencia y seguridad de datos
- Base de datos local: `estacionamiento.db` (SQLite).  
- **Auto-Backup** programable (`estacionamientobackup.db`) con notificación al completar.  
- Rescate automático desde backup si la DB activa está vacía.  

### 🖥️ Experiencia de escritorio pulida
- **Modo oscuro** por defecto y barra de título oscura (Windows 10/11).  
- Inicio maximizado y **instancia única** (si ya está abierta, trae la ventana al frente).  
- **Actualizaciones automáticas** con notificación y barra de progreso.  
- Compatible con **pantallas HiDPI** (DPI Awareness per-monitor v2).  

---

## 💰 Lógica de precios (Promociones)
- **Primera hora completa** (mínimo 1.0 h).  
- Hasta **12 h** → precio por hora con topes mínimos (por tipo) y opcional “promo 6 h”.  
- **12–24 h** → tarifa fija de 24 h.  
- **> 24 h** → múltiplos de 24 h (ceil).  
- **Redondeo limpio** a $500 (con empate hacia arriba).  

---

## 📥 Instalación
1. Descarga el instalador desde la sección de [**Releases**](../../releases) 👉 `Setup_P-Parking_x.y.z.exe`  
2. El instalador detecta instalaciones previas y actúa como **Actualizar**.  
3. Por defecto se instala en:  
4. Los datos (DB, backups, ajustes) se **conservan entre actualizaciones**.  

---

## 🖥️ Requisitos
- Windows **10/11 (x64)**  
- Impresora Termica compatible con Windows (para tickets)  

## ⌨️ Atajos útiles
- `F11` → Pantalla completa  
- `Escape` → Salir de pantalla completa  

---

## 🔄 Actualizaciones
- La app consulta un **feed remoto (GitHub)** y muestra una notificación si hay una versión nueva.  
- El instalador descarga/instala en modo silencioso y relanza la app automáticamente.  

---

## 📜 Licencia
[MIT](./LICENSE) © 2025 — FX DOPA SOFTWARE.  

---
