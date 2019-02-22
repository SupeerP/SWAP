# Tema 1. Introducción

Para empezar la asignatura vamos a suponer que hemos terminado la carrera, estamos trabajando y una empresa nos ha pedido que realicemos el despliegue de un servidor web. Entonces tenemos 2 opciones:

- Trabajar mucho al inicio y tras esto vivir después sin preocupaciones
- Empezar de manera rápida siendo necesario  de manera obligatoria el mantenimiento y mejora de este

Para empezar el planteamiento necesitaríamos:
- Montar un servidor en una máquina
- Adquirir un segundo servidor para desarrollo y testeo del servidor
- Segundo servidor para sustituir el principal debido a cualquier percance de la primera

Otra opción sería realizar una **Granja Web**.

Para entenderlo mejor, existe un balanceador de carga y puede darse el aso que cada servidor este destinado a una cosa específica, como uno estático, otro de gestión de BD...

![Web-farm](../img/web-farm-t1.png)

## Conceptos básicos

En cada uno de esos grupos de máquinas se puede instalar diferente tipo de aplicaciones, como he dicho anteriormente, siendo cada uno de esos más eficiente para un tipo de servicio.

## Un sitio web mal planificado

Este ejemplo sería debido a querer realizar el trabajo de manera rápida y con el menor coste posible, realizando la instalación de todos los servicios en una sola máquina.

![Overload-Icon](../img/overload-icon-t1.png)

Esto lo malo que se sobrecargaría el servidor cuando empiece a atender más solicitudes. Esto daría lo mismo que tuviesemos la mejor máquina, ya que habrá un punto que esta no pueda realizar las respuestas.

