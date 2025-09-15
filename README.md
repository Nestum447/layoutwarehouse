# layoutwarehouse
# Bodega Visual Interactiva - 15 Racks

Esta es una aplicación web interactiva que simula la **distribución de una bodega** con 15 racks, cada uno con:

- **23 columnas** (A → W)  
- **6 niveles** (1 → 6)  
- **3 sub-ubicaciones por ubicación**  

La aplicación permite **seleccionar sub-ubicaciones**, ver el **total de seleccionadas/no seleccionadas**, y **exportar la distribución a JSON**.

---

## 📂 Archivos del repositorio

- `index.html` → Archivo principal de la aplicación (cargará automáticamente en GitHub Pages).  
- `README.md` → Este archivo con instrucciones.  
- `assets/` (opcional) → Para CSS o imágenes adicionales si quieres personalizar la visualización.

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
