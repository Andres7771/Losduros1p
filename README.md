Descripción del Proyecto:

1. Interfaz de Usuario:
•	La interfaz de usuario se compone de un encabezado, un formulario para agregar nuevas tareas, una lista de tareas, y botones de filtro y limpieza.
•	El encabezado muestra el título "TAREAS".
•	El formulario permite al usuario ingresar nuevas tareas mediante un campo de entrada de texto y un botón "Agregar".
•	La lista de tareas muestra todas las tareas agregadas por el usuario.
•	Los botones de filtro permiten al usuario filtrar las tareas por estado: todas, activas o completadas.
•	El botón "Limpiar Completadas" permite al usuario eliminar todas las tareas completadas de la lista.

2. Funcionalidad:
•	El usuario puede agregar nuevas tareas ingresando el texto en el campo de entrada y presionando el botón "Agregar".
•	Cada tarea en la lista puede ser marcada como completada haciendo clic en ella. Al hacerlo, se aplicará un efecto de tachado al texto.
•	El usuario puede editar una tarea haciendo clic en el botón "Editar" asociado a la tarea. Esto abrirá un cuadro de diálogo donde el usuario puede ingresar el nuevo texto para la tarea.
•	El usuario puede eliminar una tarea haciendo clic en el botón "Borrar" asociado a la tarea.
•	Los botones de filtro permiten al usuario ver solo las tareas activas, completadas o todas las tareas.
•	El botón "Limpiar Completadas" elimina todas las tareas completadas de la lista.
3. Estilos:
•	El proyecto utiliza estilos CSS para dar formato y estilo a los diferentes elementos de la interfaz de usuario.
•	Se aplican efectos de animación para mejorar la experiencia del usuario, como la transición suave de las tareas al agregarlas o eliminarlas.

Tecnologías Utilizadas.
Las tecnologías utilizadas en el proyecto son fundamentales para la creación de una aplicación web efectiva y funcional para gestionar una lista de tareas. A continuación, se proporciona una descripción más detallada de cada una de estas tecnologías y cómo se relacionan con el proyecto:

1. HTML (HyperText Markup Language):
•	HTML es el lenguaje estándar utilizado para crear la estructura y el contenido de una página web.
•	En el proyecto, HTML se utiliza para definir los elementos de la interfaz de usuario, como el encabezado, el formulario para agregar nuevas tareas, la lista de tareas y los botones de filtro y limpieza.
•	La semántica de HTML ayuda a organizar y describir el contenido de la página de manera significativa, lo que facilita la comprensión del propósito y la función de cada elemento por parte de los desarrolladores y los motores de búsqueda.

2. CSS (Cascading Style Sheets):
•	CSS es un lenguaje de estilo utilizado para dar formato y diseño a los elementos HTML en una página web.
•	En el proyecto, CSS se utiliza para definir la apariencia visual de la interfaz de usuario, incluyendo colores, fuentes, tamaños, márgenes, rellenos, bordes y animaciones.
•	La separación de la estructura (HTML) y el estilo (CSS) permite un desarrollo más modular y mantenible, donde los estilos pueden aplicarse de manera consistente en toda la aplicación.

3. JavaScript:
•	JavaScript es un lenguaje de programación que se utiliza para agregar interactividad y funcionalidad dinámica a las páginas web.
•	En el proyecto, JavaScript se emplea para manejar la lógica de la lista de tareas, como la adición, eliminación, edición y filtrado de tareas, así como el almacenamiento y la recuperación de datos en el almacenamiento local del navegador.
•	La capacidad de JavaScript para interactuar con el DOM (Document Object Model) permite actualizar la interfaz de usuario en respuesta a las acciones del usuario, creando una experiencia fluida y receptiva.

Estas tecnologías trabajan en conjunto para crear una aplicación web completa y eficiente para la gestión de listas de tareas. HTML proporciona la estructura y el contenido, CSS ofrece el estilo y el diseño, y JavaScript añade la interactividad y la funcionalidad, lo que resulta en una experiencia de usuario atractiva y fácil de usar.



Desarrollo Código:
Este código HTML establece una interfaz básica para gestionar tareas en una página web. A continuación se detalla cada parte del código:

Estructura del Documento HTML:
Declaración del Tipo de Documento (<!DOCTYPE html>):

Indica que el documento sigue la especificación de HTML5.
Elemento <html>:

Atributo lang="en": Define el idioma de la página como inglés.
Elemento <head>:

