# TicTacToe. Requisitos Cliente/Servidor
Universo Santa Tecla  
[uSantaTecla@gmail.com](mailto:uSantaTecla@gmail.com)  
  
**Índice**

1. [Requisitos](#requisitos)  
2. [Vista de Casos de Uso](#vista-de-casos-de-uso)  
2.1. [Vista de Caso de Uso Start](#vista-de-caso-de-uso-start)  
2.2. [Vista de Caso de Uso Play](#vista-de-caso-de-uso-play)  
2.2. [Vista de Caso de Uso Undo](#vista-de-caso-de-uso-undo)  
2.2. [Vista de Caso de Uso Redo](#vista-de-caso-de-uso-redo)  
2.3. [Vista de Caso de Uso Resume](#vista-de-caso-de-uso-resume)  
2.4. [Prototipo de Interfaz](#prototipo-de-interfaz)  
2.4.1. [Consola](#consola)  
3. [Analisis](#analisis)  
3.1. [Casos de Uso](#casos-de-uso)  
3.1.1. [Analisis Start](#analisis-start)  
3.1.2. [Analisis Play](#analisis-play)  
3.1.2. [Analisis Undo](#analisis-undo)  
3.1.2. [Analisis Redo](#analisis-redo)  
3.1.5. [Analisis Resume](#analisis-resume)  
3.2. [Paquetes](#paquetes)  
3.2.1. [Vistas](#vistas)  
3.2.2. [Controladores](#controladores)  
3.2.3. [Modelos](#modelos)  
3.2.4. [Types](#types)  
  
## Requisitos  

| * _Funcionalidad: **Básica + Undo/Redo**_<br/>  * _Interfaz: **Gráfica y Texto**_<br/>  * _Distribución: **Standalone + Client/Server**_<br/>  * _Persistencia: **No**_<br/> | ![TicTacToe](../docs/images/tictactoe.png) | 
| :------- | :------: |  

## Vista de Casos de Uso  

| Diagrama de Actores y Casos de Uso | Diagrama de Contexto |
|---|---|
| ![TicTacToe](./docs/diagrams/out/vistaCasosUso/casosUso/useCase.svg) | ![TicTacToe](./docs/diagrams/out/vistaCasosUso/diagramaEstadosGeneral/StateDiagramGameStates(ContextDiagram).svg) |  

## Vista de Caso de Uso Start  
![Start](./docs/diagrams/out/vistaCasosUso/casoUsoStart/StateDiagramFluxInitialState.svg)  

## Vista de Caso de Uso Play  
![Play](./docs/diagrams/out/vistaCasosUso/casoUsoPlay/StateDiagramFluxPlayState.svg)  

## Vista de Caso de Uso Undo  
![Play](./docs/diagrams/out/vistaCasosUso/casoUsoUndo/StateDiagramFluxUndoState.svg)  

## Vista de Caso de Uso Redo  
![Play](./docs/diagrams/out/vistaCasosUso/casoUsoRedo/StateDiagramRedoUndoState.svg)  

## Vista de Caso de Uso Resume  
![Resume](./docs/diagrams/out/vistaCasosUso/casoUsoResume/resume_usecase.svg) 

### Prototipo de Interfaz  

#### Consola  

```
--- TIC TAC TOE ---
---------------
 |   |   |   | 
 |   |   |   | 
 |   |   |   | 
---------------

----- Choose one option -----
1) Do a action
1
Enter a coordinate to put a token:
Row: 1
Column: 1
---------------
 | X |   |   | 
 |   |   |   | 
 |   |   |   | 
---------------

----- Choose one option -----
1) Do a action
2) Undo previous action
1
Enter a coordinate to put a token:
Row: 2
Column: 1
---------------
 | X |   |   | 
 | O |   |   | 
 |   |   |   | 
---------------

----- Choose one option -----
1) Do a action
2) Undo previous action
2
---------------
 | X |   |   | 
 |   |   |   | 
 |   |   |   | 
---------------

----- Choose one option -----
1) Do a action
2) Undo previous action
3) Redo previous action
3
---------------
 | X |   |   | 
 | O |   |   | 
 |   |   |   | 
---------------

----- Choose one option -----
1) Do a action
2) Undo previous action
1
Enter a coordinate to put a token:
Row: 1
Column: 2
---------------
 | X | X |   | 
 | O |   |   | 
 |   |   |   | 
---------------

----- Choose one option -----
1) Do a action
2) Undo previous action
1
Enter a coordinate to put a token:
Row: 2
Column: 2
---------------
 | X | X |   | 
 | O | O |   | 
 |   |   |   | 
---------------

----- Choose one option -----
1) Do a action
2) Undo previous action
1
Enter a coordinate to put a token:
Row: 1
Column: 3
---------------
 | X | X | X | 
 | O | O |   | 
 |   |   |   | 
---------------
X player: You win!!! :-)
Do you want to continue? (y/n): 
```

## Analisis  
![Analisis](./docs/diagrams/out/Analisis/analisisGeneral/analisis.svg)  

## Casos de Uso  

### Analisis Start  
![Start](./docs/diagrams/out/Analisis/analisisStart/start.svg)  

### Analisis Play 
![Play](./docs/diagrams/out/Analisis/analisisPlay/play.svg)  

### Analisis Undo 
![Play](./docs/diagrams/out/Analisis/analisisUndo/undo.svg)  

### Analisis Redo 
![Play](./docs/diagrams/out/Analisis/analisisRedo/redo.svg)  

### Analisis Resume  
![Resume](./docs/diagrams/out/Analisis/analisisResume/resume.svg)  

## Paquetes  
![ShowBoard](./docs/diagrams/out/Analisis/arquitecturaPaquetes/arquitectura-paquetes.svg)  

### Vistas  
![ShowBoard](./docs/diagrams/out/Analisis/paquetesViews/packageViews.svg)  

### Controladores  
![ShowBoard](./docs/diagrams/out/Analisis/paquetesControllers/packageControllers.svg)  

### Modelos  
![ShowBoard](./docs/diagrams/out/Analisis/paquetesModels/modelspackage.svg)  

### Types  
![ShowBoard](./docs/diagrams/out/Analisis/paquetesTypes/typespackages.svg)  
