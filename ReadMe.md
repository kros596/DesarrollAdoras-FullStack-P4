<h1>Práctica 6: API's HTML5 - Desarrollo Full-Stack (Nivel 3) ED.2022</h1>
<p>
  En esta práctica se pedía elaborar un documento HTML que permitiese depositar mediante DROP un archivo de vídeo y que éste fuese reproducido,
  haciendo uso de las API's de HTML5 para esto.
</p>
<p>
  De este modo se ha elaborado el fichero Index.html en el cual se presenta una página con un área en el cual depositar los archivos y un área de reproducción de vídeo.
  Así mismo se incluye una botonera con botones que permiten:
  <ul>
    <li>Reproducir el vídeo</li>
    <li>Pausar el vídeo</li>
    <li>Subir el volumen</li>
    <li>Bajar el volumen</li>
    <li>Quitar el vídeo asociado</li>
    <li>Reiniciar el vídeo</li>
  </ul>
</p>
<p>
  Se han elaborado estilos para el diseño de la página y una serie de funciones en javascript que permiten:
  <ul>
    <li><b>función dragover_handler(evento)</b>: maneja el evento de arrastrar un archivo por encima del área de deposito de archivos. Resalta dicha área para indicar al usuario la acción.</li>
    <li><b>función dragleave_handler(evento)</b>: maneja el evento de dejar de arrastrar un archivo por encima del área de deposito de archivos. Resetea dicha área para indicar al usuario la salida de la acción.</li>
    <li><b>función drop_handler(evento)</b>: maneja el evento depositar un archivo en el área de deposito de archivos. Ejecuta diversos procesos:
        <ol>
          <li>Desasocia el vídeo que pudiese estar asociado previamente.</li>
          <li>Comprueba que se han depositado archivos, en caso contrario, sale de la función omitiendo el resto de procesos.</li>
          <li>Extrae el fichero depositado y la extensión del mismo para validar que es un formato de archivo válido (mp4, mp3, wav, wma) y realiza una acción en función de la validez:
            <ul>
              <li>En caso de <b>ser válido</b>, muestra el mensaje de que el vídeo se está reproduciendo, asocia la fuente del vídeo al fichero depositado y lo reproduce.</li>
              <li>En caso de <b>no ser válido</b> muestra el error indicando que el fichero es inválido.</li>
            </ul>
          </li>
        </ol>
    </li>
    <li><b>función validateExtension(extensión)</b>: Valida la extensión pasada como parámetro con la lista de extensiones permitidas: mp4, mp3, wav y wma.
      Para ello, busca coincidencias en la lista y, en caso de encontrarla, sale del bucle y devuelve el valor true. En caso contrario devuelve false.
    </li>
    <li><b>función clearVideo()</b>: Pausa el vídeo, resetea la fuente del mismo y esconde el mensaje de aviso.</li>
    <li><b>función restartVideo()</b>: Pausa el vídeo, indica el tiempo actual del video a 0 para reiniciarlo y lo reproduce.</li>
  </ul>
</p>
