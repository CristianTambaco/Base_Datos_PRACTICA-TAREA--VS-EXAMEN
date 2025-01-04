Examen -PRACTICO de Base de Datos:

Objetivo del examen: El examen tiene como objetivo evaluar tu capacidad para trabajar con bases de datos utilizando MySQL. A lo largo de este examen, deberás crear tablas, procedimientos almacenados, funciones, triggers y gestionar usuarios con privilegios específicos. Es importante que sigas las instrucciones detalladamente y utilices buenas prácticas al diseñar y crear la base de datos.

Instrucciones Generales:

Crear la Base de Datos y las Tablas:
Crea la base de datos y las tablas necesarias utilizando el script SQL proporcionado. Asegúrate de que las tablas se creen correctamente con las relaciones adecuadas y los campos correctos.

Las tablas a crear son:

 Clientes

 Productos

 Categorias

 Ordenes

 DetallesOrden

 AuditoriaEliminaciones

 AuditoriaPrecios

Insertar Datos de Ejemplo:
Inserta los datos de ejemplo proporcionados en el script. Asegúrate de que cada tabla tenga al menos unos pocos registros para realizar las consultas posteriores.

Realizar las Consultas y Procedimientos:
Desarrolla las consultas, funciones, procedimientos almacenados, triggers y usuarios según los siguientes requerimientos.

Requerimientos de la practica Examen:

Función para Calcular el Total de una Orden:
o Crea una función llamada CalcularTotalOrden que reciba como parámetro un OrdenID y devuelva el monto total de la orden.

o El monto total debe ser la suma del precio de los productos multiplicado por la cantidad de cada uno, utilizando las tablas DetallesOrden y Productos.

Procedimiento para Insertar un Cliente:
o Crea un procedimiento almacenado llamado InsertarCliente que reciba los parámetros Nombre, Apellidos, FechaNacimiento, Telefono y Correo, y los inserte en la tabla Clientes.

o Después de la inserción, muestra un mensaje que indique que el cliente ha sido registrado exitosamente.

Trigger para Auditar Eliminaciones:
o Crea un trigger que se active después de una eliminación en la tabla Productos.

o El trigger debe registrar la eliminación en la tabla AuditoriaEliminaciones, incluyendo el ProductoID, Nombre, Precio y la fecha de eliminación.

Creación de un Usuario con Privilegios Específicos:
o Crea un usuario llamado usuario_cliente con una contraseña segura.

o Este usuario debe tener privilegios de solo lectura (SELECT) sobre las tablas Clientes, Productos y Ordenes, sin permisos para insertar, actualizar ni eliminar registros.

Procedimiento para Actualizar el Precio de un Producto:
o Crea un procedimiento almacenado llamado ActualizarPrecioProducto que reciba como parámetros un ProductoID y un PrecioNuevo.

o Este procedimiento debe actualizar el precio del producto en la tabla Productos y registrar este cambio en la tabla AuditoriaPrecios, almacenando el PrecioAnterior, PrecioNuevo y la fecha de cambio.

Función para Obtener el Total Gastado por un Cliente:
o Crea una función llamada TotalGastadoPorCliente que reciba como parámetro un ClienteID y devuelva el monto total gastado por ese cliente en todas sus órdenes.

o La función debe calcular el total utilizando las tablas Ordenes y DetallesOrden.

Trigger para Actualizar el Stock de Productos:
o Crea un trigger AFTER INSERT en la tabla DetallesOrden para actualizar el stock de productos en la tabla Productos cada vez que se inserte un nuevo detalle de orden.

o La cantidad vendida debe restarse del stock actual del producto. Si el stock es menor que 1, el trigger debe generar un error.

Procedimiento para Generar un Informe de Ventas por Categoría:
o Crea un procedimiento almacenado llamado InformeVentasPorCategoria que reciba como parámetro un CategoriaID y devuelva el total de ventas para esa categoría.

o El informe debe mostrar el nombre de la categoría y el total de ventas, incluyendo el nombre de los productos vendidos y la cantidad de cada uno.

Creación de un Usuario Administrador con Privilegios Completos:
o Crea un usuario administrador llamado admin_ventas con privilegios completos sobre todas las tablas de la base de datos.

o Este usuario debe tener permisos para ejecutar procedimientos almacenados y triggers.

Backup Completo de la Base de Datos:
o Realiza un backup completo de la base de datos después de haber completado todos los ejercicios. Guarda el archivo generado y súbelo junto con las consultas que hayas ejecutado.

o NO SE OLVIDE CREAR EL INFORME EN PDF

DESCARGUE EL SCRIPT EN EL AULA VIRTUAL
