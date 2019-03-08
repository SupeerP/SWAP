# Tema 2. Alta disponibilidad y escalabilidad

## Introducción

Disponibilidad y escalabilidad son los dos conceptos más importantes al diseñar una granja web.

El éxito de una empresa depende de que los usuarios tengan una buena experiencia la visitarla. Nuestros servidores deben dar el mejor servicio a todos los usuarios y deben estar todo el tiempo disponible (24/7)

Por otro lado, está el concepto de escalabilidad. Si más y más usuarios van solicitando el servicio, que este sea capaz de responder a todos, adaptandose a las peticiones realizadas.

## Concepto de alta disponibilidad

Cuando un sitio no está disponible se die que se ha caído o sufre un problma de no-disponibilidad.

- Tiempo de no-disponibilidad **programado**. Está bajo nuestro control (Ej, cambiarle el ventilador a una máquina)
- Tiempo de no-disponibilidad **no programado**. No está bajo control y tenemos que tener cuidado (Ej, rotura del disco, calentamiento de la placa...)

Solo debería haber "tiempos de no-disponibilidad programados" (y lo más cortos posible).

Es necesario **medir** la disponibilidad dando un porcentaje, con orientación a marketing. Esto se realiza con el nombre de **escala punto nueve**. La fórmula sería la siguiente

`100 - (tiempoCaido / periodoTiempo) * 100`

Un 100% de disponibilidad es no sufrir caidas no programadas.

Para calcular la disponibilidad de un sistema es:

` As = Ac1 * Ac2 * ... * Acn`

Si tenemos un servidor (web/BD) si se ha caido la web, el usuario igualmente no puede acceder a la BD, asi que es como si se hubiesen caido los 2.

Para mejorar esto es por ejemplo añadir un segundo servidor web, haciendo:

`disponibilidad_web2 = 85% + (1-85%) * 85% = 97.75%`

La encuación general sería:

`As = Acn-1 (1-Acn-1) * Acn`

El uso de **subsistemas redundantes** y monitorizarlos mejora la disponibilidad del sistema global. Surgen conceptos como:
- Disponibilidad de red
- Disponibilidad del servidor
- Disponibilidad de las aplicaciones

Nota: Ejercicio T2.2-> Buscar frameworks y librerías para diferentes lenguajes que permitan hacer aplicaciones altamente disponibles con relativa facilidad. Como ejemplo, examina [PM2](https://github.com/Unitech/pm2)

## Concepto de escalabilidad

Vemos que hay dos tipos de escalado:
- Ampliación vertical, incrementando la RAM, CPI, disco de un servidor
- Ampliación horizontal, dividiendo el trabajo entre diferentes máquinas.


## Escalar un sitio web



## Conclusiones