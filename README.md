<h1 align="center">📦 Gestión de Almacén</h1>
<h3 align="center">🎓 Proyecto Académico de 2do Año</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white" alt="Java"/>
  <img src="https://img.shields.io/badge/VS_Code-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white" alt="VS Code"/>
</p>

<div align="center">
  <img src="https://raw.githubusercontent.com/LachoCardenas44/GestionAlmacen.VisualParadigm/main/PreviewGestionAlmacen.jpg" alt="Diagrama UML General" width="600">
</div>

## 📄 Descripción
Aplicación de escritorio en Java diseñada para la administración intuitiva de almacenes. Permite gestionar el inventario de productos, coordinar al personal e intermediarios (clientes y proveedores), y llevar un control estructurado de envíos y pedidos.

---

## 👥 Roles y Funcionalidades

El sistema está diseñado para tres tipos de usuarios con flujos de trabajo específicos:

*   **🛠️ Administrador (Gestión Total):**
    *   Acceso exclusivo a la administración de su almacén.
    *   Gestiona el catálogo de **Agentes** (alta y baja de Clientes y Proveedores).
    *   Controla el **Stock** (registro, edición y eliminación de productos).
    *   Coordina los **Envíos** a clientes y confecciona nuevos **Pedidos** a los proveedores.
*   **🛒 Cliente (Consulta):**
    *   Explora los almacenes disponibles en el sistema.
    *   Visualiza el catálogo de productos (Stock) con sus tipos y precios.
    *   Consulta el estado de sus envíos (las solicitudes se realizan por vía externa con el Administrador).
*   **🚚 Proveedor (Validación):**
    *   Accede al listado de almacenes para revisar las órdenes de reabastecimiento.
    *   Consulta detalles de los pedidos (producto, cantidad, precio) y tiene la autoridad para **Validar** o cancelar dichas órdenes.

---

## 🧩 Arquitectura y Módulos

El proyecto está modularizado en dos bloques principales:

### Módulo 1: Operaciones y Logística
**Desarrollador:** [@LachoCardenas44](https://github.com/LachoCardenas44)
*   **Warehouse:** Gestión de datos de los almacenes (nombre, localización).
*   **Delivery:** Control de envíos (costos, destino, impuestos, descuentos).
*   **Order:** Administración de pedidos internos a proveedores (fechas, cantidades, estado).
<details>
  <summary><b>Ver Diagrama UML</b></summary>
  <img src="https://github.com/LachoCardenas44/GestionAlmacen.VisualParadigm/blob/main/modulos/moduloLachoCardenas44.jpg" alt="UML Módulo 1">
</details>

### Módulo 2: Usuarios e Inventario
**Desarrollador:** [@vmcalderingamez](https://github.com/vmcalderingamez)
*   **Actores (User, Agents, Admin, Client, Supplier):** Jerarquía de clases abstractas e interfaces que define los roles internos/externos y sus accesos al sistema.
*   **Inventario (Product, PhysicLocation):** Clases que estructuran los artículos, sus propiedades de negocio y su ubicación física exacta.
<details>
  <summary><b>Ver Diagrama UML</b></summary>
  <img src="https://github.com/LachoCardenas44/GestionAlmacen.VisualParadigm/blob/main/modulos/Modulo%20vmcalderingamez.jpg?raw=true" alt="UML Módulo 2">
</details>

---

## 💻 Autores

| <img src="https://avatars.githubusercontent.com/u/116188859?v=4" width="80"><br><sub>**Lázaro C. Cárdenas**</sub> | <img src="https://avatars.githubusercontent.com/u/109447884?v=4" width="80"><br><sub>**Víctor M. Calderín**</sub> |
| :---: | :---: |
| [LachoCardenas44](https://github.com/LachoCardenas44) | [vmcalderingamez](https://github.com/vmcalderingamez) |

---

## ⚖️ Licencia
Distribuido bajo la licencia **[Apache License](http://www.apache.org/licenses/)**.
