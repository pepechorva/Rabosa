# 🐭 Rabosa - Micromouse Autónomo de Competición

Rabosa es un proyecto de código abierto para construir un robot micromouse autónomo de competición. Está fuertemente inspirado en el esquemático y la forma de la PCB del micromouse **Green Giant 5.19V** de Green Ye.

El objetivo es diseñar una plataforma robusta y de alto rendimiento capaz de navegar y resolver laberintos en el menor tiempo posible.

## 🛠️ Especificaciones Técnicas

| Componente  | Detalle  |
|---|---|
|  Microcontrolador | STM32F405RGTx (24 MHz)  |
| Dimensiones  | 100,93 mm x 75 mm  |
| Motores  | Coreless 2085  |

## Estado del Proyecto

**Actualmente en desarrollo.** La parte electrónica está diseñada y esperando revisiones finales. Queda trabajo pendiente en el diseño 3D y el firmware.

## Clonar el Repositorio

El repositorio está separado en 3 partes (submódulos) para gestionar las versiones de PCB, diseño 3D y Firmware por separado. Para clonar todo el repositorio, ejecuta el siguiente comando en tu terminal:

git clone --recurse-submodules git@github.com:pepechorva/Rabosa.git



## 📸 Vistas Previas del Diseño

Aquí puedes ver algunas imágenes del estado actual del diseño de la PCB y los componentes:

<img width="685" height="922" alt="Esquemático de la PCB de Rabosa, vista superior" src="https://github.com/user-attachments/assets/7e1ea981-de4f-4501-8f45-65a42df3637f" />
<img width="651" height="654" alt="Vista del ensamblaje 3D de Rabosa" src="https://github.com/user-attachments/assets/a608ac0a-43a4-47ca-90c2-ecb36d8a4ee2" />
<img width="1280" height="720" alt="Vista detallada de la PCB y sus componentes" src="https://github.com/user-attachments/assets/cb139614-63b8-4b67-9694-13987a6bef82" />

## ⚙️ Estructura del Repositorio y Licencias


| Carpeta   |      Contenido      |  Licencia Aplicable |
|----------|:-------------:|------:|
| Hardware/ |Archivos de diseño electrónico (KiCad PCB y Esquemáticos) |CERN-OHL-S v2 (Fuerte)|
|Firmware/ | Código fuente del microcontrolador (STM32) | GNU GPL v3 |
| Mechanical/ | Modelos 3D, ensamblajes y archivos de FreeCAD | CERN-OHL-S v2 (Fuerte) |
| Docs/ | Documentación, hojas de datos y reportes. | Licencia Abierta (Creative Commons) |

## 🔗 Cómo Empezar: Configuración de Librerías

Para que el proyecto funcione sin errores de huellas/símbolos faltantes necesitas importar un repositorio de símbolos y huellas personalizadas referenciadas.

### 1. Clonar el Repositorio de Librerías

Clona el repositorio que contiene todas las huellas y símbolos personalizados:

git clone [https://github.com/pepechorva/KiCAD_github/KiCAD_libs.git](https://github.com/pepechorva/KiCAD_github/KiCAD_libs.git) 

### 2. Definir la Variable de Entorno en KiCad

Una vez clonado, abre KiCad (la ventana principal del gestor de proyectos):

Preferencias > Configurar Rutas...

Añade una nueva entrada con el siguiente nombre y ruta:

**variable**: KICAD_PEPECHORVA_GITHUB_LIBS **Ruta**: [PATH]/KiCAD_github/KiCAD_libs


## 📜 Licenciamiento

**Hardware y Diseño Mecánico:**
El diseño de la PCB, los esquemáticos y los archivos mecánicos están licenciados bajo la **CERN Open Hardware Licence v2 - Strong (CERN-OHL-S)**. Esto asegura que todas las modificaciones y distribuciones se mantengan bajo la misma licencia Open Source.

Consulte el archivo LICENSE para más detalles.

**Firmware y Software:**
El código que corre en el microcontrolador está licenciado bajo la **GNU General Public License v3 (GPLv3)**.

Consulte el archivo Firmware/LICENSE para más detalles.