Metaetiquetas:
<meta charset="UTF-8">: Especifica la codificación de caracteres como UTF-8.
<meta name="viewport" content="width=device-width, initial-scale=1.0">: Configura la escala inicial y el ancho de la ventana para dispositivos móviles.
Título de la Página (<title>): Establece el título de la página como "Los Duros".
Enlace a Archivo CSS (<link rel="stylesheet" href="./Proyecto.css">): Vincula el archivo CSS externo Proyecto.css para estilos adicionales.
Elemento <body>:

Contenido Visual:
<div class="background"></div>: Un contenedor vacío que podría usarse para el fondo de la página.
<div class="container">: Contenedor principal de contenido.
<h1>TAREAS</h1>: Encabezado principal que indica el propósito de la página.
Formulario de Agregar Tareas (<div class="todo-form">):
<input type="text" id="taskInput" placeholder="Agregar nueva tarea">: Campo de entrada de texto para agregar nuevas tareas.
<input type="date" id="startDateInput">: Campo de entrada para la fecha de inicio de la tarea.
<input type="date" id="dueDateInput">: Campo de entrada para la fecha límite de la tarea.
<button id="addTask">Agregar</button>: Botón para agregar una nueva tarea.
Lista de Tareas (<ul id="taskList"></ul>): Lista ordenada donde se mostrarán las tareas.
Opciones de Filtrado (<div id="filterOptions">):
Botones para filtrar las tareas:
<button id="allTasks">Todas</button>: Mostrar todas las tareas.
<button id="activeTasks">Activas</button>: Mostrar solo las tareas activas.
<button id="completedTasks">Completadas</button>: Mostrar solo las tareas completadas.
<button id="clearCompleted">Limpiar Completadas</button>: Limpiar las tareas completadas de la lista.
Script JavaScript (<script src="./Proyecto.js"></script>):

Vincula el archivo JavaScript externo Proyecto.js, que probablemente contenga la lógica para agregar, filtrar y administrar las tareas en la página.

Este código JavaScript agrega funcionalidad interactiva a una página web diseñada para la gestión de tareas. A continuación, se proporciona una documentación breve de cada parte del código:

Descripción del Código JavaScript:

1. **Evento `DOMContentLoaded`**:
   - Este evento se dispara cuando el HTML ha sido completamente cargado y analizado, sin esperar a que se carguen las imágenes y otros recursos.
   - La función dentro de este evento se ejecuta una vez que la estructura DOM está lista para ser manipulada.

2. **Selección de Elementos del DOM**:
   - Se seleccionan varios elementos del documento HTML utilizando `document.getElementById()` para acceder a los elementos por su ID.
     - `taskInput`, `startDateInput`, `dueDateInput`: Campos de entrada de texto y fechas para ingresar nuevas tareas.
     - `taskList`: Elemento `<ul>` donde se mostrarán las tareas.
     - `allTasksBtn`, `activeTasksBtn`, `completedTasksBtn`, `clearCompletedBtn`: Botones para filtrar y limpiar tareas.

3. **Inicialización de la Lista de Tareas**:
   - Se carga la lista de tareas desde el almacenamiento local (localStorage). Si no hay datos almacenados, se inicializa como un array vacío (`[]`).

4. **Función `saveTasks()`**:
   - Guarda las tareas en el almacenamiento local (localStorage) convirtiéndolas en formato JSON.

5. **Función `renderTasks(filter)`**:
   - Renderiza las tareas en la lista (`taskList`) según el filtro especificado (`'all'`, `'active'`, `'completed'`).
   - Limpia el contenido existente de la lista (`taskList.innerHTML = ''`) antes de renderizar las tareas.
   - Crea elementos `<li>` para cada tarea y los agrega a la lista (`taskList`).
   - Asocia eventos (como editar, borrar y marcar como completado) a cada tarea.

6. **Función `filterTasks(filter)`**:
   - Filtra las tareas según el tipo de filtro especificado (`'active'` para tareas activas, `'completed'` para tareas completadas).
   - Devuelve un array de tareas filtradas.

7. **Manejo de Eventos**:
   - `taskInput.addEventListener('keypress', function(e) { ... })`: Agrega una nueva tarea cuando se presiona la tecla Enter en el campo de texto.
   - `editButton.addEventListener('click', function() { ... })`: Permite editar una tarea existente.
   - `deleteButton.addEventListener('click', function() { ... })`: Permite eliminar una tarea existente.
   - `li.addEventListener('click', function() { ... })`: Permite marcar una tarea como completada o activa.

