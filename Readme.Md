¿Qué es un repositorio en Git y cómo se diferencia de un proyecto "normal"?

Un repositorio en Git es un contenedor donde se guarda el historial completo de un proyecto, incluyendo todas las versiones y los cambios realizados en los archivos. A diferencia de un proyecto "normal", un repositorio Git mantiene el control de versiones, lo que permite rastrear y revertir cambios, colaborar con otros, y gestionar versiones de manera eficiente.

Las tres áreas principales de Git:

Working Directory: Es el área donde trabajas, los archivos modificados que no han sido aún registrados por Git.

Staging Area (Index): Es el área intermedia donde preparas los cambios antes de realizar un commit. Usas git add para mover los cambios aquí.

Repository: Es la base de datos de Git donde se guardan los commits (la historia completa de tu proyecto). Aquí se guarda el historial de cambios.

¿Cómo representa Git los cambios internamente?
Git usa varios tipos de objetos:

Blob: Representa el contenido de un archivo.

Tree: Representa un directorio, contiene punteros a otros objetos (archivos o directorios).

Commit: Representa un snapshot o versión del proyecto. Incluye un puntero al árbol de directorios y metainformación como el autor y mensaje.

Tag: Es una referencia a un commit específico, generalmente usada para marcar versiones importantes.

¿Cómo se crea un commit y qué información almacena un objeto commit?
Un commit se crea con git commit. El objeto commit almacena:

Puntero al árbol de directorios (snapshot).

Metainformación como el autor, fecha y mensaje de commit.

Un puntero al commit anterior (referencia al historial).

Diferencia entre git pull y git fetch:

git pull: Trae los cambios del repositorio remoto y los fusiona (merge) automáticamente con tu rama local.

git fetch: Solo descarga los cambios del remoto, pero no los fusiona automáticamente. Te permite revisar cambios antes de integrarlos.

¿Qué es un branch (rama) en Git?
Un branch (rama) es una línea paralela de desarrollo en Git. Puedes hacer cambios en una rama sin afectar el proyecto principal. Git gestiona ramas usando punteros a los commits más recientes de cada rama.

¿Cómo se realiza un merge y qué conflictos pueden surgir?
Un merge une dos ramas. Si Git no puede fusionar automáticamente los cambios (por ejemplo, si dos ramas modifican la misma línea de código), surge un conflicto. Los conflictos se resuelven editando el archivo afectado y luego marcándolo como resuelto con git add.

¿Cómo funciona el área de staging (git add)?
git add mueve los cambios del directorio de trabajo al área de staging. Si omites este paso, Git no incluirá esos cambios en el siguiente commit.

¿Qué es el archivo .gitignore?
Es un archivo que le dice a Git qué archivos o carpetas debe ignorar y no seguir. Se usa para evitar que se agreguen archivos temporales, logs, o configuraciones específicas de la máquina.

Diferencia entre git commit --amend y un nuevo commit:
git commit --amend modifica el último commit (puedes cambiar el mensaje o agregar cambios). Crear un nuevo commit crea una entrada separada en el historial.

¿Cómo se utiliza git stash?
git stash guarda temporalmente los cambios no comprometidos para que puedas trabajar en otra cosa y luego recuperarlos con git stash pop.

Mecanismos para deshacer cambios:

git reset: Deshace commits o mueve el puntero de la rama.

git revert: Crea un nuevo commit que revierte los cambios de un commit anterior.

git checkout: Cambia de rama o restaura archivos a un estado anterior.

Configuración de remotos (origin, upstream):

origin: El repositorio remoto por defecto.

upstream: En un fork, se refiere al repositorio original.

Comandos comunes para forks: git remote add, git pull, git push.

Inspeccionar historial de commits:

git log: Muestra el historial de commits.

git diff: Muestra las diferencias entre cambios.

git show: Muestra información detallada sobre un commit.

Programación en Java:

Tipos de datos primitivos en Java:

byte, short, int, long (enteros)

float, double (decimales)

char (carácter)

boolean (verdadero/falso)

Estructuras de control de flujo en Java:

if/else: Para decisiones condicionales.

switch: Selección entre múltiples opciones.

for, while, do-while: Bucles de repetición.

Importancia de nombres significativos:
Usar nombres descriptivos mejora la legibilidad del código, facilita su mantenimiento y reduce el riesgo de errores.

¿Qué es la Programación Orientada a Objetos (POO)?
La POO es un paradigma de programación que organiza el código en "objetos" que representan entidades del mundo real y agrupan tanto datos como comportamientos.

Cuatro pilares de la POO:

Encapsulamiento: Ocultar detalles internos y exponer solo lo necesario.

Abstracción: Ocultar complejidad y mostrar solo la interfaz relevante.

Herencia: Crear nuevas clases basadas en clases existentes.

Polimorfismo: Permitir que una misma interfaz sea utilizada para diferentes tipos de objetos.

¿Qué es la herencia en POO y cómo se utiliza en Java?
La herencia permite que una clase derive de otra, heredando sus propiedades y comportamientos. Se usa con la palabra clave extends.

Modificadores de acceso en Java:

public: Acceso desde cualquier lugar.

private: Acceso solo dentro de la clase.

protected: Acceso dentro del paquete o en subclases.

default (sin modificador): Acceso solo dentro del paquete.

Variable de instancia:
Es una variable que pertenece a una instancia de una clase. Se declara dentro de la clase pero fuera de los métodos.
