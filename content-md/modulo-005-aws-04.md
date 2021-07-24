# Módulo 5 - Amazon Inspector

![](../aws-images/aws-modulo-05/m5-sprincipales-aws-020.png)

Este módulo abarca **Amazon Inspector**, una herramienta que lo ayuda a mejorar la seguridad y la conformidad de las aplicaciones implementadas en AWS.

En la actualidad, para cualquier negocio, la seguridad es una prioridad principal. La evaluación de amenazas es una parte fundamental de cualquier plan de seguridad, pero las herramientas disponibles son costosas y se requiere mucho tiempo para crearlas, configurarlas y mantenerlas, lo que dificulta su incorporación en el ciclo de vida de desarrollo.

![](../aws-images/aws-modulo-05/m5-sprincipales-aws-021.png)

Sin una herramienta automatizada y eficaz para realizar evaluaciones de seguridad, las empresas dedican demasiado tiempo a las evaluaciones manuales y corren el riesgo de omitir vulnerabilidades de seguridad.

**Amazon Inspector** puede ayudarlo a solucionar estos problemas.

![](../aws-images/aws-modulo-05/m5-sprincipales-aws-022.png)

**Amazon Inspector** es un servicio automatizado de seguridad que ayuda a mejorar la seguridad y la conformidad de las aplicaciones implementadas en AWS.

El servicio evalúa automáticamente las aplicaciones en busca de vulnerabilidades o desviaciones respecto a las prácticas de AWS recomendadas.

Tras realizar una evaluación, Amazon Inspector genera un informe detallado con los pasos principales para solucionar el problema.

Es importante tener en cuenta que AWS no garantiza que seguir las recomendaciones resuelva todos los potenciales problemas de seguridad.  Los hallazgos que genere Amazon inspector dependerán de los paquetes de reglas que usted haya elegido e incluido en cada plantilla de evaluación, así como de la presencia en el sistema de componentes que no sean de AWS y de otros factores. 

![](../aws-images/aws-modulo-05/m5-sprincipales-aws-023.png)

Usted es responsable de la seguridad de las aplicaciones, los procesos y las herramientas que se ejecutan en el servidor de AWS. Para obtener más información, consulte el Modelo de responsabilidad compartida de AWS en: https://aws.amazon.com/es/compliance/shared-responsibility-model/

![](../aws-images/aws-modulo-05/m5-sprincipales-aws-024.png)

Conozcamos otras acciones que Amazon Inspector puede realizar por su organización.

- Amazon Inspector lo ayudará a identificar vulnerabilidades de seguridad y desviaciones respecto a las prácticas recomendadas en las aplicaciones, tanto antes de su implementación como durante la ejecución en un entorno de producción. Esto lo ayuda a mejorar el plan general de seguridad de las aplicaciones implementadas en AWS.
-  Amazon Inspector se instala en el agente, funciona mediante una API y se entrega como servicio. De este modo, les resultará más sencillo integrarlo en su proceso de DevOps porque descentraliza y automatiza las evaluaciones de vulnerabilidad, y alienta a los equipos de desarrollo y operaciones a convertir  la evaluación de seguridad en parte fundamental del proceso de implementación.
- Este servicio lo ayuda a reducir el riesgo de introducir problemas de seguridad durante el desarrollo y la implementación mediante la automatización de la evaluación de seguridad de aplicaciones y la identificación proactiva de las vulnerabilidades. Esto permite desarrollar y probar nuevas aplicaciones rápidamente, así como valorar la conformidad con las prácticas recomendadas y las políticas.
- AWS evalúa continuamente el entorno de AWS y actualiza una base de conocimientos sobre prácticas recomendadas y reglas de seguridad. Amazon Inspector pone a su disposición estos conocimientos por medio de un servicio que simplifica el proceso de establecer y hacer que se cumplan las prácticas recomendadas en su entorno de AWS.
- Amazon Inspector permite a los equipos y auditores de seguridad comprobar las pruebas que se realizan durante el desarrollo de las aplicaciones. De este modo, se simplifica el proceso de validar y demostrar el seguimiento de los estándares y prácticas recomendadas de seguridad y conformidad.
- Amazon Inspector permite definir estándares y prácticas recomendadas para sus aplicaciones, y comprobar que se cumplen. Esto simplifica el proceso de hacer que se cumplan los estándares y las prácticas recomendadas de seguridad en su organización, y ayuda a administrar de forma proactiva los problemas de seguridad antes de que afecten a la aplicación de producción.

Puede obtener acceso a estas características de varias maneras diferentes.

- Inicie Sesión en la consola de administración de AWS y abra la consola de Amazon Inspector, una interfaz basada en navegador que le permite acceder al servicio.
- También puede utilizar la CLI de AWS, el SDK o la API para acceder al servicio. 
- El uso de las herramientas de línea de comandos de AWS para ejecutar tareas de Amazon Inspector puede resultar más rápido y práctico que utilizar la consola. Las herramientas de línea de comandos también son útiles si quiere crear scripts que realicen tareas de AWS.

![](../aws-images/aws-modulo-05/m5-sprincipales-aws-025.png)

Para ayudarlo a comenzar rápido, Amazon Inspector incluye una base de conocimientos con cientos de reglas asignadas a los estándares de seguridad y conformidad más habituales y a las definiciones de vulnerabilidad. Algunos ejemplos de estas reglas incorporadas son las comprobaciones de activación de inicio de sesión raíz remoto o instalación de versiones de software vulnerables. Los investigadores de seguridad de AWS actualizan regularmente las reglas. 

![](../aws-images/aws-modulo-05/m5-sprincipales-aws-026.png)

Cuando Amazon Inspector evalúa un objeto, proporciona hallazgos, es decir, descripciones detalladas de posibles problemas de seguridad. Los hallazgos también contienen recomendaciones sobre cómo resolver los problemas de seguridad.

Finalicemos con unas revisión de lo que Amazon Inspector puede hacer por su organización. Como vimos, Amazon Inspector le permite hacer lo siguiente:

-  Puede evaluar de forma rápida y sencilla la seguridad de sus recursos de AWS para fines forenses de solución de problemas o de auditoría activa a su propio ritmo.
- Puede centrarse en problemas de seguridad más complejos y delegar en este servicio automatizado las tareas generales para evaluar la seguridad de la infraestructura.
-  Si utiliza Amazon Inspector, obtendrá conocimientos más amplios de sus recursos de AWS, ya que los hallazgos de Amazon Inspector se generan a partir del análisis de la actividad real y de los datos de configuración de los recursos de AWS.

![](../aws-images/aws-modulo-05/m5-sprincipales-aws-027.png)

Para obtener más información visite: https://aws.amazon.com/es/inspector/