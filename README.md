# LicenTrack

## 🎯 Objetivo

LicenTrack es una aplicación de escritorio desarrollada en C++ para la gestión de licencias de software en entornos empresariales. Permite registrar productos licenciados, asignar licencias a usuarios, controlar vencimientos, gestionar renovaciones y generar reportes.

Este proyecto se desarrolla como parte del trabajo integrador final de la asignatura, incluyendo todos los temas del programa: punteros, memoria dinámica, POO, relaciones entre clases, sobrecarga de operadores, flujos de I/O (texto y binario), programación genérica, STL e interfaces gráficas.

---

## 🧱 Estructura de clases

- `ProductoSoftware`: contiene datos como nombre, versión, proveedor y tipo de licencia.
- `Licencia`: incluye ID, fechas de compra/vencimiento, clave de activación, estado, y referencia al producto correspondiente.
- `Usuario`: representa a un empleado o área interna. Puede tener múltiples licencias asignadas.
- `GestorLicencias`: clase central que administra productos, licencias y usuarios. Permite buscar, asignar, validar vencimientos, generar reportes, y manejar la persistencia.

---

## 🔄 Relaciones entre clases

- Un producto puede tener múltiples licencias asociadas.
- Una licencia puede estar asignada a un único usuario a la vez.
- Un usuario puede tener varias licencias.

---

## 💾 Persistencia

- **Archivos binarios**: almacenamiento de licencias, productos y usuarios.
- **Archivos de texto**: generación de reportes (por ejemplo, licencias próximas a vencer).

---

## 🧠 Temas del programa integrados

| Tema                         | Aplicación                                                                 |
|-----------------------------|----------------------------------------------------------------------------|
| Punteros y memoria dinámica | Relaciones entre objetos (`Licencia*`, `Usuario*`)                         |
| Programación orientada a objetos | Diseño modular y reutilizable con clases definidas                       |
| Relaciones entre clases     | Asociación entre productos, licencias y usuarios                           |
| Sobrecarga de operadores    | Comparación por fecha de vencimiento, impresión con `<<`                   |
| Flujos de I/O               | Guardado binario y exportación de reportes en texto                        |
| Programación genérica       | Validaciones y estructuras parametrizadas                                  |
| Biblioteca STL              | Uso de `vector`, `map`, `set`, `algorithm` y otras utilidades             |
| Interfaces gráficas         | Interfaz visual desarrollada con Qt, SFML o wxWidgets                      |

---

## 🖥️ Funcionalidades de la interfaz gráfica

- Visualización y gestión de productos, licencias y usuarios
- Filtros por estado: activo, vencido, asignado
- Formularios para alta de productos y licencias
- Buscador por nombre o ID
- Exportación de reportes a archivo de texto
- Alertas visuales por vencimientos próximos

---

## 🌟 Funcionalidades adicionales (opcional)

- Validación automática de vencimientos al iniciar la aplicación
- Estadísticas por departamento o usuario
- Logs de acciones y modificaciones
- Alertas visuales y/o sonoras

---

## 🛠️ Tecnologías

- Lenguaje: C++
- Librerías: STL, Qt / SFML / wxWidgets (para GUI)
- Entrada/Salida: archivos binarios y de texto

