# Módulo 4 - Tolerancia a errores y alta disponibilidad

![](../aws-images/aws-modulo-04/m4-sprincipales-aws-014.png)

Para comenzar, veamos los significados detrás de la tolerancia a errores y la alta disponibilidad.

La **tolerancia es errores** es la capacidad de un sistema para seguir funcionando, incluso si algunos de sus componentes presentan errores. Puede verse como la redundancia integrada de los componentes de una aplicación.

![](../aws-images/aws-modulo-04/m4-sprincipales-aws-015.png)

Luego, veamos la **alta disponibilidad**,  un concepto que se refiere a todo el sistema. Su objetivo es garantizar que los sistemas estén siempre en funcionamiento y disponibles, y que el tiempo de inactividad se minimice lo más posible, sin necesidad de intervención humana. Aunque un sitio no esté disponible durante un minuto, puede ser perjudicial para un negocio. Sin embargo, Amazon Web Service proporciona herramientas que pueden ayudar en estos momentos de necesidad.  La plataforma de **AWS** está disponible para que los usuarios creen sistemas y arquitecturas con alta disponibilidad y tolerancia a los errores. **AWS** es un servicio único porque los usuarios pueden crear estos sistemas con mínima interacción humana e inversión económica inicial; todo esto se puede ajustar a sus necesidades.

![](../aws-images/aws-modulo-04/m4-sprincipales-aws-016.png)

Comparemos la disponibilidad de las ubicaciones en las instalaciones y en **AWS**. Antes, garantizar una alta disponibilidad en su centro de datos local podía ser muy costoso y, por lo general, sólo se lograba en aplicaciones completamente críticas para la misión. Sin embargo, en **AWS**, tiene las opciones para ampliar la disponibilidad y la capacidad de recuperación entre los servicios que elija. Puede garantizar una alta disponibilidad en varios servidores, en varias zonas de disponibilidad dentro de cada región y en varias regiones. Además, tiene acceso a servicios tolerantes a errores para utilizarlos como quiera.

![](../aws-images/aws-modulo-04/m4-sprincipales-aws-017.png)

Analicemos en mayor profundidad cómo algunos servicios específicos pueden ayudar a proporcionar alta disponibilidad. Veamos lo siguiente: 

![](../aws-images/aws-modulo-04/m4-sprincipales-aws-018.png)

- **Balanceadores de Carga Elásticos, ELB**
- **Direcciones IP elásticas** 
- **Amazon Route 53**
- **Auto Scaling**
- **Amazon CloudWatch**

En primer lugar, **los balanceadores de carga elástica**, o **ELB**, ofrecen un servicio que distribuye el tráfico o las cargas entrantes en sus instancias. **ELB** también puede enviar métricas a **Amazon CloudWatch**, qué es un servicio de monitoreo administrado. Examinaremos más información sobre este tema más adelante en el módulo. **ELB** puede ser un desencadenador y notificarlo si ocurre una alta latencia o si los servidores se están utilizando en exceso. **ELB** también se puede personalizar. Por ejemplo, puede configurarlo para que reconozca instancias **EC2** en mal estado. Puede hacerlo de manera pública o interna. Por último, puede utilizar varios protocolos diferentes.

![](../aws-images/aws-modulo-04/m4-sprincipales-aws-019.png)

A Continuación, veamos las **direcciones IP elásticas**. Las **direcciones IP elásticas** son útiles para proporcionar una mayor tolerancia a errores en su aplicación. Las **direcciones IP  elásticas** son direcciones IP estáticas diseñadas para la informática en la nube dinámica. Con esta herramienta, es posible ocultar el error de una instancia o software porque permite a los usuarios utilizar las mismas direcciones IP con recursos de sustitución. El uso de direcciones IP elásticas garantiza una alta disponibilidad, y ya que los clientes pueden acceder a la aplicación aunque hubiera un error en la instancia. 

![](../aws-images/aws-modulo-04/m4-sprincipales-aws-020.png)

