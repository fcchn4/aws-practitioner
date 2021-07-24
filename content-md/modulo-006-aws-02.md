# Módulo 6 - Información sobre precios

![](../aws-images/aws-modulo-06/m6-sprincipales-aws-004.png)

El pago de los servicios de AWS incluye estas tres características fundamentales:

- Informática 
- Almacenamiento 
- Transferencia saliente de datos

![](../aws-images/aws-modulo-06/m6-sprincipales-aws-005.png)

Estas características varían en función del producto de AWS que utilice. Sin embargo, estos son los factores principales que más afectan los costos.

Aunque se le cobra por la transferencia saliente de datos, no se aplican cargos por la transferencia entrante de datos y la que se realiza entre otros servicios de AWS de la misma región. La transferencia saliente de datos se suma en Amazon EC2, Amazon S3, Amazon RDS, Amazon SimpleDB, Amazon SQS, Amazon SNS y Amazon VPC, y después se cobra en función de la tarifa de transferencia saliente de datos. Este monto aparece en el extracto mensual como AWS Data Transfer Out (Transferencia saliente de datos de AWS).

![](../aws-images/aws-modulo-06/m6-sprincipales-aws-006.png)

Desglosemos las características de precios de los productos de AWS de uso común: Amazon Elastic Compute Cloud (Amazon EC2),  Amazon Simple Storage Service (Amazon S3), Amazon Elastic Block Store (Amazon EBS), Amazon Relational Database Service (Amazon RDS) y Amazon CloudFront.

Primero, analizaremos Amazon Elastic Compute Cloud (Amazon EC2).

![](../aws-images/aws-modulo-06/m6-sprincipales-aws-007.png)

Amazon EC2 es un servicio web que proporciona capacidad de cómputo de tamaño modificable en la nube. La sencilla interfaz de servicios web de Amazon EC2 permite obtener y configurar su capacidad con una fricción mínima. Proporciona un control completo sobre los recursos informáticos en el entorno informático acreditado de Amazon. Amazon EC2 cambia el modelo económico de la informática y permite pagar sólo por la capacidad que realmente se utiliza.

![](../aws-images/aws-modulo-06/m6-sprincipales-aws-008.png)

Para comenzar a estimar el costo de Amazon EC2 debe tener en cuenta lo siguiente:

- Horas reloj del tiempo de servicio. El hecho de que los recursos incurren en cargos cuando se ejecutan. Por ejemplo, se generan cargos desde el momento en que se lanzan las instancias de Amazon EC2 hasta el momento en que se terminan, o bien desde el momento en que se asignan las IP elásticas hasta el momento en que se cancela su asignación. 
- Configuración de la máquina. Tenga en cuenta la capacidad física de la instancia de Amazon EC2 que elija. Los precios de las instancias varían en función de la región de AWS, el SO, el número de núcleos y la memoria.

![](../aws-images/aws-modulo-06/m6-sprincipales-aws-009.png)

Con las instancias bajo demanda, paga por la capacidad de cómputo por hora, sin compromisos de uso mínimo. Llas instancias reservadas le ofrecen la opción de realizar un pago único o de no realizar ningún pago inicial por cada instancia que quiera reservar. A cambio, obtiene un importante descuento en el cargo por uso por hora de dicha instancia. En el caso de las instancias de **spot**, puede ofertar por la capacidad de Amazon EC2 que no haya utilizado.

![](../aws-images/aws-modulo-06/m6-sprincipales-aws-010.png)

También debe tener en cuenta el número de instancias y el balanceo de carga.

- Número de instancias. Puede aprovisionar varias instancias de sus recursos de Amazon EC2 y Amazon EBS para gestionar cargas máximas.
- Balanceo de carga: Se puede utilizar un balanceador de carga elástico para distribuir el tráfico entre instancias de Amazon EC2. El costo mensual está determinado por la cantidad de horas durante las cuales se ejecuta el Balanceador de carga elástico y por el volumen de datos que procesa.
- Monitoreo detallado. Puede utilizar Amazon CloudWatch para monitorear sus instancias de Amazon EC2. De forma predeterminada, el monitoreo básico está habilitado y disponible sin costo adicional. Sin embargo por una tarifa mensual fija, puede optar por el monitoreo detallado, que incluye siete métricas preseleccionadas registradas una vez por minuto. Los meses parciales se cobran según un prorrateo por hora, a una tarifa por hora de instancia.
-  Escalado automático. El escalado automático ajusta automáticamente el número de instancias de Amazon EC2 en su implementación según las condiciones que establezca. Este servicio está disponible sin cargo adicional más allá de las tarifas de Amazon CloudWatch.
- Direcciones IP elásticas. Puede tener una dirección IP elástica asociada con una instancia en ejecución sin cargo alguno.

