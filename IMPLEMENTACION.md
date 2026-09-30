# Registro sin área

Esta copia envía nombre, correo, año de nacimiento y género a la pestaña `gid=0` de la hoja indicada en `Código.gs`.

La aplicación web ya está configurada en `app.js` con la URL `/exec` proporcionada. Publica esta carpeta como sitio estático para usar el formulario. Comprueba un envío de prueba directamente en la hoja: el navegador usa `no-cors` y no puede confirmar que se haya guardado la fila.

La hoja debe tener en A1:E1: **Fecha y Hora | Nombre | Correo | Año de nacimiento | Género**. Si está vacía, el script crea esos encabezados con el primer envío. Si ya contiene otros encabezados, el script devuelve un error y no agrega datos.
