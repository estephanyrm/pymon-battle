# PyMon Battle

Simulador de batalla estilo Pokémon, jugado por consola, **1 jugador contra la máquina**. Proyecto en Python puro con arquitectura **MVC** (Modelo - Vista - Controlador) y clases abstractas para representar los distintos tipos de Pokémon.

## Estructura del proyecto

```
pymonBattle/
├── main.py           # Punto de entrada del programa
├── controlador.py     # Lógica del juego: turnos, elección de Pokémon, flujo de la partida
├── modelo.py           # Clases: Pokemon (abstracta), PokemonFuego, PokemonAgua, PokemonPlanta, Entrenador, Batalla
└── vista.py             # Presentación en consola: mensajes animados, barras de vida, validación de datos
```

## Requisitos previos

- **Python 3.8 o superior** — [descargar aquí](https://www.python.org/downloads/)

No se necesitan librerías externas: el proyecto solo usa módulos estándar de Python (`time`, `sys`, `random`, `abc`).

## Cómo correrlo

### 1. Clonar o descomprimir el proyecto

Ubícate en la carpeta raíz (`pymonBattle`).

### 2. Ejecutar el juego

```bash
python main.py
```

En algunos sistemas (Linux/macOS) el comando puede ser `python3` en vez de `python`:

```bash
python3 main.py
```

## Cómo se juega

1. Al iniciar, se te muestra tu equipo de 3 Pokémon: **Charmander** (Fuego), **Bulbasaur** (Planta) y **Squirtle** (Agua).
2. Escribes el número del Pokémon que quieres elegir para la batalla.
3. La máquina elige uno de su equipo (**Chikorita**, **Cyndaquil**, **Totodile**) de forma aleatoria.
4. La batalla avanza por turnos, con mensajes animados en consola y barras de vida.
5. Gana quien deje sin vida al Pokémon del rival.

Todo el juego es interactivo: solo sigue las instrucciones que aparecen en la terminal.