![](../aws-images/aws-modulo-06/m6-sprincipales-aws-011.png)

Sistemas operativos y paquetes de software.

- Los precios del sistema operativo se incluyen en los precios de la instancia. AWS le ha simplificado el camino por medio de su asociación con Microsoft, IBM y otros proveedores para facilitar la ejecución de ciertos paquetes de software comercial en sus instancias de Amazon EC2 (por ejemplo, Microsoft SQL Server en Windows). Para los paquetes de software comercial no provisto por AWS, como los sistemas operativos no estándar, las aplicaciones de Oracle o las aplicaciones de Windows Server, como Microsoft SharePoint y Microsoft Exchange, debe obtener una licencia de los proveedores. También puede llevar su licencia existente a la nube por medio de programas de proveedores específicos, como el programa de movilidad de licencias a través de Software de Assurance de Microsoft. 

![](../aws-images/aws-modulo-06/m6-sprincipales-aws-012.png)

Amazon S3 es almacenamiento para internet.

Proporciona una sencilla interfaz de servicios web que puede utilizarse para almacenar y recuperar la cantidad de datos que quiera, en cualquier momento y desde cualquier parte de la web.

Para comenzar a estimar los costos de Amazon S3, debe tener en cuenta lo siguiente: 

- Clase de almacenamiento. El almacenamiento estándar está diseñado para proporcionar una durabilidad del 99.999999999% y una disponibilidad del 99.99%. Estándar - Acceso poco frecuente, o SIA, es una opción de almacenamiento dentro de Amazon S3 que puede utilizar para reducir los costos mediante el almacenamiento de los datos a los que se accede con menos frecuencia a niveles de redundancia ligeramente inferiores a los del almacenamiento estándar de Amazon S3. Estándar: acceso poco frecuente; está diseñado para proporcionar la misma durabilidad del 99.999999% que Amazon S3 con una disponibilidad del 99.9% en un año determinado. 

![](../aws-images/aws-modulo-06/m6-sprincipales-aws-013.png)

Es importante tener en cuenta que cada clase tiene distintas tarifas.

- Almacenamiento.  También deben tenerse en cuenta la cantidad y el tamaño de los objetos almacenados en los bucket de Amazon S3, y el tipo de almacenamiento.
- Solicitudes. El número y el tipo de las solicitudes. Las solicitudes GET generan cargos a tasas diferentes a las otras solicitudes, como las solicitudes PUT o COPY.
- Transferencia de datos. La cantidad de datos transferidos fuera de la región de Amazon S3.

![](../aws-images/aws-modulo-06/m6-sprincipales-aws-014.png)

Amazon EBS ofrece volúmenes de almacenamiento a nivel de bloques para utilizarlos con instancias de Amazon EC2.

![](../aws-images/aws-modulo-06/m6-sprincipales-aws-015.png)

Los volúmenes de Amazon EBS constituyen almacenamiento fuera de la instancia que persiste independientemente de la vida de una instancia. Son análogos a los discos virtuales en la nube. Amazon EBS ofrece tres tipos de volúmenes:
- Uso general (SSD) 
- IOPS provisionados (SSD)
- Magnéticos 

![](../aws-images/aws-modulo-06/m6-sprincipales-aws-016.png)

Los tres tipos de volúmenes difieren en las características del rendimiento y el costo, con lo que puede elegir el rendimiento y el precio idóneo de almacenamiento para sus aplicaciones.

![](../aws-images/aws-modulo-06/m6-sprincipales-aws-017.png)

Para comenzar a estimar el costo de Amazon EBS, debe tener en cuenta lo siguiente:

- Volúmenes. El almacenamiento de volúmenes para todo tipo de volúmenes de Amazon EBS se cobra en función de la cantidad de GB que aprovisione al mes hasta que liberen la capacidad almacenada.
- Operaciones de entrada y salida por segundo (IOPS). Las operaciones de entrada y salida E/S están incluidas en el precio de los volúmenes de uso general, mientras que para los volúmenes EBS, las operaciones de E/S se cobran en función de la cantidad de solicitudes que efectúe al volumen. Los volúmenes de IOPS provisionadas también se cobran en función de la cantidad que aprovisione en IOPS (multiplicada por el porcentaje de días aprovisionados al mes).
-  Instancia. Amazon EBS le brindan la posibilidad de realizar copias de seguridad como instancias de datos en Amazon S3 para que pueda recuperarlos a largo plazo. Si opta por las instancias de EBS, el costo adicional es por gigabyte al mes de datos almacenados. 
- Transferencia de datos. Tenga en cuenta la cantidad de datos transferidos desde su aplicación. La transferencia entrante de datos es gratuita, y los cargos por la transferencia saliente de datos se aplican por niveles.

