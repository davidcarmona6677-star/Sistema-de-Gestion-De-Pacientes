# Sistema de Gestión de Pacientes

## Integrantes

* **David Carmona Rosa**
  Matrícula: **25-SISN-2-013**

* **Manuel M. Rijo**
  Matrícula: **25-SSON-2-006**

---

## Descripción breve

El **Sistema de Gestión de Pacientes** es un programa desarrollado en **C#** como aplicación de consola, cuyo objetivo es permitir la administración de la información de diferentes pacientes de manera sencilla y organizada.

El proyecto utiliza los principios de la **Programación Orientada a Objetos (POO)** y una **lista dinámica** para almacenar los pacientes durante la ejecución del programa.

El sistema implementa las operaciones básicas de un **CRUD**, permitiendo:

* **Crear** nuevos pacientes.
* **Consultar** los pacientes registrados.
* **Actualizar** la información de un paciente.
* **Eliminar** pacientes del sistema.

El programa funciona mediante un menú de opciones que permite al usuario seleccionar la operación que desea realizar.

---

## Tecnologías utilizadas

* **Lenguaje:** C#
* **Tipo de aplicación:** Aplicación de consola
* **Programación Orientada a Objetos (POO)**
* **Listas dinámicas**
* **Visual Studio / Visual Studio Code**
* **.NET**

---

## Estructura del proyecto

El proyecto está organizado en diferentes archivos para separar las responsabilidades del programa.

### `Program.cs`

Este archivo contiene el **punto de entrada principal del programa**.

Desde aquí se inicia la aplicación y se presenta el menú principal al usuario. El usuario puede seleccionar las diferentes opciones disponibles para administrar los pacientes.

El archivo se encarga principalmente de:

* Iniciar el programa.
* Mostrar el menú de opciones.
* Solicitar al usuario la opción que desea ejecutar.
* Coordinar las diferentes operaciones del sistema.
* Mostrar los resultados de las operaciones en la consola.

---

### `Pacientes.cs`

Este archivo contiene la clase **Pacientes**, que representa la información correspondiente a cada paciente.

La clase permite crear objetos de tipo paciente y almacenar sus datos.

Cada objeto representa a un paciente individual dentro del sistema.

La utilización de una clase permite aplicar el concepto de **Programación Orientada a Objetos**, facilitando la organización y administración de la información.

---

### `GestorPacientes.cs`

Este archivo contiene la lógica encargada de **administrar la lista de pacientes**.

El gestor permite realizar las diferentes operaciones CRUD sobre los pacientes registrados.

Entre las operaciones principales se encuentran:

* Agregar pacientes.
* Consultar pacientes.
* Buscar información.
* Actualizar datos.
* Eliminar pacientes.

De esta manera, la lógica relacionada con la administración de los pacientes se mantiene separada del archivo principal `Program.cs`.

---

## Datos de entrada

El sistema solicita al usuario la información necesaria para registrar y administrar los pacientes.

Dependiendo de la operación seleccionada, el usuario puede proporcionar datos como:

* Identificador del paciente.
* Nombre del paciente.
* Edad.
* Diagnóstico.
* Información necesaria para actualizar o identificar al paciente.

Los datos son introducidos directamente mediante el teclado utilizando la consola.

---

## Datos que procesa

El sistema procesa la información ingresada por el usuario y permite realizar diferentes operaciones sobre la lista de pacientes.

### Crear

Permite registrar un nuevo paciente en el sistema.

El usuario introduce los datos correspondientes y el programa crea un nuevo objeto de tipo `Pacientes`, agregándolo a la lista.

### Consultar

Permite visualizar los pacientes que se encuentran registrados actualmente en el sistema.

El programa recorre la lista y muestra la información correspondiente en la consola.

### Actualizar

Permite modificar la información de un paciente que ya se encuentra registrado.

El sistema identifica al paciente y permite modificar los datos correspondientes.

### Eliminar

Permite eliminar un paciente de la lista.

El sistema identifica al paciente seleccionado y lo elimina de los registros almacenados durante la ejecución.

### Validaciones

El programa también realiza validaciones para evitar operaciones incorrectas, como intentar trabajar con un paciente que no se encuentra registrado o introducir información no válida.

---

## Datos de salida

Los resultados de las operaciones son mostrados directamente en la consola.

Entre los datos y mensajes que puede mostrar el sistema se encuentran:

* Lista de pacientes registrados.
* Información de un paciente.
* Confirmación de registro.
* Confirmación de actualización.
* Confirmación de eliminación.
* Mensajes cuando un paciente no existe.
* Mensajes de error o validación.
* Opciones disponibles en el menú principal.

---

## Funcionamiento del sistema

Al ejecutar el programa, se muestra un menú principal con las diferentes opciones disponibles.

El usuario selecciona una opción y el sistema ejecuta la operación correspondiente.

El flujo general del programa es:

1. Iniciar el sistema.
2. Mostrar el menú principal.
3. El usuario selecciona una operación.
4. El sistema solicita los datos necesarios.
5. Se procesa la información.
6. Se muestra el resultado en la consola.
7. El sistema vuelve al menú principal.
8. El usuario puede realizar otra operación o finalizar el programa.

---

## Operaciones CRUD

El proyecto implementa las cuatro operaciones fundamentales para administrar información:

| Operación  | Función                               |
| ---------- | ------------------------------------- |
| **Create** | Registrar un nuevo paciente           |
| **Read**   | Consultar pacientes registrados       |
| **Update** | Actualizar información de un paciente |
| **Delete** | Eliminar un paciente                  |

Estas operaciones permiten administrar los registros de pacientes durante la ejecución del programa.

---

## Capturas de pantalla

### Menú principal

En esta captura se muestra el menú principal del sistema y las opciones disponibles para el usuario.

![Menú principal](capturas/menu.png)

### Registro de paciente

Muestra el proceso mediante el cual el usuario introduce la información de un nuevo paciente.

![Registrar paciente](capturas/registrar.png)

### Consulta de pacientes

Muestra la información de los pacientes registrados en el sistema.

![Consultar pacientes](capturas/consultar.png)

### Actualización de paciente

Muestra el proceso utilizado para modificar la información de un paciente existente.

![Actualizar paciente](capturas/actualizar.png)

### Eliminación de paciente

Muestra el proceso utilizado para eliminar un paciente de la lista.

![Eliminar paciente](capturas/eliminar.png)

### Validaciones y mensajes de error

Muestra el comportamiento del sistema cuando el usuario introduce información incorrecta o intenta realizar una operación que no puede ejecutarse.

![Validaciones](capturas/errores.png)

---