Otro servicio es **Amazon Route 53**. **Amazon Route 53** es un servicio de DNS autorizado de **AWS**. Se utiliza para traducir los nombres de dominio a direcciones IP. El diseño y el mantenimiento de **Amazon Route 53** cuentan con el nivel más alto de disponibilidad. Se ha desarrollado para admitir el direccionamiento sencillo, el direccionamiento pasado en latencia, las comprobaciones de estado y las conmutaciones por error a nivel de DNS y el direccionamiento de geolocalización. Todas estas características aumentan la disponibilidad de las aplicaciones orientadas al cliente.

![](../aws-images/aws-modulo-04/m4-sprincipales-aws-021.png)

**Auto Scaling** lanza o termina instancias en función de las condiciones especificadas. Este servicio está diseñado para ayudarlo a crear un sistema flexible que se pueda ajustar y modificar según los cambios en la demanda del cliente. Con el escalado automático, puede evitar las limitaciones de la creación manual de nuevos recursos. Por el contrario, puede crear nuevos recursos bajo demanda o tener un aprovisionamiento programado. Esto garantiza que sus aplicaciones y sistemas están siempre disponibles, independientemente de cuál sea la carga. También es importante tener en cuenta que puede configurar aprovisionamientos para escalar en forma ascendente o descendente, en función de sus políticas.

![](../aws-images/aws-modulo-04/m4-sprincipales-aws-022.png)

Por último, veamos **Amazon CloudWatch**. Amazon CloudWatch es un sistema distribuido de recopilación de estadísticas. Recopila y hace un seguimiento de las métricas de sus aplicaciones. Otra característica es que tiene la capacidad de crear y utilizar sus propias métricas personalizadas. Si hay latencia o métricas altas que han superado el umbral establecido, CloudWatch puede ejecutarse automáticamente para garantizar la alta disponibilidad de su arquitectura. 

![](../aws-images/aws-modulo-04/m4-sprincipales-aws-023.png)

Veamos algunas herramientas tolerantes a errores. 

![](../aws-images/aws-modulo-04/m4-sprincipales-aws-024.png)

En primer lugar, **Amazon Simple Queue Service**, o **Amazon SQS**, que puede utilizarse como la red troncal de su aplicación tolerante a errores. Es un sistema de mensajería distribuida de gran confianza. **Amazon SQS** puede ayudarlo a garantizar que la cola esté siempre disponible.

A continuación, veamos **Amazon Simple Storage Service** o **Amazon S3**, que proporciona almacenamiento de datos de larga duración y tolerante a errores. Es un servicio web sencillo que puede utilizar y en cualquier lugar, paga únicamente por el almacenamiento que utilice. **Amazon S3** almacena todos los datos de forma redundante en varios dispositivos diferentes en varias instalaciones de una región, por lo que si se produjera un error, seguiría teniendo acceso a toda la información.

Ahora, analicemos **Amazon Relational Database Service**, o **Amazon RDS**, que es otra herramienta de servicio web para que utilice en las bases de datos relacionales. Proporciona alta disponibilidad y tolerancia a errores porque ofrece varias características orientadas a mejorar la fiabilidad de sus bases de datos críticas.

Entre las características, se incluyen copias de seguridad automatizadas, instancias e implementaciones en varias zonas de disponibilidad. Todos estos servicios diferentes son herramientas de gran confianza, de larga duración y con tolerancia a errores para sus aplicaciones a fin de garantizar una alta disponibilidad y contar con sistemas tolerantes a errores.

Construir una arquitectura con alta disponibilidad y tolerancia a errores no tiene porqué ser difícil. Con la plataforma de **AWS**, puede utilizar los servicios y las herramientas que se ofrecen para garantizar que sus aplicaciones y sistemas tengan alta disponibilidad y mayor tolerancia a errores. Para obtener información más detallada sobre los de servicios y arquitecturas con alta disponibilidad y tolerancia a errores, puede consultar: https://aws.amazon.com/