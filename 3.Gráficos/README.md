# TicTacToe. Requisitos Gráficos
Universo Santa Tecla  
[uSantaTecla@gmail.com](mailto:uSantaTecla@gmail.com)  
  
**Índice**

1. [Requisitos](#requisitos)  
2. [Vista de Casos de Uso](#vista-de-casos-de-uso)  
2.1. [Vista de Caso de Uso Start](#vista-de-caso-de-uso-start)  
2.2. [Vista de Caso de Uso Play](#vista-de-caso-de-uso-play)  
2.3. [Vista de Caso de Uso Resume](#vista-de-caso-de-uso-resume)  
2.4. [Prototipo de Interfaz](#prototipo-de-interfaz)  
2.4.1. [Grafica](#grafica)  
2.4.2. [Consola](#consola)  
3. [Analisis](#analisis)  
3.1. [Casos de Uso](#casos-de-uso)  
3.1.1. [Analisis Start](#analisis-start)  
3.1.2. [Analisis Play](#analisis-play)  
3.1.3. [Analisis Resume](#analisis-resume)  
3.2. [Paquetes](#paquetes)  
3.2.1. [Vistas](#vistas)  
3.2.2. [Controladores](#controladores)  
3.2.3. [Modelos](#modelos)  
3.2.4. [Types](#types)  
4. [Diseño](#diseño)  
   4.1. [Vista de Despliegue](#vista-de-despliegue)  
   4.2. [Vista de Participantes](#vista-de-participantes)  
   4.3. [Vista de Interaccion de Participantes](#vista-de-interaccion-de-participantes)  
  
## Requisitos  

| * _Funcionalidad: **Básica**_<br/>  * _Interfaz: **Gráfica y Texto**_<br/>  * _Distribución: **Standalone**_<br/>  * _Persistencia: **No**_<br/> | ![TicTacToe](../docs/images/tictactoe.png) | 
| :------- | :------: |  

## Vista de Casos de Uso  

| Diagrama de Actores y Casos de Uso | Diagrama de Contexto |
|---|---|
| ![TicTacToe](./docs/diagrams/out/vistaCasosUso/actores.svg) | ![TicTacToe](./docs/diagrams/out/vistaCasosUso/contexto.svg) |  

## Vista de Caso de Uso Start  
![Start](./docs/diagrams/out/vistaCasosUso/StateDiagramFluxInitialState.svg)  

## Vista de Caso de Uso Play  
![Play](./docs/diagrams/out/vistaCasosUso/StateDiagramFluxPlayState.svg)  

## Vista de Caso de Uso Resume  
![Resume](./docs/diagrams/out/vistaCasosUso/resume_usecase.svg)  

### Prototipo de Interfaz  

#### Grafica

| Pantallas | Diálogos |
|---|---|
| ![TicTacToe](./docs/images/pantallas.png) | ![TicTacToe](./docs/images/dialogos.png) |

#### Consola  
  
```
--- TIC TAC TOE ---
-------------
|   |   |   | 
|   |   |   | 
|   |   |   | 
-------------
Coordinate to put
Row: 1
Column: 1
-------------
| X |   |   | 
|   |   |   | 
|   |   |   | 
-------------
Coordinate to put
Row: 3
Column: 2
-------------
| X |   |   | 
|   |   |   | 
|   | O |   | 
-------------
Coordinate to put
Row: 1
Column: 2
-------------
| X | X |   | 
|   |   |   | 
|   | O |   | 
-------------
Coordinate to put
Row: 3
Column: 3
-------------
| X | X |   | 
|   |   |   | 
|   | O | O | 
-------------
Coordinate to put
Row: 1
Column: 3
-------------
| X | X | X | 
|   |   |   | 
|   | O | O | 
-------------
X Player: You win!!! :-)
Do you want to continue? (y/n):
```
## Analisis  
![Analisis](./docs/diagrams/out/analisis/analisis.svg)  

## Casos de Uso  

### Analisis Start  
![Start](./docs/diagrams/out/analisis/start.svg)  

### Analisis Play 
![Play](./docs/diagrams/out/analisis/play.svg)  

### Analisis Resume  
![Resume](./docs/diagrams/out/analisis/resume.svg)  

## Paquetes  
![ShowBoard](./docs/diagrams/out/analisis/arquitectura-paquetes.svg)  

### Vistas  
![ShowBoard](./docs/diagrams/out/analisis/packageViews.svg)  

### Controladores  
![ShowBoard](./docs/diagrams/out/analisis/packageControllers.svg)  

### Modelos  
![ShowBoard](./docs/diagrams/out/analisis/modelspackage.svg)  

### Types  
![ShowBoard](./docs/diagrams/out/analisis/typespackages.svg)  

## Diseño  

### Vista de Despliegue  
![Despliegue](./docs/diagrams/out/Diseño/first/diseño_la_arquitectura.svg)  

### Vista de Participantes  
![Participantes](./docs/diagrams/out/Diseño/second/diseño_caso_uso.svg)  

### Vista de Interaccion de Participantes  
![Interaccion_Participantes](./docs/diagrams/out/Diseño/third/secuencia.svg)  
