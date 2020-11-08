# TicTacToe. Requisitos Cliente/Servidor
Universo Santa Tecla  
[uSantaTecla@gmail.com](mailto:uSantaTecla@gmail.com)  
  
**Índice**

1. [Requisitos](#requisitos)  
2. [Vista de Casos de Uso](#vista-de-casos-de-uso)  
2.1. [Prototipo de Interfaz](#prototipo-de-interfaz)  
  
## Requisitos  

| * _Funcionalidad: **Básica + Undo/Redo**_<br/>  * _Interfaz: **Gráfica y Texto**_<br/>  * _Distribución: **Standalone + Client/Server**_<br/>  * _Persistencia: **No**_<br/> | ![TicTacToe](../docs/images/tictactoe.png) | 
| :------- | :------: |  

## Vista de Casos de Uso  

| Diagrama de Actores y Casos de Uso | Diagrama de Contexto |
|---|---|
| ![TicTacToe](./docs/diagrams/out/vistaCasosUso/actores.svg) | ![TicTacToe](./docs/diagrams/out/vistaCasosUso/contexto.svg) |  

### Prototipo de Interfaz  
  
```
--- TIC TAC TOE ---
Number of users [0-2] 1

----- Choose one option -----
1) Do a movement
1
-------------
| - | - | - | 
| - | - | - | 
| - | - | - | 
-------------
Enter a coordinate to put a token:
Row: 1
Column: 1
-------------
| X | - | - | 
| - | - | - | 
| - | - | - | 
-------------

----- Choose one option -----
1) Do a movement
2) Undo previous movement
1
-------------
| X | - | - | 
| - | - | - | 
| - | - | - | 
-------------
-------------
| X | - | - | 
| - | O | - | 
| - | - | - | 
-------------

----- Choose one option -----
1) Do a movement
2) Undo previous movement
1
-------------
| X | - | - | 
| - | O | - | 
| - | - | - | 
-------------
Enter a coordinate to put a token:
Row: 1
Column: 2
-------------
| X | X | - | 
| - | O | - | 
| - | - | - | 
-------------

----- Choose one option -----
1) Do a movement
2) Undo previous movement
2
-------------
| X | - | - | 
| - | O | - | 
| - | - | - | 
-------------

----- Choose one option -----
1) Do a movement
2) Undo previous movement
3) Redo previous movement
3
-------------
| X | X | - | 
| - | O | - | 
| - | - | - | 
-------------

----- Choose one option -----
1) Do a movement
2) Undo previous movement
1
-------------
| X | X | - | 
| - | O | - | 
| - | - | - | 
-------------
-------------
| X | X | - | 
| - | O | O | 
| - | - | - | 
-------------

----- Choose one option -----
1) Do a movement
2) Undo previous movement
2
-------------
| X | X | - | 
| - | O | - | 
| - | - | - | 
-------------

----- Choose one option -----
1) Do a movement
2) Undo previous movement
3) Redo previous movement
1
-------------
| X | X | - | 
| - | O | - | 
| - | - | - | 
-------------
-------------
| X | X | - | 
| - | O | - | 
| - | O | - | 
-------------

----- Choose one option -----
1) Do a movement
2) Undo previous movement
1
-------------
| X | X | - | 
| - | O | - | 
| - | O | - | 
-------------
Enter a coordinate to put a token:
Row: 1
Column: 3
-------------
| X | X | X | 
| - | O | - | 
| - | O | - | 
-------------
O Player: You win!!! :-)
Do you want to continue? (y/n):
```