8. **Funciones de Filtrado y Limpieza**:
   - `clearCompletedTasks()`: Elimina las tareas completadas de la lista.
   - `allTasksBtn.addEventListener('click', function() { ... })`: Renderiza todas las tareas.
   - `activeTasksBtn.addEventListener('click', function() { ... })`: Renderiza solo las tareas activas.
   - `completedTasksBtn.addEventListener('click', function() { ... })`: Renderiza solo las tareas completadas.
   - `clearCompletedBtn.addEventListener('click', function() { ... })`: Limpia las tareas completadas de la lista.

9. **Llamada a `renderTasks()`**:
   - Al final del código, se llama a `renderTasks()` sin un filtro específico para mostrar todas las tareas al cargar la página inicialmente.

Este código permite agregar, editar, eliminar y filtrar tareas dinámicamente en la página web, utilizando el almacenamiento local para persistir los datos entre sesiones del navegador. La funcionalidad principal está centrada en manipular la lista de tareas de manera interactiva en respuesta a las acciones del usuario.

Este código CSS define estilos para una interfaz de usuario de gestión de tareas dentro de un contenedor en una página web. A continuación, se proporciona una documentación breve de cada parte del código:

Descripción del Código CSS:

1. **Estilos Globales (`body`)**:
   - `font-family`: Establece la familia de fuentes predeterminada para todo el documento como Arial o una fuente sans-serif.
   - `margin`, `padding`: Elimina márgenes y rellenos predeterminados del cuerpo (`body`).
   - `background`: Establece una imagen de fondo (`./Fondo.jpg`) centrada y fija en el cuerpo, con tamaño de fondo que cubre toda el área visible.

2. **Estilos del Contenedor Principal (`container`)**:
   - `max-width`: Limita el ancho máximo del contenedor a 800px.
   - `margin`: Centra el contenedor verticalmente (`50px auto`) y horizontalmente (`auto`).
   - `padding`: Añade un relleno interno de 30px alrededor del contenido.
   - `background-color`: Establece un color de fondo semitransparente (blanco con opacidad del 90%).
   - `border-radius`: Aplica esquinas redondeadas con un radio de 15px.
   - `box-shadow`: Agrega una sombra suave al contenedor para un efecto de elevación.

3. **Estilos para Títulos (`h1`)**:
   - `text-align`: Centra el texto del título.
   - `color`: Establece el color del texto a un tono oscuro (`#333`).
   - `margin-bottom`: Agrega espacio inferior de 30px al título.
   - `font-size`: Define el tamaño de fuente del título como 36px.

4. **Estilos del Formulario de Tareas (`todo-form`)**:
   - `display`: Configura el diseño del formulario como flexbox para alinear elementos vertical y horizontalmente.
   - `align-items`, `justify-content`: Centra los elementos dentro del formulario.
   - `margin-bottom`: Añade espacio inferior de 20px al formulario.

5. **Estilos para Elementos del Formulario (`todo-form input[type="text"]`, `todo-form input[type="date"]`, `todo-form button`)**:
   - `padding`, `border`: Establece relleno y bordes alrededor de los elementos de entrada y botones.
   - `border-radius`: Aplica esquinas redondeadas a los elementos.
   - `margin-right`: Agrega espacio a la derecha de los elementos.

6. **Estilos para Botones (`button`)**:
   - `background-color`, `color`: Define el color de fondo y texto de los botones.
   - `cursor`: Cambia el cursor a un puntero al pasar sobre los botones.
   - `transition`: Agrega una transición suave al cambiar el color de fondo al pasar el mouse sobre los botones.

7. **Estilos para Elementos de Lista (`ul`, `li`)**:
   - `list-style-type`: Elimina los estilos de viñetas de las listas.
   - `padding`: Elimina el relleno predeterminado de las listas.
   - `position`: Define la posición relativa de los elementos de lista.
   - `border-bottom`: Agrega una línea divisoria inferior a los elementos de lista.
   - `font-size`: Define el tamaño de fuente de los elementos de lista como 20px.
   - `background-color`, `border-radius`: Establece un fondo y esquinas redondeadas para los elementos de lista.
   - `margin-bottom`: Agrega espacio inferior entre elementos de lista.

