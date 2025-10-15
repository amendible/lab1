#Editor de Mapas 2D en Godot

Herramienta para la creación de mapas 2D tipo *tile-based* para videojuegos.


---

##Objetivo general
Desarrollar una herramienta gráfica que permita a los usuarios **diseñar mapas tipo cuadrícula (tile-based)** para videojuegos 2D.  
El editor debe ser **visual, interactivo y modular**, permitiendo pintar y borrar tiles, con distintos tipos de terreno.

---

##Estado del proyecto

| Funcionalidad | Estado | Descripción |
|----------------|:------:|-------------|
| Dibujo de tiles | ✅ | Permite pintar tiles sobre una cuadrícula |
| Borrado de tiles | ✅ | Elimina tiles con clic derecho |
| Tipos de tile (césped, ladrillo, suelo) | ✅ | Tres tipos básicos implementados |
| Interfaz en Godot | ✅ | Interfaz funcional y limpia |
| Capas (fondo, objetos, colisiones) | ⏳ | En desarrollo |
| Guardado / Carga | ⏳ | Planeado con formato JSON |
| Undo / Redo | ✅ | Implementado |
| Exportación a prototipo de juego | ⏳ | Planeado |

---

## Instrucciones de uso

### Requisitos
- [Godot Engine 4.x](https://godotengine.org/download)
- Sistema operativo: **Windows**, **Linux** o **macOS**

### Ejecución
1. Clona o descarga el repositorio.
2. Abre la carpeta del proyecto en **Godot**.
3. Ejecuta la escena principal (`editor.tscn`).
4. Empieza a **dibujar y borrar tiles** con el mouse.

### Controles

| Acción | Descripción |
|--------|--------------|
| Click izquierdo | Pinta un tile del tipo seleccionado |
| Click derecho | Borra un tile |
| <img width="32" height="30" alt="image" src="https://github.com/user-attachments/assets/00f167a5-034e-4e1f-aa69-d33798c2a3f9" /> | Selecciona tile de suelo |
| <img width="33" height="31" alt="image" src="https://github.com/user-attachments/assets/9387d286-4239-4b28-9458-7bc1b62d2b3c" /> | Selecciona tile de césped |
| <img width="33" height="30" alt="image" src="https://github.com/user-attachments/assets/80e684f3-9810-46a3-9192-9b7e253b965a" /> | Selecciona tile de ladrillo |

---

## Interfaz general

> La interfaz está pensada para ser simple, clara y escalable.  
> En el futuro incluirá paneles de herramientas, capas y propiedades.

| Elemento | Descripción |
|-----------|--------------|
| **Área central** | Lienzo donde se dibuja el mapa |
| **Panel lateral** | Paleta de tiles y herramientas |
| **Barra superior (futuro)** | Menú de archivo, vista y ayuda |
| **Footer (futuro)** | Estado actual y mensajes del sistema |

**Ejemplo visual:**  
> Este es un ejemplo de mapa creado con el editor.

<div align="center">
  <img src="https://github.com/user-attachments/assets/cb3ce27d-de04-4f20-a352-d4d76e31f7b5" alt="Ejemplo mapa básico" width="700"/>
</div>


![animation](https://github.com/user-attachments/assets/66560d2e-4d77-4fc6-a3f0-4d47ab9d2da1)

---

## Estructura del proyecto

```text
editor-de-mapas/
│
├── assets/ # Recursos gráficos del editor
│ └── tiles/ # Imágenes de los distintos tipos de bloques
│ ├── cesped.png
│ ├── ladrillo.png
│ └── suelo.png
│
├── mapas/ # Archivos de mapas guardados (formato JSON)
│ └── mapa_guardado.json
│
├── src/ # Código fuente organizado por módulos
│ ├── io/ # Entrada/salida (guardar/cargar mapas)
│ │ └── SaveLoad.gd
│ ├── model/ # Datos del mapa y su representación lógica
│ │ └── MapData.gd
│ └── ui/ # Interfaz gráfica del editor
│ ├── editor.tscn
│ ├── editor.gd
│ └── tm_background.gd
│
└── icon.svg # Ícono del proyecto
```

---

## Próximos pasos

1. Implementar **capas** (fondo, objetos, colisiones).  
2. Añadir **herramientas** de selección, relleno y mover.  
3. Desarrollar **guardado/carga** en formato JSON.    
4. Agregar **exportación** para el prototipo de juego.  
5. Mejorar la **UI/UX** con zoom, scroll y vista previa.  

---

## Pruebas previstas
- Validar funcionamiento en mapas grandes (100x100 tiles).  
- Probar manejo de errores (tiles fuera de rango, archivos corruptos).  
- Optimizar el rendimiento al dibujar grandes áreas.

---

## Tecnologías utilizadas

- **Motor:** [Godot Engine 4.x](https://godotengine.org)  
- **Lenguaje:** GDScript  
- **Formato de recursos:** `.png`, `.tscn`, `.gd`, `.json` (planeado)

---
## Autores

**Juan Pablo Bustillo**  
**Andrés Santiago Mendible**  
**Keinerth De La Hoz**  
**Luis Castro Caro**  
**Alvaro Arias Useche**


**Universidad:** *[Universidad del Norte]*  
**Asignatura:** *[Estructura de datos]*  
**Año:** 2025  
**Docente:** *[DANIEL ROMERO MARTINEZ]*  

---

## 🏁 Licencia
Este proyecto fue desarrollado con fines **académicos**.  
El código puede reutilizarse y modificarse libremente con fines educativos.

---

> 💬 *“Construir herramientas es el primer paso para crear mundos.”*  
> — Proyecto Editor de Mapas 2D 🌍


