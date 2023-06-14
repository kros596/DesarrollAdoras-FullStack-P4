<h1>Práctica 4: PHP y BBDD - Desarrollo Full-Stack (Nivel 3) ED.2022</h1>
<p>
  En esta práctica se pedía elaborar un proyecto PHP que conectase con la base de datos generada en la práctica anterior.
  La finalidad del proyecto será el registro de usuarios en la tabla 'usuario' ya generada.
</p>
<p>
  La presente entrega cuenta con los ficheros necesarios para el correcto funcionamiento de la aplicación y, dentro del directorio 'cursoSQL', se localizan los archivos de la práctica:
  <ul>
    <li>formulario.html: Documento HTML con el contenido del formulario de inscripción.</li>
    <li>formulario.js: Documento JavaScript que ejecuta las funciones de validación de las entradas del usuario.</li>
    <li>style.css: Documento de Hoja de Estilos en Cascada que da estilo al documento HTML y a las entradas del usuario en función del resultado de la validación.</li>
    <li>subscribe.php: Documento PHP que contiene el código necesario para la conexión a la base de datos. Realiza las siguientes labores:
      <ul>
        <li>Recopila los datos del formulario</li>
        <li>Intenta realizar la conexión a la BD.</li>
        <li>Si la conexión es satisfactoria, comprueba si ya se ha registrado el email solicitado, en caso afirmativo, cancela la inscripción</li>
        <li>Si no existe el email solicitado, registra al nuevo usuario en la tabla 'usuario' de la BD</li>
      </ul>
    </li>
    <li>images: Directorio que contiene las imágenes (iconos) para la decoración gráfica resultante de la validación de las entradas.</li>
  </ul>
</p>

