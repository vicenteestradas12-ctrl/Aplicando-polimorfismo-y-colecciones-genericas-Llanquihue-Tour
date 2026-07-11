# Aplicando-polimorfismo-y-colecciones-gen-ricas
# LlanquihueTourApp

## Descripción del proyecto

**LlanquihueTourApp** es una aplicación desarrollada en Java como parte de las actividades de la asignatura de Programación Orientada a Objetos. El sistema representa los distintos servicios turísticos ofrecidos por la agencia **Llanquihue Tour**, utilizando una estructura organizada en paquetes y aplicando los principales conceptos de la programación orientada a objetos.

En esta séptima semana se incorporó el uso de **polimorfismo** y **colecciones genéricas**, permitiendo almacenar distintos tipos de servicios turísticos en una misma colección y recorrerlos dinámicamente mediante referencias a la superclase.

---

## Objetivos de la actividad

* Aplicar herencia entre clases.
* Implementar polimorfismo mediante sobrescritura de métodos.
* Utilizar colecciones genéricas (`List` y `ArrayList`).
* Recorrer objetos de diferentes tipos utilizando referencias de la superclase.
* Mantener una estructura modular organizada por paquetes.

---

## Estructura del proyecto

```text
LlanquihueTourApp
│
├── src
│   ├── model
│   │   ├── ServicioTuristico.java
│   │   ├── RutaGastronomica.java
│   │   ├── PaseoLacustre.java
│   │   └── ExcursionCultural.java
│   │
│   ├── data
│   │   └── GestorServicios.java
│   │
│   └── ui
│       └── Main.java
│
└── README.md
```

---

## Clases implementadas

### ServicioTuristico

Clase base que representa un servicio turístico.

**Atributos:**

* Nombre
* Duración en horas

**Método principal:**

* `mostrarInformacion()`

---

### RutaGastronomica

Hereda de `ServicioTuristico`.

Incluye información sobre la especialidad gastronómica de la ruta.

---

### PaseoLacustre

Hereda de `ServicioTuristico`.

Incluye información del lago donde se realiza el recorrido.

---

### ExcursionCultural

Hereda de `ServicioTuristico`.

Incluye el lugar histórico visitado durante la excursión.

---

### GestorServicios

Clase encargada de administrar los servicios turísticos.

Funciones principales:

* Crear una colección `List<ServicioTuristico>`.
* Almacenar distintos tipos de servicios.
* Entregar la colección para ser recorrida desde la clase principal.

---

### Main

Clase principal de ejecución.

Se encarga de:

* Crear un objeto `GestorServicios`.
* Recorrer la colección mediante un ciclo `for-each`.
* Mostrar la información de cada servicio utilizando polimorfismo.

---

## Conceptos de Programación Orientada a Objetos utilizados

* Encapsulamiento.
* Herencia.
* Polimorfismo.
* Sobrescritura de métodos (`@Override`).
* Colecciones genéricas (`List` y `ArrayList`).
* Organización modular mediante paquetes.

---

## Tecnologías utilizadas

* Java
* Apache NetBeans
* JDK 17 (o la versión utilizada en el proyecto)
* Git
* GitHub

---

## Instrucciones para ejecutar el proyecto

1. Clonar o descargar el repositorio.
2. Abrir el proyecto en Apache NetBeans.
3. Compilar el proyecto.
4. Ejecutar la clase:

```text
ui.Main
```

5. La información de los servicios turísticos se mostrará en la consola.

---

## Resultado esperado

Al ejecutar el programa se despliega la información de todos los servicios turísticos almacenados en la colección, demostrando el funcionamiento del polimorfismo mediante la sobrescritura del método `mostrarInformacion()`.

---

## Autor

**Vicente Estrada**

Actividad Formativa – Semana 7

Aplicando Polimorfismo y Colecciones Genéricas

Programación Orientada a Objetos

11/07/2026
