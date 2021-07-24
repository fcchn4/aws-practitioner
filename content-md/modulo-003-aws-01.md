# Módulo 3 - Balanceador de Carga de Aplicaciones

![](../aws-images/aws-modulo-03/m3-sprincipales-aws-002.png)

En esta oprtunidad presentaremos el segundo tipo de balanceador de carga en el servicio **Elastic Load Balancing (ELB)**, que es el **Balanceador de carga de aplicaciones**.

¿Qué es el balanaceador de carga? Cómo se mencionó antes, el **Balanceador de carga de aplicaciones** es el segundo tipo de balanceador de carga introducido como parte del servicio **Elastic Load Balancing**. Ofrece la mayoría de las características que proporciona el Balanceador de carga clásico, pero agrega algunas características y mejoras importantes que lo hacen adecuado para casos de uso únicos.

![](../aws-images/aws-modulo-03/m3-sprincipales-aws-003.png)

De forma breve algunas de las características mejoradas de manera reciente incluyen compatibilidad con más protocolos de **solicitud**, **métricas** y **registros de acceso mejorados**, y **más comprobaciones de estado de destino**. Algunas de las características adicionales del **Balanceador de carga de aplicaciones** son la capacidad de habilitar más mecanismos de direccionamiento para su solicitud mediante el direccionamiento basado en **ruta** o **host**, la compatibilidad nativa con **IPV6** en **VPC**, la **integración a firewall** para aplicaciones web de **AWS** y mucho más.

![](../aws-images/aws-modulo-03/m3-sprincipales-aws-004.png)

Hay muchas situaciones en las que puede utilizar el **Balanceador de carga de aplicaciones**.  Una es, la capacidad de utilizar contenedores para alojar sus microservicios y direccionarlos a esas aplicaciones desde un único **Balanceador de carga**. El **Balanceador de carga de aplicaciones** le permite direccionar distintas solicitudes a la misma instancia, pero con distintas rutas basadas en puertos. Si tiene diferentes contenedores que escuchan varios puertos, puede configurar reglas de direccionamiento para distribuir el tráfico sólo a la  aplicación de backend deseada.

![](../aws-images/aws-modulo-03/m3-sprincipales-aws-005.png)

Hay algunos términos nuevos que aprender cuando se analiza el **Balanceador de carga de aplicaciones**. Aunque los agentes de escucha sean básicamente los mismos, ahora puede agrupar los **destinos** en **grupos de destino**. Dado que el **Balanceador de carga de aplicaciones** registra distintos destinos en lugar de instancias, un grupo de destino es la forma en la que se registran los destinos en el **Balanceador de carga**. Aquí podemos ver cómo el **Balanceador de carga de aplicaciones** direcciona y organiza los destinos de backend. Cuando configura los agentes de escucha para el **Balanceador de carga**, crea **reglas** a fin de determinar la forma en la que las solicitudes recibidas por el **Balanceador de carga** se direccionan a los destinos de backend. Para registrar esos destinos en el **Balanceador de carga** y configurar la comprobación de estado que esté utilizará para los destinos, se crean grupos de destino. Como vemos en las imágenes los destinos también pueden ser miembros de varios grupos de destino.

![](../aws-images/aws-modulo-03/m3-sprincipales-aws-006.png)

Cómo se mencionó anteriormente, el **Balanceador de carga de aplicaciones** incluye características mejoradas y agregadas. En el **Balanceador de carga de aplicaciones**, se ha mejorado la compatibilidad con protocolos al agregar compatibilidad con HTTP/2 y Websockets. Además, se incrementaron las capacidades de monitoreo con más dimensiones de métricas, la realización de comprobaciones de estado más detalladas y detalles adicionales en los registros de acceso. Algunas de las características agregadas son el direccionamiento basado en **ruta** y en **host**. El **direccionamiento basado en ruta** le permite crear reglas para direccionar a grupos de destino en función de la URL de la solicitud. El **direccionamiento basado en host** permite tener varios dominios compatibles con el mismo balanceador de carga y direccionar las solicitudes a los grupos de destino en función del dominio solicitado. 

![](../aws-images/aws-modulo-03/m3-sprincipales-aws-007.png)

Además, obtiene la capacidad de utilizar el seguimiento de las solicitudes de los clientes a los destinos y la capacidad de habilitar puertos de host dinámicos cuando se utilizan contenedores programados en **EC2 Container Service**.

![](../aws-images/aws-modulo-03/m3-sprincipales-aws-008.png)