Introducción
En el mundo acelerado de hoy, donde las agendas están llenas de tareas y compromisos, la gestión eficaz del tiempo se ha vuelto más importante que nunca. En este contexto, las aplicaciones de listas de tareas juegan un papel fundamental al ayudar a las personas a organizar y priorizar sus actividades diarias.
La presente aplicación web, desarrollada para la gestión de listas de tareas, surge como una solución práctica y accesible para aquellos que buscan optimizar su productividad y mantenerse al tanto de sus responsabilidades. Al proporcionar una interfaz intuitiva y funcionalidades clave, esta aplicación busca simplificar el proceso de manejo de tareas, permitiendo a los usuarios concentrarse en lo que realmente importa.
A lo largo de esta experiencia de desarrollo, se explorarán y aplicarán diversas tecnologías web, desde la estructura básica de HTML hasta la interactividad dinámica de JavaScript, pasando por la estilización elegante de CSS. Mediante la combinación de estas tecnologías, se construirá una aplicación robusta y fácil de usar que pueda adaptarse a las necesidades y preferencias de una amplia gama de usuarios.
En esta introducción, se establecerán los fundamentos del proyecto y se delineará su alcance y objetivo principal. A través del análisis detallado de las tecnologías utilizadas y las funcionalidades implementadas, se brindará una visión general completa de la aplicación de lista de tareas y se sentarán las bases para el desarrollo posterior del proyecto.














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

Estructura Básica:
Se define el tipo de documento y el idioma (en para inglés).
Se incluyen metaetiquetas para el juego de caracteres (UTF-8) y la configuración de la vista.
Se establece el título de la página como "Los Duros".
Se vincula un archivo CSS externo (disenio.css) para los estilos de la página.
 
Se incorpora un archivo JavaScript externo (funcion.js) para la lógica de la aplicación.
Contenido Principal:
Se utiliza un contenedor principal (div con clase container) para estructurar el contenido.
Se agrega un encabezado principal (<h1>) con el texto "TAREAS".
Dentro del contenedor principal, se encuentra un formulario (div con clase todo-form) para agregar nuevas tareas.
Formulario de Tareas:
El formulario contiene etiquetas (<label>) y campos de entrada (<input>) para:
Nombre de la tarea (taskInput).
Fecha de inicio (startDateInput) usando un campo de tipo date.
Hora de inicio (startTimeInput) usando un campo de tipo time.
Fecha de entrega (dueDateInput) usando un campo de tipo date.
Hora de entrega (dueTimeInput) usando un campo de tipo time.
Lista de Tareas:
 

Se utiliza una lista no ordenada (<ul>) con el id taskList para mostrar las tareas agregadas.
Opciones de Filtro:
Se proporcionan botones dentro del div con id filterOptions para filtrar las tareas:
Todas (allTasks): Muestra todas las tareas.
Activas (activeTasks): Muestra las tareas activas.
Completadas (completedTasks): Muestra las tareas completadas.
Limpiar Completadas (clearCompleted): Permite limpiar las tareas completadas de la lista.
Recursos Externos:
Se enlazan archivos externos:
disenio.css para estilos.
funcion.js para la lógica de la aplicación.
Este código JavaScript agrega funcionalidad interactiva a una página web diseñada para la gestión de tareas. A continuación, se proporciona una documentación breve de cada parte del código:
Descripción del Código JavaScript:
El código JavaScript proporcionado se encarga de agregar funcionalidad a la página HTML mediante eventos y lógica para administrar una lista de tareas, incluyendo la capacidad de agregar, editar, eliminar, filtrar y marcar tareas como completadas.


1. Evento `DOMContentLoaded`:
   - Se utiliza `document.addEventListener('DOMContentLoaded', function() { ... })` para ejecutar el código una vez que el DOM está completamente cargado.

2. Obtención de Referencias a Elementos del DOM:
   - Se obtienen referencias a varios elementos del DOM utilizando `document.getElementById` para:
     - `taskInput`, `startDateInput`, `startTimeInput`, `dueDateInput`, `dueTimeInput`: Campos de entrada para datos de la tarea.
     - `taskList`: Lista `<ul>` donde se mostrarán las tareas.
     - `allTasksBtn`, `activeTasksBtn`, `completedTasksBtn`, `clearCompletedBtn`: Botones para filtrar y limpiar tareas.

3. Inicialización de la Lista de Tareas:
   - Se intenta obtener la lista de tareas del almacenamiento local utilizando `localStorage.getItem`, y si está vacía o no existe, se inicializa una lista vacía.

