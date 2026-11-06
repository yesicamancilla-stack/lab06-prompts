
# Bitacora de prompts

Laboratorio 06: Fundamentos de Ingenieria de Prompts.

Herramienta de IA usada: ChatGPT

## Ejercicio 2: Tokens y ventana de contexto

| Texto | Caracteres | Tokens |
|-------|------------|--------|
| Los estudiantes programan en Java. | 35 | 7 |
| The students program in Java. | 30 | 6 |
| desafortunadamente | 18 | 4 |


### Observaciones sobre la ventana de contexto

En el mismo chat, ChatGPT recordo que mi aplicacion se llamaba TiendaTec y utilizaba Java Swing porque esa informacion estaba en la conversacion.

Al abrir un chat nuevo, ChatGPT tambien respondio correctamente. Esto puede deberse a que tiene una funcion de memoria que permite recordar informacion de otras conversaciones.


## Ejercicio 3: Temperatura

| Temperatura | % de BiblioTec | Nombres en los 5 intentos |
|-------------|----------------|---------------------------|
| 0 | 100 % | BiblioTec, BiblioTec, BiblioTec, BiblioTec, BiblioTec |
| 0.5 | 65.3 % | PrestaLibro, BiblioTec, BiblioTec, BiblioTec, LibroYa |
| 1 | 44.5 % | NubeDeTinta, LibroYa, LibroYa, LectoGo, LibroYa |
| 1.8 | 32.2 % | LibroYa, NubeDeTinta, PaginaLibre, LibroYa, LibroYa |

### Observaciones

Al aumentar la temperatura, los nombres fueron mas variados y BiblioTec tuvo menos probabilidad de salir.

El simulador nunca invento nombres nuevos porque solo puede elegir entre las seis opciones que estan escritas en el codigo.

Al repetir la temperatura 1.8, los porcentajes fueron iguales, pero los nombres elegidos cambiaron.


## Ejercicio 4: Prompt vago vs estructurado


| Criterio | Prompt vago | Prompt estructurado |
|----------|-------------|---------------------|
| Menciona el objetivo del sistema | Si | Si |
| Menciona a los usuarios principales | Si | Si |
| Tiene exactamente 3 funcionalidades | No | Si |
| Esta en 3 parrafos | No | Si |
| Lo usaria en un informe real | No | Si |

### Comparacion

El prompt vago genero una descripcion general del sistema, pero no organizo la informacion como necesitaba.

El prompt estructurado dio una respuesta mas clara y ordenada porque indique el objetivo, los usuarios, las funcionalidades y el formato.


## Ejercicio 5: Anatomia de un prompt

### Componentes del prompt final

| Componente | Texto de mi prompt |
|------------|--------------------|
| Rol | Actua como desarrollador Java. |
| Instruccion | Crea un programa en Java usando una clase Producto con los atributos codigo, nombre, precio y stock. |
| Contexto | Para gestionar los productos de una tienda. |
| Ejemplo | Usa este estilo para los metodos: getPrecio(), setPrecio(double precio). |
| Formato | Explica primero la estructura de la clase y luego presenta el codigo Java. |

### Cambios en cada nivel

**Nivel 1:** La IA creo un programa sencillo que mostraba Hola mundo.

**Nivel 2:** Al agregar el rol de desarrollador Java, la IA creo una calculadora con operaciones matematicas.

**Nivel 3:** Al agregar el contexto, la IA creo un programa para gestionar productos de una tienda.

**Nivel 4:** Al indicar los atributos, la IA creo una clase Producto con codigo, nombre, precio y stock.

**Nivel 5:** Al agregar el formato, la IA explico primero la estructura de la clase y despues mostro el codigo Java.

**Ejemplo adicional:** Al agregar ejemplos de metodos, la IA utilizo getters y setters para consultar y modificar los atributos.

