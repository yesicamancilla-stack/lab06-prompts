
# Tarea: Mi prompt profesional

## Funcionalidad elegida

Registro de estudiantes y calculo de notas en Java.

## Version 1: prompt basico

```text
Crea un programa en Java para registrar estudiantes.
```

**Que cambie:** Escribi una instruccion basica.

**Por que:** Queria comprobar que programa generaba la IA sin darle muchos detalles.

**Resultado:** La IA creo un registro de estudiantes con codigo, nombre, edad y carrera, pero no calculaba notas.

## Version 2

```text
Actua como desarrollador Java. Crea un programa para registrar estudiantes con codigo, nombre y tres notas. El programa debe calcular el promedio de las notas y mostrar si el estudiante aprobo o desaprobo. La nota minima aprobatoria es 11.
```

**Que cambie:** Agregue un rol y especifique los datos y calculos necesarios.

**Por que:** La primera version no calculaba los promedios.

**Que mejoro:** La IA incluyo tres notas, el calculo del promedio y el estado del estudiante.

## Version 3: prompt final

```text
Actua como desarrollador Java. Crea un programa de consola para registrar estudiantes con codigo, nombre y tres notas de 0 a 20. El programa debe calcular el promedio y mostrar si el estudiante aprobo con 11 o mas, o desaprobo.

Utiliza una clase Estudiante y metodos con nombres como calcularPromedio() y obtenerEstado().

Explica primero los atributos y metodos, luego muestra el codigo Java completo y un ejemplo de ejecucion.

No utilices librerias externas y valida que las notas esten entre 0 y 20.
```

**Que cambie:** Agregue ejemplos de metodos, el formato de respuesta y restricciones.

**Por que:** Queria obtener un programa mas completo, organizado y con validacion de notas.

**Mejora que debo comprobar:** El programa debe validar las notas, calcular el promedio y presentar una explicacion antes del codigo.

## Componentes del prompt final

| Componente | Texto de mi prompt |
|------------|--------------------|
| Rol | Actua como desarrollador Java. |
| Instruccion | Crea un programa de consola para registrar estudiantes con codigo, nombre y tres notas de 0 a 20. |
| Contexto | El programa debe calcular el promedio y mostrar si el estudiante aprobo con 11 o mas, o desaprobo. |
| Ejemplo | Metodos con nombres como calcularPromedio() y obtenerEstado(). |
| Formato | Explica primero los atributos y metodos, luego muestra el codigo Java completo y un ejemplo de ejecucion. |

**Restricciones:** No utilizar librerias externas y validar las notas entre 0 y 20.

## Evaluacion del resultado

| Criterio | Cumple |
|----------|--------|
| Registra estudiantes | Por verificar |
| Calcula el promedio de tres notas | Por verificar |
| Muestra aprobado o desaprobado | Por verificar |
| Valida notas entre 0 y 20 | Por verificar |
| Explica primero la estructura | Por verificar |
| No utiliza librerias externas | Por verificar |

## Errores que evite

**Error 1: Ser demasiado general.**

En la primera version no indique todas las funciones. Lo corregi especificando las notas y el promedio.

**Error 2: No indicar el formato.**

Al inicio no explique como queria recibir la respuesta. En la version final pedi primero la explicacion y despues el codigo.