4. Función `saveTasks`:
   - Esta función guarda la lista de tareas en el almacenamiento local utilizando `localStorage.setItem`.

5. Función `renderTasks`:
   - Esta función renderiza las tareas en la lista (`taskList`) según un filtro especificado (`all`, `active`, `completed`).
   - Itera sobre las tareas filtradas y crea elementos HTML dinámicamente para cada tarea.
   - Asigna eventos a los botones de editar, eliminar y marcar tareas como completadas/incompletas.

6. Función `filterTasks`:
   - Esta función filtra las tareas según el estado (`active`, `completed`).

7. Función `clearCompletedTasks`:
   - Esta función elimina las tareas completadas de la lista.

8. Eventos:
   - Se asignan varios eventos a elementos del DOM:
     - `keypress` en `taskInput` para agregar una tarea cuando se presiona Enter.
     - `click` en los botones de filtro (`allTasksBtn`, `activeTasksBtn`, `completedTasksBtn`) para mostrar tareas según su estado.
     - `click` en `clearCompletedBtn` para limpiar las tareas completadas.

9. Validación y Manipulación de Datos:
   - Antes de agregar una tarea, se realizan validaciones como verificar que la fecha de inicio no sea posterior a la fecha de entrega.
   - Se agrega la tarea a la lista, se guarda en el almacenamiento local usando `saveTasks` y se renderizan las tareas nuevamente en la lista.
   - Se limpian los campos de entrada después de agregar una tarea.

10. Renderizado Inicial:
    - Al cargar la página (`renderTasks();`), se renderizan todas las tareas por defecto.

En resumen, este código JavaScript implementa la funcionalidad necesaria para manejar una lista de tareas dentro de una página web, permitiendo agregar, editar, eliminar, filtrar y marcar tareas como completadas/incompletas, todo integrado con el almacenamiento local del navegador para persistir los datos entre sesiones.
Descripción del Código CSS:

1. Estilos Globales (`body`):
•	`font-family`: Establece la familia de fuentes predeterminada para todo el documento como Arial o una fuente sans-serif.
•	`margin`, `padding`: Elimina márgenes y rellenos predeterminados del cuerpo (`body`).
•	`background`: Establece una imagen de fondo (`./Fondo.jpg`) centrada y fija en el cuerpo, con tamaño de fondo que cubre toda el área visible.

2. Estilos del Contenedor Principal (`container`):
•	`max-width`: Limita el ancho máximo del contenedor a 800px.
•	`margin`: Centra el contenedor verticalmente (`50px auto`) y horizontalmente (`auto`).
•	`padding`: Añade un relleno interno de 30px alrededor del contenido.
•	`background-color`: Establece un color de fondo semitransparente (blanco con opacidad del 90%).
•	`border-radius`: Aplica esquinas redondeadas con un radio de 15px.
•	`box-shadow`: Agrega una sombra suave al contenedor para un efecto de elevación.

3. Estilos para Títulos (`h1`):
•	`text-align`: Centra el texto del título.
•	`color`: Establece el color del texto a un tono oscuro (`#333`).
•	`margin-bottom`: Agrega espacio inferior de 30px al título.
•	`font-size`: Define el tamaño de fuente del título como 36px.

4. Estilos del Formulario de Tareas (`todo-form`):
•	`display`: Configura el diseño del formulario como flexbox para alinear elementos vertical y horizontalmente.
•	`align-items`, `justify-content`: Centra los elementos dentro del formulario.
•	`margin-bottom`: Añade espacio inferior de 20px al formulario.

5. Estilos para Elementos del Formulario (`todo-form input[type="text"]`, `todo-form input[type="date"]`, `todo-form button`):
•	`padding`, `border`: Establece relleno y bordes alrededor de los elementos de entrada y botones.
•	`border-radius`: Aplica esquinas redondeadas a los elementos.
•	`margin-right`: Agrega espacio a la derecha de los elementos.

6. Estilos para Botones (`button`):
•	`background-color`, `color`: Define el color de fondo y texto de los botones.
•	`cursor`: Cambia el cursor a un puntero al pasar sobre los botones.
•	`transition`: Agrega una transición suave al cambiar el color de fondo al pasar el mouse sobre los botones.

7. Estilos para Elementos de Lista (`ul`, `li`):
•	`list-style-type`: Elimina los estilos de viñetas de las listas.
•	`padding`: Elimina el relleno predeterminado de las listas.
•	`position`: Define la posición relativa de los elementos de lista.
•	`border-bottom`: Agrega una línea divisoria inferior a los elementos de lista.
•	`font-size`: Define el tamaño de fuente de los elementos de lista como 20px.
•	`background-color`, `border-radius`: Establece un fondo y esquinas redondeadas para los elementos de lista.
•	`margin-bottom`: Agrega espacio inferior entre elementos de lista.

