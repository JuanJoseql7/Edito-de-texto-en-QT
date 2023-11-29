# Editor de texto en QT
# Descripcion
Este proyecto es un editor de texto implementado en C++ utilizando la biblioteca Qt. Proporciona una interfaz gráfica intuitiva y funcionalidades esenciales para manipular texto, así como opciones avanzadas para dar formato y personalizar la apariencia del contenido. A continuación, se detallan las características clave, instrucciones de compilación y otras consideraciones.

# Herramientas utilizadas   

c++ 23

Qt creator 11.0.3 o una version superior 

Un compilador C++ compatible con Qt

# Instrucciones de compilacion y ejecucion 

Para poder ejecutar este proyecto es necesario seguir 3 pasos:

1. Clone el repertorio
2. Abra el proyecto en el programa y ejecutable Qt creator
3. Compile el codigo con ayuda de Qt

# Caracteristicas destacadas

1. Características Destacadas: Abrir y Guardar Archivos: El editor permite abrir archivos de diversos formatos, incluyendo texto (.txt), PDF (.pdf), y documentos ODT (.odt). Asimismo, proporciona opciones para guardar el contenido en diferentes formatos.
2. Eliminar Archivos: Facilita la eliminación de archivos seleccionados mediante una interfaz amigable.
3. Imprimir Contenido: Permite imprimir el contenido del editor con configuraciones personalizables.
4. Formato de Texto: Ofrece opciones para dar formato al texto, como centrado, alineación a la izquierda, justificación y alineación a la derecha.
5. Color de Texto: Permite cambiar el color del texto para personalizar aún más la presentación.
6. Cambiar Fuente: Proporciona la capacidad de cambiar la fuente del texto, ya sea seleccionando una de las opciones predeterminadas o eligiendo una fuente personalizada.

# Arquitectura del codigo

La arquitectura del código sigue un enfoque simple y estructurado, utilizando las clases proporcionadas por la biblioteca Qt. La interfaz gráfica se define mediante un objeto QMainWindow, mientras que las acciones y funciones específicas se manejan mediante funciones conectadas a las señales de los elementos de la interfaz.

# Logica

La lógica del código se basa en la conexión de acciones de la interfaz con funciones específicas. Se utilizan funciones lambda y señales de Qt para establecer estas conexiones. Por ejemplo, la acción de centrar el texto activa la función centrarTexto. Esta lógica modular facilita la expansión y mantenimiento del código.

El código sigue un enfoque orientado a eventos, respondiendo a las acciones del usuario mediante la conexión de señales y ranuras (slots) de Qt. La lógica de manipulación de texto se realiza utilizando QTextCursor y formatos específicos para modificar el contenido del área de edición.

El manejo de archivos y la interacción con el usuario se realiza de manera segura, considerando posibles errores y proporcionando mensajes informativos mediante QMessageBox en caso de operaciones no exitosas. La aplicación sigue las mejores prácticas de diseño de interfaz y programación en Qt.

# Funciones principales 

centrarTexto(QTextEdit* textoEdit)
Esta función utiliza la clase QTextCursor para modificar el formato del bloque actual, centrando así el texto en el área de edición (QTextEdit).

alinearIzquierda(QTextEdit* textoEdit)
Similar a la función anterior, esta función ajusta la alineación del bloque actual a la izquierda, utilizando QTextCursor y QTextBlockFormat.

justificarTexto(QTextEdit* textoEdit)
Justifica el texto en el área de edición al modificar la alineación del bloque actual a través de QTextCursor y QTextBlockFormat.

alinearDerecha(QTextEdit* textoEdit)
Alinea el texto a la derecha en el área de edición mediante la modificación de la alineación del bloque actual utilizando QTextCursor y QTextBlockFormat.

aplicarFormatoTexto(QTextEdit* textoEdit, QTextCharFormat formato)
Esta función aplica el formato de texto proporcionado (QTextCharFormat) al texto seleccionado en el área de edición.

cambiarColorTexto(QTextEdit* textoEdit)
Permite al usuario seleccionar un color mediante un cuadro de diálogo (QColorDialog) y aplica ese color al texto seleccionado en el área de edición.

# Bibliotecas utilizadas

QApplication, QMainWindow, QMenuBar, QMenu, QAction
Estas clases forman la base de la interfaz gráfica de la aplicación. QApplication representa la aplicación en sí, QMainWindow es la ventana principal, y las demás clases se utilizan para construir la interfaz de menú y acciones.

QFileDialog, QFileInfo
Estas clases facilitan la interacción con archivos. QFileDialog permite abrir y guardar archivos, mientras que QFileInfo proporciona información sobre los archivos seleccionados.

QTextEdit
Representa un área de edición de texto enriquecido. Permite la manipulación del contenido de texto, incluida la aplicación de formato.

QPrinter, QPrintDialog
Estas clases están involucradas en la funcionalidad de impresión. QPrinter se configura para imprimir el contenido, y QPrintDialog facilita la interacción con el usuario para seleccionar opciones de impresión.

QToolBar, QIcon, QPixmap
QToolBar crea una barra de herramientas que contiene acciones rápidas. QIcon y QPixmap manejan la carga y visualización de iconos.

QMessageBox, QColorDialog
QMessageBox se utiliza para mostrar mensajes al usuario, mientras que QColorDialog proporciona un cuadro de diálogo para seleccionar colores.

QTextDocumentWriter, QTextStream
Estas clases están relacionadas con la escritura y manipulación de archivos de texto. QTextDocumentWriter se utiliza para escribir documentos en diferentes formatos, y QTextStream ayuda en la manipulación de texto.

QFontDialog
Ofrece un cuadro de diálogo para seleccionar la fuente del texto, proporcionando opciones de personalización.

# Colaborador

Nombre : Juan Jose Quintero Lopez

IE: Universidad tecnologica de pereira - Colombia

Carrera: Ingeneria de sistemas y computacion

Materia: Programacion II

Profesor: Felipe Gutierrez Isaza

Correo Personal: juanjosequinterolopez7@gmail.com

Correo institucional: j.quintero8@utp.edu.co

![Imagen de la UTP](https://www.utp.edu.co/cms-utp/data/bin/UTP/web/uploads/media/comunicaciones/img/utp-n.jpg)

# Colaborador

Nombre : Santiago Orjuela Diaz

IE: Universidad tecnologica de pereira - Colombia

Carrera: Ingeneria de sistemas y computacion

Materia: Programacion II

Profesor: Felipe Gutierrez Isaza

Correo Personal: saordi2702@gmail.com

Correo institucional: santiago.orjuela1@utp.edu.co

![Imagen de la UTP](https://www.utp.edu.co/cms-utp/data/bin/UTP/web/uploads/media/comunicaciones/img/utp-n.jpg)




