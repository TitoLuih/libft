# Libft - 42 Cursus

Libft es el primer proyecto del cursus de 42. El objetivo de este proyecto es crear una biblioteca de funciones en C que replican el comportamiento de funciones de la librería estándar de C, así como otras funciones útiles que podrán ser reutilizadas en proyectos futuros.

## Tabla de contenidos
- [Introducción](#introducción)
- [Estructura del proyecto](#estructura-del-proyecto)
- [Compilación](#compilación)
- [Uso](#uso)
- [Funciones implementadas](#funciones-implementadas)
- [Evaluación](#evaluación)
- [Créditos](#créditos)

---

## Introducción
Libft es un proyecto que busca desarrollar habilidades fundamentales en programación C, como el manejo de memoria, punteros y estructuras. Crearás tu propia librería personalizada con funciones que podrás incluir en futuros proyectos simplemente enlazándola durante la compilación.

## Estructura del proyecto
El repositorio tiene la siguiente estructura:

```
.
|-- libft.h          // Archivo de cabecera principal
|-- Makefile         // Archivo para automatizar la compilación
|-- src/             // Directorio que contiene las implementaciones de las funciones
|-- obj/             // Directorio para los archivos objeto generados durante la compilación
|-- tests/           // Scripts y programas de prueba (opcional)
```

## Compilación
Para compilar la biblioteca, simplemente ejecuta el siguiente comando en la terminal:

```bash
make
```
Esto generará un archivo `libft.a` que podrá ser enlazado en tus futuros proyectos.

Para limpiar los archivos objeto generados durante la compilación, puedes usar:

```bash
make clean
```

Si también deseas eliminar el archivo `libft.a`, usa:

```bash
make fclean
```

Puedes recompilar desde cero utilizando:

```bash
make re
```

## Uso
Para usar tu librería en un proyecto, incluye el archivo de cabecera `libft.h` y enlaza `libft.a` durante la compilación. Por ejemplo:

```bash
gcc -Wall -Wextra -Werror main.c -L. -lft -o programa
```

## Funciones implementadas
Libft incluye varias categorías de funciones:

### Funciones de la librería estándar
- **isalpha**: Comprueba si un carácter es alfabético.
- **isdigit**: Comprueba si un carácter es un dígito.
- **isalnum**: Comprueba si un carácter es alfanumérico.
- **...** (y otras similares).

### Manejo de cadenas
- **strlen**: Calcula la longitud de una cadena.
- **strcpy**: Copia una cadena.
- **strdup**: Duplica una cadena.

### Manejo de memoria
- **memset**: Llena una región de memoria con un valor.
- **memcpy**: Copia bloques de memoria.
- **calloc**: Asigna memoria inicializada a cero.

### Funciones adicionales
- **ft_itoa**: Convierte un entero en una cadena.
- **ft_split**: Divide una cadena en un array de cadenas usando un delimitador.
- **ft_strjoin**: Concatena dos cadenas.

Para más detalles sobre las funciones implementadas, revisa el archivo `libft.h`.

## Evaluación
Durante la evaluación, se comprobará:
1. El correcto funcionamiento de cada función.
2. El cumplimiento de las normativas de estilo de código de 42 (Norminette).
3. La eficiencia y robustez del código.

Asegúrate de probar tu librería exhaustivamente antes de enviarla para la evaluación.

## Créditos
Este proyecto fue desarrollado como parte del programa 42 Cursus.

Para preguntas o sugerencias, no dudes en contactar conmigo.
