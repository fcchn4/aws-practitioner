# Módulo 3 - Amazon CloudWatch

![](../aws-images/aws-modulo-03/m3-sprincipales-aws-045.png)

**¿Qué es Amazon CloudWatch?**  Básicamente es un servicio de monitoreo de los recursos y las aplicaciones de **AWS** que ejecuta en ellos en tiempo real. Algunas características de **Amazon CloudWatch** incluyen la recopilación y el seguimiento de métricas, como el uso de la CPU, la transferencia de datos, así como la E/S y el uso de disco. También podemos monitorear servicios de aplicaciones y recursos en la nube. Además tiene la posibilidad de establecer alarmas en cualquiera de las métricas para enviar notificaciones o realizar otras acciones automatizadas. 

![](../aws-images/aws-modulo-03/m3-sprincipales-aws-046.png)

Está es en realidad una de las características principales de **CloudWatch** que la convierte en una herramienta extraordinariamente potente: la capacidad de reaccionar de manera automática a los cambios. Podría enviar una aplicación del sistema existente y archivos de registro personalizados a registros de **Cloudwatch** que podrían analizarse casi en tiempo real. En general, esto le permite obtener una visibilidad de todo el sistema sobre la utilización de los recursos, el rendimiento de las aplicaciones y el estado operativo.

![](../aws-images/aws-modulo-03/m3-sprincipales-aws-047.png)

La arquitectura de **Amazon CloudWatch** incluye recursos compatibles con **CloudWatch**, como métricas de **CloudWatch**. Las métricas básicas incluyen aquellas como el uso de la CPU y las comprobaciones de estado. Las métricas personalizadas específicas de la aplicación también pueden incluirse o registrarse a partir de las estadísticas disponibles dentro de su aplicación. Todas estas cosas que se notificaron a la consola de administración de **AWS** también se puede registrar y enviar para activar una alarma de **Amazon CloudWatch**. Las alarmas de **CloudWatch** pueden enviar una notificación por correo electrónico o SMS. Además, tiene la posibilidad de activar un evento de **Auto Scaling**, que, como verá  más adelante, es un servicio muy potente. 

![](../aws-images/aws-modulo-03/m3-sprincipales-aws-048.png)

Algunos casos de uso comunes de **CloudWatch**, por supuesto, son responder a los cambios de estado de los recursos de **AWS** o invocar de manera automática una función de **Lambda** para realizar una actualización.  Por ejemplo, se pueden actualizar las entradas de DNS cuando un evento notifica que una instancia **EC2** entra en un estado de ejecución. También podría dirigir registros de API específicos de **CloudTrail** a un flujo de **Kinesis** para realizar un análisis detallado de los posibles riesgos de seguridad o disponibilidad. Asimismo, tiene la posibilidad de tomar una instancia de un volumen de **EBS** de forma programada o de registrar operaciones de nivel de objeto de **S3** mediante eventos de **CloudWatch**. 

![](../aws-images/aws-modulo-03/m3-sprincipales-aws-049.png)

Algunos de los componentes de **Amazon CloudWatch** incluyen las:

- Métricas
- Alarmas
- Eventos
- Registros 
- Paneles de Control

![](../aws-images/aws-modulo-03/m3-sprincipales-aws-050.png)

Hablaremos de cada uno de estos componentes de modo individual.

**Métricas de CloudWatch**, aquí es de dónde provienen los datos sobre el rendimiento de su sistema. En realidad, una métrica representa un conjunto de puntos de datos ordenados en el tiempo que se publicarán en **CloudWatch**. De forma predeterminada, varios servicios proporcionan métricas gratuitas desde cursos, como instancias **EC2**, volúmenes de **EBC** e instancias de bases de datos de **RDS**. Sin embargo, también puede publicar sus propias métricas de aplicación por una tarifa adicional. Todas estas métricas se cargan en su cuenta para las búsquedas y los gráficos, y la activación de alarmas más adelante.

![](../aws-images/aws-modulo-03/m3-sprincipales-aws-051.png)

Las alarmas de **CloudWatch** controlan una única métrica. Podría realizar una o varias acciones según el valor de la métrica con respecto a un umbral dado durante varios periodos. Por lo tanto, esa acción podría ser una de **EC2**, como detener, iniciar, terminar, reiniciar. Podría ser una acción de **Auto Scaling**, cómo lanzar una configuración de **Auto Scaling** y agregar más instancias al grupo de aplicaciones. O podría ser simplemente una notificación enviada a través de un tema de SMS. Se invocan acciones únicamente para los cambios de estado prolongados. 

![](../aws-images/aws-modulo-03/m3-sprincipales-aws-052.png)

Como ejemplo de una alarma de CloudWatch. Supongamos que quieres realizar el seguimiento del uso de la CPU en su instancia **EC2**. En este caso la CPU supera el porcentaje de seguridad durante 5 minutos, ese es el umbral que hemos establecido. Puede activar cosas como “Si la cantidad de conexiones simultáneas en una instancia de **RDS** es menor o mayor que 10 durante 1 minuto”. O bien, si tenemos uno, podríamos monitorear un Balanceador de carga elástico y establecer lo siguiente: “Si la cantidad  de hosts en buen estado es inferior a 5 durante 10 minutos, active una alarma o desencadene alguna acción”.