8. **Estilos para Tareas Completadas (`completed`)**:
   - `text-decoration`: Aplica una línea tachada al texto de las tareas completadas.
   - `color`: Cambia el color del texto de tareas completadas a un tono más suave (`#999`).

9. **Estilos para Botones de Edición y Eliminación (`edit-btn`, `delete-btn`)**:
   - `background`, `color`: Define el color de fondo y texto de los botones de edición y eliminación.
   - `cursor`: Cambia el cursor a un puntero al pasar sobre los botones.
   - `margin-left`: Agrega espacio a la izquierda de los botones.

10. **Estilos para Fechas (`dates`)**:
    - `font-weight`: Define el grosor de la fuente para las fechas como negrita.

11. **Estilos para Opciones de Filtrado (`#filterOptions`)**:
    - `margin-top`: Agrega espacio en la parte superior de las opciones de filtro.
    - `text-align`: Centra el contenido de las opciones de filtro.

Estos estilos CSS trabajan juntos para crear una interfaz limpia y atractiva para la aplicación de gestión de tareas, con un diseño responsivo y elementos interactivos que mejoran la experiencia del usuario. Los selectores y propiedades CSS se utilizan de manera efectiva para aplicar estilos coherentes y funcionales a los diferentes componentes de la página.


¿Cómo utilizar la aplicación?

 
Entramos al link que es el que nos aparecerá a continuación.
 
Llenamos datos y agregamos proyectos.
 
Agregamos una nueva tarea y nos aparece el inicio y la entrea con el botón de agregar que es el siguiente
 
 
Este botón es para consultar las listas completadas
 
Activas es para ver las tareas activas
  
Que en nuestro caso son las siguientes.

 
Al presionar editar podemos editar parámetros de lo que requiere el trabajo.

Clonar un Repositorio desde GitHub
Paso 1: Obtener la URL del Repositorio
Primero, necesitas la URL del repositorio que deseas clonar desde GitHub. Puedes encontrar la URL en la página del repositorio en GitHub, en el botón verde "Code".

Paso 2: Abrir la Terminal (en Windows, usa Git Bash)
En Windows: Abre Git Bash. Puedes hacer clic derecho en una carpeta y seleccionar "Git Bash Here", o abrir Git Bash desde el menú de inicio.
En macOS o Linux: Abre la Terminal desde la carpeta donde deseas clonar el repositorio.
Paso 3: Clonar el Repositorio
Ejecuta el siguiente comando en la Terminal (sustituye <URL_del_repositorio> con la URL que copiaste en el Paso 1):

bash
Copy code
git clone <URL_del_repositorio>
Esto descargará todos los archivos del repositorio y creará una carpeta local con el nombre del repositorio en el directorio actual.

Ejecutar un Proyecto HTML Localmente
Paso 1: Abrir la Carpeta del Proyecto
Navega a la carpeta del proyecto clonado usando la Terminal. Por ejemplo, si el repositorio se llama nombre-del-repositorio, usa el comando:

bash
Copy code
cd nombre-del-repositorio
Paso 2: Ejecutar un Servidor Web Local
Para ejecutar un proyecto HTML localmente, puedes usar un servidor web simple. Por ejemplo, si tienes Python instalado, puedes usar el módulo http.server para iniciar un servidor web local.

Ejecuta el siguiente comando en la Terminal para iniciar un servidor web en el puerto 8000 (o cualquier otro puerto que desees):

bash
Copy code
python -m http.server
Si estás utilizando Python 3, usa este comando:

bash
Copy code
python3 -m http.server
Paso 3: Abrir el Proyecto en el Navegador
Una vez que el servidor web esté en funcionamiento, abre tu navegador web y visita la siguiente URL:

arduino
Copy code
http://localhost:8000
Esto cargará tu proyecto HTML localmente desde el servidor web en tu navegador. Ahora puedes interactuar con tu proyecto y ver cómo se ve y se comporta en un entorno local.

Nota sobre Otros Servidores Web Locales
Además de usar Python para ejecutar un servidor web local, también puedes utilizar otras herramientas como live-server (para Node.js), XAMPP, WAMP, MAMP, entre otros, para ejecutar proyectos HTML localmente. Cada herramienta tiene su propio método de instalación y uso, así que elige el que mejor se adapte a tus necesidades y conocimientos.

 
Con borrar borramos una tarea, y completadas son para las tareas que ya hayamos hecho.
Link de la página para probar funcionamiento.
Andres7771.github.io