8. Estilos para Tareas Completadas (`completed`):
•	`text-decoration`: Aplica una línea tachada al texto de las tareas completadas.
•	`color`: Cambia el color del texto de tareas completadas a un tono más suave (`#999`).

9. Estilos para Botones de Edición y Eliminación (`edit-btn`, `delete-btn`):
•	`background`, `color`: Define el color de fondo y texto de los botones de edición y eliminación.
•	`cursor`: Cambia el cursor a un puntero al pasar sobre los botones.
•	`margin-left`: Agrega espacio a la izquierda de los botones.

10. Estilos para Fechas (`dates`):
•	`font-weight`: Define el grosor de la fuente para las fechas como negrita.

11. Estilos para Opciones de Filtrado (`#filterOptions`):
•	`margin-top`: Agrega espacio en la parte superior de las opciones de filtro.
•	`text-align`: Centra el contenido de las opciones de filtro.

Estos estilos CSS trabajan juntos para crear una interfaz limpia y atractiva para la aplicación de gestión de tareas, con un diseño responsivo y elementos interactivos que mejoran la experiencia del usuario. Los selectores y propiedades CSS se utilizan de manera efectiva para aplicar estilos coherentes y funcionales a los diferentes componentes de la página.


¿Cómo utilizar la aplicación?
Primero debemos de entrar al link que esta en el post de github  
Que es el que nos aparecerá a continuación. https://andres7771.github.io/Losduros1p/ 






 
Llenamos datos y agregamos proyectos, tenemos que agregar la asignación o tarea, fecha de inicio. Hora de inicio, fecha de entrega y hora de entrega.

 
Asignamos nombre a la tarea y una fecha de inicio
 
Asignamos hora de inicio con el panel.
 
Así como fecha y hora de entrega

Ya agregado nos aparece esto  

 
Podemos editar la asignación.
 
Así como completarlas
 
Con el siguiente menú
Donde tenemos las opciones de ver todas las actividades, listas activas, completadas y borrar las actividades.

Link de la página para probar funcionamiento.
https://andres7771.github.io/Losduros1p/ 

Conclusiones:

El proyecto de aplicación web para gestionar una lista de tareas ha sido una experiencia favorable, ya  que ha permitido explorar y aplicar diversas tecnologías web. A lo largo del desarrollo de este proyecto, se han alcanzado varias conclusiones significativas:

1. Importancia de la Interactividad: La incorporación de JavaScript para agregar interactividad a la aplicación ha demostrado ser fundamental. Gracias a JavaScript, los usuarios pueden realizar acciones como agregar, editar, eliminar y filtrar tareas de manera intuitiva, lo que mejora significativamente la experiencia del usuario.

2. Separación de Responsabilidades: La separación clara entre la estructura (HTML), el estilo (CSS) y la funcionalidad (JavaScript) ha facilitado el desarrollo y mantenimiento del proyecto. Esta práctica de desarrollo ayuda a organizar el código de manera más ordenada y modular, lo que hace que sea más fácil de entender y mantener a medida que el proyecto crece.

3. Persistencia de Datos: La utilización del almacenamiento local del navegador para guardar las tareas ha resultado ser una solución eficaz para mantener la integridad de los datos entre sesiones. Esto permite a los usuarios retomar su lista de tareas exactamente donde la dejaron, incluso después de cerrar el navegador.

4. Diseño Responsivo: Aunque no se ha mencionado explícitamente en el proyecto, es importante tener en cuenta la importancia del diseño responsivo en aplicaciones web. Garantizar que la aplicación se vea y funcione correctamente en una variedad de dispositivos y tamaños de pantalla es crucial para brindar una experiencia de usuario consistente y accesible.

5. Aprendizaje Continuo: El desarrollo de este proyecto ha servido como una oportunidad para aprender y mejorar las habilidades en el desarrollo web. Desde la comprensión más profunda de HTML, CSS y JavaScript hasta el descubrimiento de técnicas avanzadas y prácticas recomendadas, cada paso del proyecto ha sido una oportunidad para crecer y desarrollarse como desarrollador web.

En resumen, el proyecto de aplicación web para gestionar una lista de tareas ha sido un ejercicio valioso que ha permitido aplicar y consolidar conocimientos en tecnologías web fundamentales. A través de la planificación, implementación y refinamiento de la aplicación, se han obtenido lecciones importantes que servirán como base para proyectos futuros y un mayor desarrollo profesional en el campo del desarrollo web.



