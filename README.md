# Simulación de Vehículo en Three.js

Este proyecto es una simulación 3D de un vehículo con forma de tanque utilizando **Three.js**. Incluye un vehículo controlable, obstáculos en el entorno y la capacidad de disparar proyectiles para destruirlos. El tanque tiene una torreta que rota independientemente del vehículo, un cañón ajustable y efectos de retroceso al disparar.

## Características

- **Control del Vehículo**: Mueve el vehículo usando las teclas `W`, `A`, `S` y `D`.
- **Rotación de la Torreta**: Usa las flechas `←` y `→` para rotar la torreta.
- **Disparo de Proyectiles**: Dispara usando la tecla `Espacio` para lanzar proyectiles en la dirección del cañón.
- **Colisión con Obstáculos**: Los proyectiles destruyen obstáculos al colisionar.
- **Efecto de Retroceso**: Al disparar, el tanque se mueve ligeramente hacia atrás simulando retroceso.

## Requisitos

- **Node.js** y **npm** deben estar instalados en tu sistema. Puedes descargarlos desde [Node.js](https://nodejs.org/).
- **Three.js**: La librería está incluida como módulo en el código del proyecto.


**Instala un Servidor Local** (opcional pero recomendado para manejar el módulo Three.js):
    ```
    npm install -g http-server
    ```

## Cómo Correr la Simulación

1. Si has instalado `http-server`, corre el servidor en el directorio raíz del proyecto:
    ```bash
    http-server .
    ```
    Luego, abre tu navegador y navega a `http://localhost:8080` (o el puerto que indique el servidor).

## Controles del Vehículo

- **Mover el vehículo**:
  - `W`: Avanzar
  - `S`: Retroceder
  - `A`: Mover a la izquierda
  - `D`: Mover a la derecha

- **Control de la torreta y disparo**:
  - `←` y `→`: Girar la torreta a izquierda/derecha
  - `Espacio`: Disparar proyectil

## Estructura del Código

- **Configuración de Three.js**: Inicializa la escena, cámara y renderizador.
- **Texturas**: Se aplican texturas al suelo y al vehículo, con un `TextureLoader`.
- **Iluminación**: Luz ambiental y direccional en la escena.
- **Vehículo**: Se crea un grupo de `vehicleGroup` con una base cilíndrica y una torreta esférica.
- **Proyectiles**: Se crean y se lanzan desde la posición del cañón con efectos de retroceso.
- **Obstáculos**: Obstáculos aleatorios en la escena con detección de colisiones.

## Dependencias

- **Three.js**: El proyecto incluye Three.js como módulo local en `three.module.js`.