![](../aws-images/aws-modulo-03/m3-sprincipales-aws-053.png)

Por lo tanto, las alarmas de **CloudWatch** pueden medir una única métrica y realizar una o varias acciones. Podrían detener, terminar o reiniciar una instancia de recuperación. Podrían realizar un escalado o una reducción horizontal de un grupo de **Auto Scaling**. Recuerde que siempre realizamos un escalado horizontal para satisfacer la demanda de rendimiento y, una reducción horizontal, para ahorrar dinero. Queremos pensarlo en términos de un movimiento en ambas direcciones, o simplemente, podría enviar un mensaje de **SNS** por correo electrónico, HTTP o SMS para informarle de algo, por ejemplo, que se ha producido un evento. 

![](../aws-images/aws-modulo-03/m3-sprincipales-aws-054.png)

Los eventos de **CloudWatch** ofrecen una transmisión de eventos del sistema casi en tiempo real que describe los cambios hechos en los recursos de **AWS**. Se utilizan reglas sencillas que coinciden con eventos y luego se los direcciona a uno o más flujos o funciones de destino. Se podría conocer los cambios operativos cuando se producen. También se podría responder a estos cambios operativos y adoptar medidas correctivas según sea necesario. También puede programar acciones automatizadas que se activarán de forma automática en determinados momentos a través de expresiones **rate** o de trabajo **cron**.

![](../aws-images/aws-modulo-03/m3-sprincipales-aws-055.png)

A continuación se muestra, un ejemplo de los eventos de **CloudWatch**. En este caso, ¿cómo detecta y revoca de forma automática el acceso no intencionado de **IAM** con eventos de **CloudWatch**? Tengo una acción de la API que realiza una llamada a la API para un determinado evento. Los eventos de **CloudWatch** registrarán eso. Pueden ofrecer una regla que coincida con una función de **Lambda**. En este caso, si se produce ese evento concreto de un usuario autorizado, podemos revocar el acceso de ese usuario autorizado en particular mediante la función **Lambda**.

![](../aws-images/aws-modulo-03/m3-sprincipales-aws-056.png)

Registros de **CloudWatch**.

Básicamente, puede utilizar los registros de **CloudWatch** para monitorear los sistemas y aplicaciones, y solucionar los problemas de ellos con archivos de registro existentes.  Podríamos monitorear sus archivos de registro para detectar frases, valores o patrones específicos y recuperar los datos del registro asociados de los registros de **CloudWatch**. Todo se ejecuta en función de los agentes instalados en el sistema operativo. Por supuesto, tenemos agentes compatibles con todos los sistemas operativos que se admiten en **AWS**.

![](../aws-images/aws-modulo-03/m3-sprincipales-aws-057.png)

Las características del registro de **Amazon CloudWatch** incluyen la capacidad de monitorear registros de instancias **EC2** en tiempo real. Además, pueden monitorear los eventos de **AWS CloudTrail**. Recuerde: los eventos de **CloudTrail** son todas las acciones de la API que se queden en su cuenta. Y como todo lo que ocurre básicamente en **AWS** ya sea en la consola, la CLI o acceso directo a la API, depende de la API. Esto le ofrece un registro completo de quién hizo que, cuando estaba en su entorno. Resulta muy útil para la seguridad y la conformidad. Y, por supuesto también, puede archivar datos de registro para análisis futuros.

![](../aws-images/aws-modulo-03/m3-sprincipales-aws-058.png)

Además, puede almacenar y monitorear los archivos de registro de la aplicación, recopilar esas métricas y almacenarlas de forma duradera durante un periodo de tiempo prolongado. Los administradores pueden visualizarlos en la consola. Pueden almacenarse en **S3** para el acceso de otro servicio o los puede incorporar a otro servicio, usuario o herramienta. Y podemos realizar el procesamiento de datos en esa solución concreta, analizarlos a través de una transmisión de **Kinesis** o **AWS Lambda** y tomar medidas adicionales sobre esa métrica concreta. 

![](../aws-images/aws-modulo-03/m3-sprincipales-aws-059.png)

El panel de control de **CloudWatch** es en realidad una página de inicio personalizable dentro de la consola de **CloudWatch** para monitorear sus recursos por medio de un único panel, si lo desea. Incluso los recursos que se reparten entre diferentes regiones podrían agregarse en un solo lugar, lo que facilita en gran medida su visualización. Puede crear vistas personalizadas de las métricas y alarmas para sus recursos de **AWS**. Cada panel puede mostrar varias métricas, y se le puede agregar texto e imágenes según su preferencia.  Puede  crear paneles mediante la consola, la interfaz de línea de comandos, o la API de PutDashboard. 

![](../aws-images/aws-modulo-03/m3-sprincipales-aws-060.png)