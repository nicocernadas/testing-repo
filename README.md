# Ejemplo base para TP Algo3

[![Build](https://github.com/algo3-unsam/proyecto-base-tp/actions/workflows/build.yml/badge.svg)](https://github.com/algo3-unsam/tp-recetas-2020-gr-xx/actions/workflows/build.yml) ![Coverage](./.github/badges/jacoco.svg)

- El build de Github Actions funciona de una, no tenés que configurar nada
- También el coverage se genera solito si respetás las dependencias que están en el `build.gradle.kts`
- en el archivo [settings.gradle.kts](./settings.gradle.kts) que está en el raíz tenés que cambiarle al nombre de tu proyecto

```kts
rootProject.name = "proyecto-base-tp"
```

- Para los badges de build y coverage (las imágenes que ves con el build passing y el % en este README), tenés que reemplazar `tp-worldcapp-2023-gr-xx` por el repositorio correspondiente.

## El proyecto

Antes que nada, la idea de este proyecto es que te sirva como base para poder desarrollar el backend en la materia [Algoritmos 3](https://algo3.uqbar-project.org/). Por eso está basado en _Maven_, y el archivo `build.gradle.kts` tiene dependencias a

- Spring Boot
- JUnit
- JaCoCo (Java Code Coverage), para que agregues el % de cobertura en el README
- la versión de Kotlin que estaremos usando
- además de estar basado en la JDK 21

### Pasos para adaptar tu proyecto de Algo2 a Algo3

El proceso más simple para que puedan reutilizar el proyecto de Algo2 en Algo3 es:

- generar una copia de todo el directorio que contiene este proyecto
- eliminar la carpeta `.git` que está oculta
- copiar del proyecto de Algo2 las carpetas `src/main/kotlin` y `src/test/kotlin` y la ubican en el mismo lugar en el proyecto de Algo3
- apuntar al proyecto de github mediante

```bash
git remote add origin ...dirección del repo git...
```

El proyecto tiene un main, en la clase `ProyectoApplication`, que levantará el servidor web en el puerto 9000, tienen que renombrarlo al TP actual. También tenés

- un test de integración de ejemplo (en `src/test/kotlin`)

--------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 🍽️ Algo que Pedir

**Algo que Pedir** es una aplicación web para gestión de pedidos en locales gastronómicos. Este proyecto presenta una serie de vistas estáticas desarrolladas con HTML y CSS, enfocadas en la experiencia del usuario y la organización visual de la interfaz.

## 👨‍🏫 Tutor:

👨‍💻 FOGLIA, Pablo

## 🤝 Integrantes

👨‍💻 **Andrés Bianchimano**, Maximiliano  
👨‍💻 **Cernadas**, Nicolás  
👩‍💻 **Correa**, Catalina  
👩‍💻 **Cossettini Reyes**, Dana  
👩‍💻 **Pérez**, Fernanda

## 📚 Vistas incluidas

El proyecto contiene las siguientes pantallas:

- 🔐 **Login**  
  Formulario de acceso para usuarios registrados.

- 📝 **Registro**  
  Formulario de creación de cuenta para nuevos usuarios.

- 📦 **Pedidos**  
  Listado general de pedidos realizados.

- 📄 **Detalle de Pedido**  
  Información específica de un pedido individual.

- 🍕 **Menú**  
  Vista del menú disponible con platos ofrecidos por el local.

- ✏️ **Edición de Plato**  
  Formulario para modificar los datos de un plato existente.

- 🧂 **Ingredientes**  
  Listado de ingredientes disponibles en el sistema.

- 🧪 **Edición de Ingrediente**  
  Formulario para editar o actualizar un ingrediente.

- 🏪 **Perfil del Local**  
  Información del local gastronómico, incluyendo datos de contacto y configuración.

---

## 🛠️ Tecnologías utilizadas

- **Svelte**
- **TypeScript**  
- **Kotlin**
- **SpringBoot**
- **Gradle**
- **Vite**  


---
