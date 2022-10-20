## nttdatacenters-hibernate-t2-cghCristian

   <p align="left">
   <img src="https://img.shields.io/badge/STATUS-EN%20DESAROLLO-green">
   </p>
<h1 align="center">*VERSIÓN ADAPTADA DE LA T1*</h1>

<h2>🚀 Tecnologías usadas:</h2>

* Java +8
* Hibernate
* MySQL

<h2>🆕 Añadidos:</h2>

* Clase Abstracta con elementos comunes
* Ahora verificará que el DNI no existe antes de solicitar datos del contrato.
* Esta versión a diferencia del T3 el método "findByIdClient" en la clase contractDaoImpl que dará como resultado una lista de objetos Contract resultado de pasar el objeto cliente generado a través de una petición de ID del mismo, en la versión T3 se pasaba directamente el integer para realizar una consulta join.
* Por medio te .toString() al objeto Contract obtendremos el contrato + clientes y contratos sin clientes que se podrán asignar a clientes ya creados.

<h3><i>Ejercicio propuesto:</i></h3>

Crear una tabla cliente con columnas (ID, Nombre, Apellido1, Apellido2, DNI que será único).

Crear los siguientes métodos CRUD con el diseño DAO mediante Hibernate:

- `Funcionalidad 1`: Nuevo cliente.
- `Funcionalidad 2`: Obtener todos los clientes.
- `Funcionalidad 3`: Obtener cliente por ID.
- `Funcionalidad 4`: Obtener cliente por nombre, apellidos.
- `Funcionalidad 5`: Actualizar cliente por ID.
- `Funcionalidad 6`: Eliminar cliente por ID.
- `Funcionalidad 7`: Eliminar todos los clientes.

Crear una tabla Contrato con columnas (ID, Fecha de vigencia, Fecha de expiracion, Precio, Relacion con el cliente), un cliente puede tener 1 contrato y un contrato puede tener N clientes.

Creados los siguientes métodos CRUD con el diseño DAO mediante Hibernate:

- `Funcionalidad 8`: Crear contrato nuevo.
- `Funcionalidad 9`: Asociar contrato nuevo con cliente.
- `Funcionalidad 10`: Obtener todos los contratos y clientes relacionados.
- `Funcionalidad 11`: Obtener contrato por ID contrato.
- `Funcionalidad 12`: Actualizar contrato por ID.
- `Funcionalidad 13`: Eliminar contrato por ID.
- `Funcionalidad 14`: Eliminar contrato por ID.
- `Funcionalidad 15`: Eliminar todos los contratos.
- `Funcionalidad 0`: Salir


<h4 align="center">⚠️ En eclipse revisar Run Application para verificar que carga correctamente en caso de recibir un error de carga de clase principal. ⚠️</h4>
