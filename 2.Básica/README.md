# TicTacToe. Requisitos Básica
Universo Santa Tecla  
[uSantaTecla@gmail.com](mailto:uSantaTecla@gmail.com)  
  
**Índice**

1. [Requisitos](#requisitos)  
2. [Vista de Casos de Uso](#vista-de-casos-de-uso)  
2.1. [Prototipo de Interfaz](#prototipo-de-interfaz)  
2.1.1. [Número de jugadores: 0](#número-de-jugadores-0)  
2.1.1. [Número de jugadores: 1](#número-de-jugadores-1)  
2.1.1. [Número de jugadores: 2](#número-de-jugadores-2)  
  
## Requisitos  

| * _Funcionalidad: **Básica**_<br/>  * _Interfaz: **Texto**_<br/>  * _Distribución: **Standalone**_<br/>  * _Persistencia: **No**_<br/> | ![TicTacToe](../docs/images/tictactoe.png) | 
| :------- | :------: |  

## Vista de Casos de Uso  

| Diagrama de Actores y Casos de Uso | Diagrama de Contexto |
|---|---|
| ![TicTacToe](./docs/diagrams/out/vistaCasosUso/actores.svg) | ![TicTacToe](./docs/diagrams/out/vistaCasosUso/contexto.svg) |  

## Vista de Caso de Uso Start  
![Start](./docs/diagrams/out/vistaCasosUso/StateDiagramFluxInitialState.svg)  

## Vista de Caso de Uso Propose  
![Propose](./docs/diagrams/out/vistaCasosUso/StateDiagramFluxPlayState.svg)  

## Vista de Caso de Uso Resume  
![Resume](./docs/diagrams/out/vistaCasosUso/resume_usecase.svg)  

### Prototipo de Interfaz
  
#### Número de jugadores: 0  
```
--- TIC TAC TOE ---
Number of user? [0, 2]: 0
-------------
|   |   |   |
|   |   |   |
|   |   |   |
-------------
-------------
|   |   |   |
|   |   |   |
| X |   |   |
-------------
-------------
|   | O |   |
|   |   |   |
| X |   |   |
-------------
-------------
|   | O |   |
|   |   | X |
| X |   |   |
-------------
-------------
| O | O |   |
|   |   | X |
| X |   |   |
-------------
-------------
| O | O |   |
|   |   | X |
| X |   | X |
-------------
-------------
| O | O |   |
|   | O | X |
| X |   | X |
-------------
-------------
| O | O |   |
| X | O | X |
|   |   | X |
-------------
-------------
| O | O | O |
| X |   | X |
|   |   | X |
-------------
O Player: You win!!! :-)
Do you want to continue? (y/n):
```  
  
#### Número de jugadores: 1  
  
```
--- TIC TAC TOE ---
Number of user? [0, 2]: 1
-------------
|   |   |   |
|   |   |   |
|   |   |   |
-------------
Enter a coordinate to put a token:
Row: 1
Column: 1
-------------
| X |   |   |
|   |   |   |
|   |   |   |
-------------
-------------
| X |   | O |
|   |   |   |
|   |   |   |
-------------
Enter a coordinate to put a token:
Row: 2
Column: 2
-------------
| X |   | O |
|   | X |   |
|   |   |   |
-------------
-------------
| X |   | O |
|   | X | O |
|   |   |   |
-------------
Enter a coordinate to put a token:
Row: 3
Column: 2
-------------
| X |   | O |
|   | X | O |
|   | X |   |
-------------
-------------
| X |   | O |
|   | X | O |
|   | X | O |
-------------
O Player: You win!!! :-)
Do you want to continue? (y/n):
```  
  
#### Número de jugadores: 2  
  
```
--- TIC TAC TOE ---
Number of user? [0, 2]: 2
-------------
|   |   |   |
|   |   |   |
|   |   |   |
-------------
Enter a coordinate to put a token:
Row: 4
Column: -1
The coordinates are wrong
Enter a coordinate to put a token:
Row: 1
Column: 1
-------------
| X |   |   |
|   |   |   |
|   |   |   |
-------------
Enter a coordinate to put a token:
Row: 1
Column: 1
The square is not empty
Enter a coordinate to put a token:
Row: 1
Column: 2
-------------
| X | O |   |
|   |   |   |
|   |   |   |
-------------
Enter a coordinate to put a token:
Row: 2
Column: 2
-------------
| X | O |   |
|   | X |   |
|   |   |   |
-------------
Enter a coordinate to put a token:
Row: 3
Column: 3
-------------
| X | O |   |
|   | X |   |
|   |   | O |
-------------
Enter a coordinate to put a token:
Row: 1
Column: 3
-------------
| X | O | X |
|   | X |   |
|   |   | O |
-------------
Enter a coordinate to put a token:
Row: 3
Column: 1
-------------
| X | O | X |
|   | X |   |
| O |   | O |
-------------
Origin coordinate to move
Row: 3
Column: 1
There is not a token of yours
Origin coordinate to move
Row: 1
Column: 1
Target coordinate to move
Row: 1
Column: 1
The origin and target squares are the same
Target coordinate to move
Row: 3
The origin and target squares are the same
Target coordinate to move
Row: 3
Column: 1
The square is not empty
Target coordinate to move
Row: 3
Column: 2
-------------
|   | O | X |
|   | X |   |
| O | X | O |
-------------
Origin coordinate to move
Row: 1
Column: 2
Target coordinate to move
Row: 1
Column: 1
-------------
| O |   | X |
|   | X |   |
| O | X | O |
-------------
Origin coordinate to move
Row: 1
Column: 3
Target coordinate to move
Row: 1
Column: 2
-------------
| O | X |   |
|   | X |   |
| O | X | O |
-------------
X Player: You win!!! :-)
Do you want to continue? (y/n):
```
## Analisis  
![Analisis](./docs/diagrams/out/analisis/analisis.svg)  

## Casos de Uso  

### Analisis Start  
![Propose](./docs/diagrams/out/analisis/start.svg)  

### Analisis Propose  
![Resume](./docs/diagrams/out/analisis/play.svg)  

### Analisis Resume  
![ShowBoard](./docs/diagrams/out/analisis/resume.svg)  

## Paquetes  

### Vistas  
![ShowBoard](./docs/diagrams/out/analisis/packageViews.svg)  

### Controladores  
![ShowBoard](./docs/diagrams/out/analisis/packageControllers.svg)  

### Modelos  
![ShowBoard](./docs/diagrams/out/analisis/modelspackage.svg)  

### Types  