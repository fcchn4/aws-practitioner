# Módulo 2 - Elastic Block Store (Amazon EBS)

![](../aws-images/aws-modulo-02/m2-sprincipales-aws-007.png)

Los volúmenes de **EBS** se pueden utilizar como unidad de almacenamiento para para las instancias de **Amazon EC2**, por lo que siempre que piense que necesita espacio en disco para las instancias que se ejecutan en **AWS**, puede recurrir a ellos. Estos volúmenes pueden ser discos duros, o dispositivos SSD, y usted paga según el uso, por lo que cuando ya no necesite un volumen, solo tiene que eliminarlo y dejar de pagar por él. Los volúmenes de **EBS** están diseñados para ofrecer **durabilidad** y **disponibilidad**. Esto significa que los datos de un volumen se replican automáticamente en varios servidores que se ejecutan en la zona de disponibilidad.

![](../aws-images/aws-modulo-02/m2-sprincipales-aws-008.png)

He realizado la comparación con los volúmenes **EBS** y los dispositivos de medios físicos como discos duros o SSD, pero en realidad es mucho mas duradero que eso debido a la **explicación** a nivel de bloque. Al crear un volumen de **EBS** puede seleccionar el tipo de almacenamiento que mejor se adapte a sus necesidades. Puede elegir entre magnético o SSD, en función de sus requisitos de rendimiento y precio. Se trata de elegir la herramienta adecuada para el trabajo correcto, por lo que, por ejemplo, si ejecuta una instancia de base de datos, puede configurar la base de datos para que utilice un volumen secundario para los datos, que puede tener un rendimiento mas rápido que el volumen asignado al sistema operativo. También puede asignar un volumen magnético para los registros, ya que el magnético es mas económico. Para proporcionar un nivel aun mayor de durabilidad de los datos, **Amazon EBS** le ofrece la posibilidad de crear instancias de un momento especifico de sus volúmenes y **AWS** le permite volver a crear un volumen nuevo a partir de una instancia en cualquier momento. Comparta instancias o incluso cópielas en diferentes regiones de **AWS** para obtener una protección de **recuperación de desastres (DR)** aun mayor. Por ejemplo puede cifrar y compartir instantáneas de Virginia a Tokio. También podrá cifrar los volúmenes de **Amazon EBS**, sin costo adicional. El cifrado se produce del lado de **Amazon EC2**, por lo que los datos que se transfieren entre la instancia **EC2**, y el volumen de **Amazon EBS** dentro de los centros de datos de **AWS** se cifrara en transito.

A medida que su empresa crece, es probable que la cantidad de datos almacenados en los volúmenes de **Amazon EBS** también aumente. Los volúmenes de **Amazon EBS** tienen el potencial de aumentar la capacidad y cambiar a diferentes tipos, lo que significa que puede cambiar de disco duro a SSD o aumentar de un volumen de 50 GB a uno de 16TB. Por ejemplo, puede realizar esta operación de cambio de tamaño sobre la marcha sin necesidad de detener las instancias. Dentro de la consola de administración de **AWS**, las instancias **EC2** y los volúmenes de **EBS** pueden estar aquí, en la consola de **EC2**, que puede encontrar haciendo clic en **EC2**, en la pestaña Compute (Computo).

**Diseñados para:**

- Disponibilidad
- Durabilidad

**Ofrece:**

- Snapshots
- Cifrado
- Elasticidad