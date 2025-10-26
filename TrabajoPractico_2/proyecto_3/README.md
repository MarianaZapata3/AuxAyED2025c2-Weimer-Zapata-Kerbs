# Proyecto “Palomas Mensajeras”
📖 Descripción General

Este proyecto modela el sistema de comunicación por palomas mensajeras entre distintas aldeas, con el objetivo de encontrar la forma más eficiente de enviar un mensaje desde la aldea central “Peligros” hacia todas las demás aldeas del reino.

Cada aldea cuenta con un palomar propio y puede enviar mensajes únicamente a sus aldeas vecinas (aquellas conectadas por rutas directas).
El archivo aldeas.txt contiene la lista de aldeas y las distancias en leguas entre cada par conectado.

El sistema busca minimizar el total de distancias recorridas por las palomas, garantizando que:

Cada aldea reciba la noticia una sola vez.

Una vez que una aldea recibe la noticia, puede replicarla y enviarla a sus vecinas.

Desde “Peligros” parten inicialmente una o más palomas.
---
## 🏗 Funcionalidad
El programa:

Lee los datos de las aldeas y las distancias desde data/aldeas.txt.

Crea un grafo no dirigido y ponderado donde los vértices son aldeas y las aristas representan rutas posibles.

Aplica un algoritmo de Árbol de Expansión Mínima (MST), como Kruskal, para encontrar la forma más eficiente de conectar todas las aldeas con la mínima distancia total.

Determina:

La aldea de origen (“Peligros”).

Para cada aldea, de qué vecina recibe la noticia.

A qué vecinas envía la noticia una vez recibida.

Muestra:

La lista de aldeas ordenadas alfabéticamente.

La suma total de distancias recorridas por todas las palomas.
---
## 📑Dependencias

1. **Python 3.x**
2. **matplotlib** (`pip install matplotlib`)
3. listar dependencias principales
4. Dependencias listadas en requierements.txt

---
## 🚀Cómo Ejecutar el Proyecto
1. **Clonar o descargar** el repositorio.

2. **Crear y activar** un entorno virtual.

3. **Instalar las dependencias**:
   ```bash
   pip install -r requirements.txt
   ```
   El archivo `requirements.txt` se encuentran en la carpeta [deps](./deps) del proyecto.

---
## 🙎‍♀️🙎‍♂️Autores

- Zapata Mariana Gabriela 
- Weimer Valentin
- Kerbs Javier

---

> **Consejo**: Mantén el README **actualizado** conforme evoluciona el proyecto, y elimina (o añade) secciones según necesites. Esta plantilla es sólo un punto de partida general.
