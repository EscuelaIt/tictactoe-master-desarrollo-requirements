## Secuencia de versiones TicTacToe

:information_source: Este diagrama muestra las diferentes versiones del juego TicTacToe

![DiagramaSecuencia](/docs/diagrams/out/TicTacToe/TicTacToe.svg)

### Instalación:

❗ La instalación corresponde al entorno Visual Studio Code.

:one: Realizar la instalacion , abrir el CMD como administrador.
  
:heavy_minus_sign: Primer comando

	@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"
	
:heavy_minus_sign: Segundo comando
    
    choco install plantuml

:two: Instalar el plugin de plantUML para Visual Studio Code.  
    
   2.1 En plantUML Ir a extensiones y escribir escribir plantuml.
   
   2.2 Botón derecho sobre la primera (PlantUML Rich PlantUML support) -> Extension Settings
   
   2.3 Apartado Plantuml: Diagrams Root (Se establece la carpeta donde van a estar localizados los diagramas .png
		Ruta: "docs/diagrams/src"

	2.4 Apartado Plantuml: Export Out Dir (Se establece la carpeta para exportar los diagramas)
		Ruta: "docs/diagrams/out"

	2.5 Apartado Plantuml: Render 
		Cambiar la opción de "Local" a "PlantUMLServer"
	
	2.6 Plantuml: Server (Establecer servidor de PlantUML)
		Escribir la ruta oficial del servidor de Plantuml: "https://www.plantuml.com/plantuml"

4. Separar cada diagrama de forma independiente.

5. Estructura del proyecto:
	
	Project Folder/
  docs/
    diagrams/
      src/
        architecture_overview.wsd
      out/
        architecture_overview/
          architecture_overview.png
  ...rest_of_your_project_folders/
  ...rest_of_your_project_files 

6. Permite includepaths, estos se incuyen en un fichero de configuración en JSON( Falta investigación)

7. Para generar el diagrama es necesario presionar Alt+D , la primera vez, despues se recarga automaticamente.

8. Paginación en un diagrama, util para digramas grandes.
	- newpage
	- title: Justo debajo de newPage, para indicar en que se centra el diagrama.

9. Exportar un diagrama, boton derecho "Export current diagram" se genera el "svg" en la carpeta out/

10. Generar URL, boton derecho "Generate URL for current diagram" en la c

No es necesario instalar el plugin para hacer la documentación. Se pueden exportar los diagramas en svg en plantext y meterlos en la carpeta out/nombrefichero/nombrediagrama.svg
Respetando la estructura del punto 5.

