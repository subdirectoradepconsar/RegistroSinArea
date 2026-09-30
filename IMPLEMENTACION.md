# Registro sin área

Esta copia envía nombre, correo, año de nacimiento y género a una pestaña llamada `RegistroSinArea` en la hoja indicada en `Código.gs`. El script crea esa pestaña y sus encabezados automáticamente si no existe, sin modificar la pestaña original.

La aplicación web ya está configurada en `app.js` con la URL `/exec` proporcionada. Después de actualizar `Código.gs` en **Extensiones → Apps Script**, guarda y crea una **nueva versión** desde **Implementar → Gestionar implementaciones**. Comprueba un envío de prueba directamente en la nueva pestaña: el navegador usa `no-cors` y no puede confirmar que se haya guardado la fila.

La nueva pestaña tendrá en A1:E1: **Fecha y Hora | Nombre | Correo | Año de nacimiento | Género**. Si ya existe una pestaña con ese nombre y otros encabezados, el script devuelve un error y no agrega datos.
