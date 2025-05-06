<!-- ─────────────────────────────────────────────────────────────────────────────
     ┌────────────────────────────────────────────────────────────────────────┐
     │                       🖨️ Lista de Piezas 3D                          │
     └────────────────────────────────────────────────────────────────────────┘
────────────────────────────────────────────────────────────────────────────────
-->

## 📦 Piezas

> **Infill:** 100 % (relleno completo)

---

## 🔧 Ajustes de Impresión

EVA está diseñada para funcionar con boquillas de hasta **0.5 mm**, activando la detección de paredes finas en tu slicer si es necesario.  
Recomienda perímetros de **∼1 mm** (p.ej. 2 perímetros de 0.55 mm o 3 de 0.45 mm) para garantizar rigidez estructural.  
Un **15 % de infill** es suficiente para la mayoría de las piezas, salvo componentes críticos donde prefieras 100 %.

---

## 🔢 Cantidades y Componentes

| Nº  | Cantidad | Componente               | ¿Imprimible? | Crítico (100 % infill) |
|:---:|:--------:|:-------------------------|:------------:|:----------------------:|
| 1   | 1        | `back_core`              | ✅           | ✅                     |
| 2   | 1        | `front_universal_fi`     | ✅           | ✅                     |
| 3   | 2        | `core_xy_belt_grabber`   | ✅           | ✅                     |
| 4   | 2        | `face_belt_grabber`      | ✅           | ✅                     |
| 5   | 1        | `hotend_mosquito_fi`     | ✅           | ✅                     |
| 6   | 1        | `hotend_revo_voron_fi`   | ✅           | ✅                     |
| 7   | 1        | `drive_bmg`              | ✅           | ✅                     |
| 8   | 1        | `drive_lgx_lite`         | ✅           | ✅                     |
| 9   | 1        | `drive_orbiter_2.0_fi`   | ✅           | ✅                     |
| 10  | 1        | `bl_touch_mount`         | ✅           | ✅                     |
| 11  | 1        | `bl_touch_mount_volcano` | ✅           | ✅                     |
| 12  | 1        | `cable_guide`            | ✅           | ❌                     |
| 13  | 1        | `cable_guide_mount_fi`   | ✅           | ✅                     |
| 14  | 1        | `bottom_trihorns_fi`     | ✅           | ✅                     |
| 15  | 1        | `shroud_tank`            | ✅           | ❌                     |
| 16  | 1        | `top_endstop_mgn12c_fi`  | ✅           | ✅                     |

---

### 🔍 Notas Adicionales

- Todos los archivos STL siguen **snake_case** para facilitar su ubicación.  
- Para imprimir:  
  1. Descarga el `.stl` correspondiente.  
  2. Carga en tu slicer (Cura, PrusaSlicer…).  
  3. Ajusta orientaciones y escala según tus necesidades.  
  4. Configura **infill** e **perímetros** según las recomendaciones anteriores.  
- Si tus piezas requieren ensamblaje, consulta la sección <a href="https://main.eva-3d.page/heat_insert" target="_blank">🔧 Montaje</a>.

---

## 🧩 Componentes y Función

EVA se compone de cuatro grupos principales de piezas, cada uno con interfaces modulares:

### 1. Core 
- **Top**: interfaz MGN12 para el resto de EVA.  
- **Front**: interfaz universal para montajes de hotend.  
- **Bottom**: soporte con opción de conducto de ventilación.  
- **Back**: variantes según sistema de movimiento (Cartesian, CoreXY…).

### 2. Drive
Montaje del extrusor que encaja sobre las piezas “Top” y “Front”.

### 3. Hotend
Soporte y conducto para ventilador, se conecta al “Front” y guía el filamento.

### 4. Otros elementos  
- **Cooling Inlet**: para tu ventilador de capa, se acopla al “Back”.  
- **Cable Management**: guía y sujeción de cables en el carro.  
- **Bed Probe**: monta el sensor de nivelación en el “Front”.

---

## 📏 Longitudes de PTFE

Cada combinación de drive + hotend requiere un trozo de tubo PTFE de longitud específica; se obtiene sumando los valores de la BOM de tu drive y tu hotend (no cortes en dos piezas).  
**Ejemplo:** Nova = 39.65 mm hasta el “roof” del frontal; LGX = 20.8 mm → **60.45 mm** total (± 0.2 mm en la práctica).  
Para precisión, inserta el PTFE montado y córtalo a ras de la transición entre drive y hotend, ajustando cualquier exceso.

---

> _¿Alguna discrepancia en nombres, cantidades o propiedades? Por favor abre un _issue_ o envía un _pull request_._

---

*¡Gracias por utilizar EVA y felices impresiones! 🚀*  
