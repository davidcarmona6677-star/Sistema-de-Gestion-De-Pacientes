# Sistema de Gestión de Pacientes

## Descripción

Este proyecto consiste en un sistema de consola desarrollado en **C#** para gestionar la información de pacientes de una clínica.

El sistema utiliza **programación orientada a objetos (POO)** y una lista dinámica `List<Paciente>` para almacenar temporalmente los datos de los pacientes durante la ejecución del programa.

El objetivo principal es implementar las operaciones básicas del **CRUD**:

* Crear pacientes.
* Consultar pacientes.
* Actualizar información.
* Eliminar pacientes.

## Funcionalidades

El programa cuenta con un menú principal que permite realizar las siguientes operaciones:

### 1. Registrar nuevo paciente

Permite ingresar los datos de un nuevo paciente:

* ID o cédula.
* Nombre completo.
* Edad.
* Sexo.
* Diagnóstico.
* Fecha de ingreso.

Antes de registrar al paciente, el sistema verifica que el ID no esté duplicado y que los datos introducidos sean válidos.

### 2. Listar todos los pacientes

Muestra en pantalla todos los pacientes registrados actualmente en el sistema junto con toda su información.

### 3. Buscar paciente

Permite localizar un paciente utilizando:

* Su ID.
* Su nombre.

Cuando se realiza una búsqueda por nombre, el sistema puede mostrar todos los pacientes cuyo nombre coincida con el texto introducido.

### 4. Actualizar paciente

Permite modificar los datos de un paciente existente.

Primero se busca al paciente mediante su ID y posteriormente se pueden actualizar datos como:

* Nombre.
* Edad.
* Sexo.
* Diagnóstico.
* Fecha de ingreso.

### 5. Eliminar paciente

Permite eliminar un paciente utilizando su ID.

Antes de realizar la eliminación, el sistema muestra los datos del paciente y solicita una confirmación al usuario para evitar eliminaciones accidentales.

### 6. Salir

Finaliza la ejecución del programa.

## Organización del proyecto

El proyecto está dividido en diferentes clases para mantener el código organizado:

### `Paciente.cs`

Contiene la clase `Paciente`, que representa la información de cada paciente.

Sus propiedades son:

```text
ID
Nombre completo
Edad
Sexo
Diagnóstico
Fecha de ingreso
```

También contiene un método encargado de mostrar los datos del paciente en pantalla.

### `GestorPacientes.cs`

Contiene la lógica principal para administrar los pacientes.

Utiliza:

```csharp
List<Paciente>
```

Esta lista permite almacenar dinámicamente todos los pacientes durante la ejecución del programa.

La clase contiene métodos para:

* Registrar pacientes.
* Listar pacientes.
* Buscar por ID.
* Buscar por nombre.
* Actualizar pacientes.
* Eliminar pacientes.

### `Program.cs`

Contiene el punto de inicio del programa y el menú principal.

Desde esta clase el usuario puede seleccionar las diferentes opciones del sistema y ejecutar las operaciones disponibles.

## Validaciones

El sistema incluye diferentes validaciones para evitar errores durante el uso:

* El ID del paciente no puede estar duplicado.
* El ID es obligatorio.
* El nombre es obligatorio.
* La edad debe ser un número válido.
* La edad debe estar dentro de un rango razonable.
* La fecha de ingreso debe tener un formato válido.
* Se solicita confirmación antes de eliminar un paciente.
* Se muestran mensajes de error cuando los datos introducidos no son válidos.

## Tecnologías utilizadas

* **Lenguaje:** C#
* **Framework:** .NET
* **Tipo de aplicación:** Aplicación de consola
* **Estructura:** Programación Orientada a Objetos (POO)
* **Estructura de datos:** `List<T>`

## Funcionamiento general

El programa comienza mostrando un menú principal. El usuario selecciona una opción y el sistema ejecuta la operación correspondiente.

Los pacientes se almacenan temporalmente en una lista dinámica:

```text
List<Paciente>
```

El menú permanece activo hasta que el usuario selecciona la opción **6. Salir del sistema**.

Después de realizar una operación, el programa permite al usuario repetir la misma operación o regresar al menú principal.

## Objetivo académico

Este proyecto fue desarrollado como práctica de la asignatura **Algoritmos Computacionales**, con el propósito de aplicar conceptos de:

* Programación orientada a objetos.
* Clases y objetos.
* Listas dinámicas.
* Métodos.
* Validación de datos.
* Operaciones CRUD.
* Estructuración y organización del código.
* Manejo de menús en aplicaciones de consola.

## Autores

Proyecto realizado como actividad académica para la asignatura **Algoritmos Computacionales – Universidad O&M**.
