# layoutwarehouse

https://nestum447.github.io/layoutwarehouse/

correo: todos@gmail.com

clave acceso publica: 123456

# 📦 Simulación de Bodega con Racks SL y SW

Aplicación web en **HTML + Firebase + JavaScript** para simular el estado de racks en una bodega.  
Permite visualizar, seleccionar y marcar ubicaciones en racks **SL** y **SW**, generar reportes y guardar estados en Firestore.

---

## ✨ Funcionalidades

- Visualización interactiva de racks **SL** y **SW**.  
- Selección de:
  - Racks completos
  - Filas
  - Ubicaciones individuales  
- Estados de ubicación:
  - ✅ Verde (ocupado / seleccionado)  
  - 🟧 Naranja (piso)  
  - ⚪ Gris (no seleccionado)  
- Dashboard con barras de progreso y totales.  
- Descarga de reporte en **Excel** (`.xlsx`).  
- Integración con **Firebase Authentication** y **Firestore**.

---

## 🔒 Permisos de acceso

La aplicación usa **Firebase Authentication** con dos modos de acceso:

1. **Admin (`ncarpio935@gmail.com`)**
   - Inicia sesión con correo y contraseña.
   - Puede **leer y escribir** en Firestore (guardar estados).
2. **Usuarios anónimos**
   - Se conectan automáticamente en **modo anónimo**.
   - Solo pueden **leer** información (modo solo lectura).
   - Pueden navegar y descargar reportes, pero **no guardar cambios**.

---

## ⚙️ Tecnologías utilizadas

- **HTML5 + CSS3** → estructura y estilos.  
- **JavaScript (Vanilla)** → lógica de la app.  
- **Firebase**  
  - Authentication (correo y anónimo).  
  - Firestore Database (almacenamiento de estados).  
- **SheetJS (XLSX)** → exportar datos a Excel.

---

## 🚀 Despliegue

La app puede desplegarse en:

- **Firebase Hosting**
- **GitHub Pages** (recomendado para visualización simple)

⚠️ Si usas GitHub Pages, la app se autentica automáticamente:
- Si puede usar las credenciales admin → entra con permisos de escritura.
- Si no → entra como usuario anónimo (solo lectura).

---

## 📂 Estructura del proyecto



---

## 🚀 Cómo usar

1. **Clona o descarga el repositorio**:

```bash
git clone https://github.com/nestum447/BodegaVisual.git
Abre index.html en cualquier navegador moderno (Chrome, Edge, Firefox) para probar localmente.

La aplicación muestra 15 racks con sub-ubicaciones clicables.

Los cuadros en rojo están ocupados y no se pueden seleccionar.

Los cuadros clicados se marcan en verde, indicando que están seleccionados.

Se muestra un contador global de sub-ubicaciones seleccionadas / no seleccionadas.

Se puede exportar la distribución completa a JSON con el botón "Exportar Distribución a JSON".
🎨 Personalización

Cambiar número de racks: totalRacks en el script de index.html.

Cambiar número de sub-ubicaciones por ubicación: subUbicaciones en el script.

Límite de selección por rack: maxSubPorRack.

Colores de ocupados y seleccionados: modificar las clases .ocupado y .seleccionado en el CSS.
