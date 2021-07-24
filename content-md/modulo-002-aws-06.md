# Módulo 2 - Grupos de Seguridad AWS

![](../aws-images/aws-modulo-02/m2-sprincipales-aws-026.png)

Una breve introducción a los grupos de seguridad de **AWS**. 

![](../aws-images/aws-modulo-02/m2-sprincipales-aws-027.png)

La seguridad de la nube de **AWS** es una de las prioridades más altas de **Amazon Web Services**, y ofreceremos numerosas opciones de seguridad sólidas para ayudarlo a proteger sus datos en la nube de **AWS**. 
Una de las características de las que se debe mencionar son los grupos de seguridad.

![](../aws-images/aws-modulo-02/m2-sprincipales-aws-028.png)

En **AWS** los grupos de seguridad actúan como un firewall integrado para sus servidores virtuales. Con estos grupos de seguridad, tiene el control completo sobre la accesibilidad de sus instancias. 
En el nivel más básico, es sólo otro método para filtrar el tráfico a las instancias. Le permite decidir de qué tráfico permitir o denegar. Para determinar quién tiene acceso a sus instancias, configurará una regla para los grupos de seguridad. Las reglas pueden variar desde mantener a la instancia completamente privada, pública o en un estado intermedio. 

Si comenzamos en la capa web, vera que existen reglas para establecer una regla para aceptar el tráfico que viene de cualquier parte de Internet en el puerto 80/443 al seleccionar la fuente 0.0.0.0/0

Si nos movemos a la capa de aplicación vemos un grupo de seguridad que sólo acepta el tráfico de la capa web, y, de forma similar, la capa de base de datos sólo puede aceptar el tráfico de la capa de aplicación. Por último, existen también reglas para permitir la administración de forma remota desde la red corporativa mediante el puerto SSH 22.