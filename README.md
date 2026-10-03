# Slayer Pong

Mi versión del Pong de 1972, en C++ con SDL2, para Introducción a la Programación en UADE. Le di una vuelta de terror: cada jugador elige un asesino clásico del cine (Freddy, Jason, Ghostface o Leatherface) y juega en su escenario.

*Pong remake in C++17 and SDL2 with a horror theme: PvP or vs AI, three difficulty levels, character and stage select, and match results saved to CSV.*

## Qué tiene

- **Dos modos**: contra otra persona en el mismo teclado, o contra la máquina.
- **Tres dificultades** para la IA: fácil, media y difícil.
- **Selección de personaje y escenario**, con un fondo distinto en cada pantalla del juego.
- **Partidas a 7 puntos o 2 minutos**. La pelota acelera con cada golpe hasta un tope.
- **Resultados guardados** en `resultados.csv` al terminar cada partida.
- Música y efectos con SDL_mixer.

## Controles

| Tecla | Acción |
|---|---|
| W / S | Jugador 1 |
| ↑ / ↓ | Jugador 2 |
| 1 / 2 / 3 | Dificultad |
| Enter | Confirmar |
| Esc | Volver |

## Cómo compilarlo

Necesitás `g++` con C++17 y las librerías SDL2, SDL2_image, SDL2_ttf y SDL2_mixer.

```bash
make
./pong
```

## Estructura

```
src/
├── main.cpp          loop principal
├── game.cpp/.h       estados, reglas, física de la pelota, IA
├── render.cpp        dibujo de cada pantalla
├── audio.cpp         música y efectos
└── csv_manager.cpp   guardado de resultados
```

---

Roman Gael Varela (RGV) · [romangaelvarela.online](https://romangaelvarela.online)