Amazon RDS es un servicio web que facilita las tareas de configuración, operación y escalado de una base de datos relacional en la nube.

![](../aws-images/aws-modulo-06/m6-sprincipales-aws-018.png)

Proporciona capacidad rentable y de tamaño modificable, y se ocupa de las tareas de administración de base de datos que llevan mucho tiempo, lo que le permite centrarse en sus aplicaciones y negocio.

![](../aws-images/aws-modulo-06/m6-sprincipales-aws-019.png)

Para comenzar a estimar el costo de Amazon RDS, debe tener en cuenta lo siguiente:

- Horas reloj del tiempo del servidor. El hecho de que los recursos incurren en cargos cuando se ejecutan. Por ejemplo, el tiempo que transcurre desde que lanza una instancia de base de datos hasta que la termina.
- Características de la base de datos. La capacidad física de la base de datos que elija tendrá un efecto sobre cuánto se le cobre. Las características de la base de datos varían según el motor, el tamaño y la clase de memoria de la base de datos.
- Tipo de compra de base de datos. Cuando utiliza instancias de base de datos bajo demanda, paga la capacidad de cómputo por cada hora de ejecución de su instancia de base de datos, sin necesidad de compromisos mínimos. Con las instancias de base de datos reservadas, puede realizar un pequeño pago inicial único por cada instancia de base de datos que desee reservar por un plazo de 1 a 3 años.
- Número de instancias de base de datos. Con Amazon RDS, puede aprovisionar varias instancias de bases de datos para gestionar cargas máximas.
- Almacenamiento aprovisionado. No se aplican cargos adicionales por el almacenamiento de copias de seguridad de hasta el 100% del almacenamiento de la base de datos aprovisionado para una instancia de base de datos activa. Una vez que se termina la instancia de base de datos, el almacenamiento de copia de seguridad se factura por gigabytes al mes.
- Almacenamiento adicional. La capacidad de almacenamiento de copia de seguridad que se suma a la cantidad de almacenamiento aprovisionado se factura por gigabyte al mes.
- Solicitudes. La cantidad de solicitudes entrantes y salientes que se realizaron a la base de datos.
- Tipo de implementación. Puede implementar su instancia de base de datos en una zona de disponibilidad única (lo que equivale a un centro de datos independiente) o en varias zonas de disponibilidad (lo que equivale a un centro de datos secundario, para disponer de una mayor disponibilidad y durabilidad). Los cargos por almacenamiento y entrada y salida varían según la cantidad de zonas de disponibilidad en las que realiza la implementación.
- Transferencia de datos. La transferencia entrante de datos es gratuita, y los costos por la transferencia saliente se aplican por niveles.

![](../aws-images/aws-modulo-06/m6-sprincipales-aws-020.png)

Según las necesidades de la aplicación, es posible optimizar los costos de las instancias de base de datos de Amazon RDS si adquiere este tipo de instancias reservadas. Para comprar instancias reservadas, hace un pago único de bajo monto por cada instancia que quiera reservar y, a cambio, recibe un descuento importante en el cargo por hora de uso de la instancia.

![](../aws-images/aws-modulo-06/m6-sprincipales-aws-021.png)

El último producto que descubriremos es Amazon CloudFront.
Amazon CloudFront es un servicio web diseñado para la entrega de contenido. Brinda integración a otros servicios de Amazon Web Services para ofrecerle una forma sencilla de distribuir contenido a los usuarios finales con baja latencia, altas velocidades de transferencia de datos y sin compromisos mínimos.

![](../aws-images/aws-modulo-06/m6-sprincipales-aws-022.png)

Para comenzar a estimar los costos de Amazon CloudFront debe tener en cuenta lo siguiente:  

- Distribución del tráfico. La transferencia de datos y los precios de solicitud varían según las regiones geográficas, y los precios se basan en la ubicación de borde mediante la cual se entrega su contenido.
- Solicitudes. El número y el tipo de solicitudes efectuadas y la región geográfica en la que se efectúan.
- Transferencia saliente de datos. La cantidad de datos transferidos desde las ubicaciones de borde de Amazon CloudFront. 

![](../aws-images/aws-modulo-06/m6-sprincipales-aws-023.png)

La mejor forma de calcular el costo es analizar las características fundamentales de cada servicio de AWS, calcular el uso de ellas y, luego, comparar ese uso con los precios publicados en el sitio web.

![](../aws-images/aws-modulo-06/m6-sprincipales-aws-024.png)