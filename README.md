# Coopetica-programacion
Modelado del dominio coopetica
UNIVERSIDAD LATINA DE COSTA RICA
Escuela de Ingeniería de Sistemas · Bachillerato en Ingeniería de Sistemas
BIS04 Programación II
TAREA 1 — TRABAJO EXTRACLASE
Modelado del dominio CoopeTica sobre un repositorio colaborativo · 5 %

Elemento	Detalle
Valor	5 % de la nota del curso
Modalidad	En parejas (máximo dos estudiantes)
Asignación	Semana 3
Entrega	Semana 5, al inicio de la sesión
Formato de entrega	Enlace al repositorio de GitHub, publicado en el Aula Virtual por ambos integrantes
Unidad	Unidad 1. Diseño de Clases

Qué se evalúa realmente en esta tarea. No es una tarea de programación: en esta entrega no se escribe código funcional. Se evalúan dos cosas que sostienen todo el resto del curso: que usted sepa abstraer un dominio real en un modelo de clases, y que la pareja sepa trabajar sobre un mismo repositorio sin destruirse. El repositorio que creen aquí es el mismo que van a usar para el Proyecto Programado, así que lo que construyan esta semana los acompaña hasta la defensa.
1. Nombres de los integrantes
Integrante 1:Andrés Bonilla  Usuario de GitHub: andresbj05

Integrante 2: Sebastian mata  Usuario de GitHub:sebasmata1215

Enlace del repositorio: https://github.com/andresbj05/Coopetica-programacion
Debe colocarlo también en el espacio de la plataforma.


2. El caso: CoopeTica R.L.
Lea el enunciado completo antes de empezar a modelar. Todo lo que necesita está aquí, y lo que no aparece no forma parte del alcance.

CoopeTica R.L. es una cooperativa de ahorro y crédito costarricense de tamaño mediano que actualmente administra su operación en hojas de cálculo dispersas. Requiere un sistema que le permita ordenar la información de sus asociados, sus cuentas y sus movimientos.

De las entrevistas con el personal de la cooperativa se obtuvo la siguiente descripción:

Cada asociado de la cooperativa se identifica por su número de cédula, y de él se registra el nombre completo, el número de teléfono, el correo electrónico y la fecha en que ingresó a la cooperativa. Un asociado puede estar activo o inactivo, y la cooperativa necesita poder desactivarlo sin borrar su información histórica.

Un asociado puede abrir varias cuentas. Toda cuenta tiene un número único, un saldo y una fecha de apertura, y puede encontrarse abierta o cerrada. La cooperativa maneja tres productos: cuenta de ahorro, cuenta corriente y certificado a plazo. Los tres permiten consultar el saldo y recibir depósitos, pero cada uno calcula sus intereses con una tasa distinta y cobra comisiones diferentes. El certificado a plazo, además, tiene un plazo en meses y una fecha de vencimiento, y no permite retiros antes de esa fecha.

Cada movimiento que se realiza sobre una cuenta queda registrado con su fecha y hora, el tipo de movimiento, el monto y el saldo que quedó después de aplicarlo. Los tipos de movimiento que maneja la cooperativa son depósito, retiro, aplicación de intereses y cobro de comisión.

La cooperativa necesita poder consultar el detalle de cualquier asociado, ver el estado de sus cuentas, registrar depósitos y retiros validando que haya saldo suficiente, calcular los intereses de un periodo y generar un reporte de movimientos por cuenta entre dos fechas.


3. Entregables
El repositorio debe contener los cuatro elementos siguientes al momento de la entrega.
3.1 Diagrama de clases del dominio
Un diagrama de clase UML con las clases que identificaron a partir del enunciado. Debe incluir, para cada clase, sus atributos con tipo y visibilidad, y sus métodos con parámetros y tipo de retorno.
•No incluya todavía las relaciones entre clases: ese contenido se estudia en la Semana 4 y no se evalúa aquí.
•Puede elaborarlo con la herramienta que prefiera. Exporte el resultado como imagen PNG o como PDF y agréguelo al repositorio en una carpeta llamada diagramas.
•Los atributos van en visibilidad privada y los métodos en pública, salvo que justifiquen lo contrario en el README.
3.2 Archivo README.md
Es el documento que se ve al abrir el repositorio y debe permitir que alguien externo entienda el trabajo sin preguntarles nada. Debe contener:
1.Título del proyecto y nombres de ambos integrantes con su usuario de GitHub.
2.Una descripción breve del dominio modelado, en sus propias palabras.
3.El diagrama incrustado como imagen.
4.La justificación del modelo: por qué escogieron esas clases y no otras, qué elementos del enunciado descartaron deliberadamente y por qué.
5.La bitácora de uso de inteligencia artificial, conforme a la política del curso.
3.3 Evidencia de trabajo colaborativo
Esta parte es la que distingue la tarea de un trabajo individual entregado por dos personas. El repositorio debe mostrar:
•Commits propios de ambos integrantes, con mensajes descriptivos. No se acepta que una sola persona publique todo el trabajo.
•Al menos una rama por integrante, además de la principal.
•Al menos dos solicitudes de incorporación cerradas, una por cada integrante.
•Al menos un conflicto de fusión resuelto, documentado en el archivo CONFLICTO.md según se indica abajo.
3.4 Archivo CONFLICTO.md
Un documento breve, de media página, que explique el conflicto que resolvieron. Debe responder cuatro preguntas:
1.¿Qué archivo entró en conflicto y por qué?
2.¿Qué mostraba Git exactamente? Incluya el fragmento con los marcadores de conflicto.
3.¿Cómo decidieron cuál versión conservar, o cómo combinaron ambas?
4.¿Qué harían distinto para evitar ese conflicto la próxima vez?

El conflicto se provoca a propósito. No esperen a que ocurra por accidente. La forma más simple es que ambos editen la misma línea del README desde sus respectivas ramas y luego intenten integrarlas. Un conflicto no es un error ni una falla del equipo: es una situación normal del trabajo colaborativo, y lo que se evalúa es que sepan resolverlo. Quien nunca resolvió uno con el profesor al lado, lo va a enfrentar solo durante el proyecto.


4. Bitácora de uso de inteligencia artificial
Conforme a la política del curso, la inteligencia artificial está permitida para aclarar conceptos, explicar errores o discutir alternativas de diseño, y no está permitida para generar el modelo ni el contenido de los entregables.
Incluya en el README una sección con la bitácora. Cada entrada debe indicar qué preguntó, a qué herramienta y qué hizo con la respuesta. Si no utilizaron ninguna herramienta, escríbanlo explícitamente.

Ejemplo de entrada válida:

## Bitacora de uso de IA
 
- Consulte a [herramienta] la diferencia entre un atributo y una
  clase cuando un sustantivo del enunciado puede ser cualquiera de
  los dos. La respuesta explico el criterio de si tiene
  comportamiento propio. Aplicamos ese criterio para decidir que
  TipoMovimiento no seria una clase separada.
 
- No utilizamos IA para construir el diagrama ni para redactar la
  justificacion del modelo.

Por qué se pide esto. La bitácora no es un control policial: es parte de la formación profesional. Saber qué le delegó a una herramienta y qué resolvió usted es una competencia en sí misma, y en la defensa oral del proyecto va a tener que sustentar sus decisiones de diseño sin ayuda. Una bitácora honesta que reconozca un uso intensivo vale más que una vacía que no corresponde al trabajo entregado.


5. Rúbrica de evaluación
Se aplican los rubros oficiales de Trabajo Extraclase del sílabo académico, instanciados en el repositorio.

N°	Rubro	Valor	Qué se verifica en el repositorio
1	Presentación del documento y cumplimiento de la fecha establecida	1 %	Último commit dentro del plazo. README completo y legible. Archivo .gitignore presente y sin carpetas de compilación publicadas.
2	El procedimiento está claramente establecido y ordenado para la solución del problema	1 %	Historial de commits legible con mensajes descriptivos. Ramas con nombre coherente. Estructura de carpetas ordenada.
3	Realiza un análisis de la solución del problema para dar respuesta al mismo	1 %	El diagrama refleja el dominio del enunciado. La justificación del README explica las clases escogidas y las descartadas.
4	Utiliza variedad de elementos técnicos que justifican la información recabada	1 %	Uso efectivo de rama y solicitud de incorporación. Conflicto resuelto y documentado en CONFLICTO.md con las cuatro preguntas respondidas.
5	Trabajo original, con nuevos conocimientos	1 %	Ambos integrantes con commits propios. Bitácora de uso de IA presente y coherente con el trabajo entregado.
	TOTAL	5 %	
5.1 Descriptores de desempeño
Nivel	Descripción
Excelente (95-100)	El modelo identifica correctamente las clases del dominio, con atributos tipados y visibilidad adecuada. La justificación explica con criterio técnico qué se incluyó y qué se descartó. El historial muestra contribución equilibrada de ambos integrantes con mensajes descriptivos. El conflicto está documentado con precisión y la reflexión final es pertinente.
Notable (94-80)	El modelo es correcto en lo esencial, con omisiones menores de atributos o métodos. La justificación existe pero es superficial en algún punto. El historial muestra participación de ambos, aunque desbalanceada. El conflicto está documentado, con alguna de las cuatro preguntas respondida de forma incompleta.
Bueno (79-70)	El modelo presenta confusiones entre clase y atributo, o incluye elementos que no corresponden al dominio. La justificación es mínima. La participación de uno de los integrantes es marginal. El conflicto se documentó de forma incompleta o sin el fragmento de los marcadores.
Desempeño insuficiente (menor a 70)	El modelo no corresponde al enunciado o está incompleto. No hay justificación. Todos los commits pertenecen a una sola persona. No hay evidencia de ramas, de solicitudes de incorporación ni de resolución de conflicto. Falta la bitácora de IA.


6. Ruta sugerida de trabajo
No es obligatoria, pero es el orden que evita la mayoría de los tropiezos.
1.Uno de los dos crea el repositorio en GitHub y agrega al compañero como colaborador. Solo uno lo crea: si ambos crean uno, terminan con dos repositorios distintos.
2.Ambos lo clonan en su equipo.
3.Agreguen primero el .gitignore y el README inicial, desde la rama principal. Es el único momento del trabajo en que van a escribir directamente en main.
4.Lean el enunciado juntos y subrayen sustantivos y verbos. Esta parte se hace en conjunto: es la decisión de diseño y no conviene repartirla.
5.Repartan el trabajo por clase, no por archivo. Por ejemplo, uno modela Asociado y Cuenta, el otro Movimiento y los productos.
6.Cada quien crea su rama y trabaja ahí. Nombres sugeridos: modelo-asociado y modelo-movimiento.
7.Cada quien abre su solicitud de incorporación y el otro la revisa antes de integrarla.
8.Provoquen el conflicto de forma deliberada, resuélvanlo y documéntenlo.
9.Redacten juntos la justificación del modelo y la bitácora de IA.
10.Verifiquen la lista de cotejo antes de entregar.
7. Lista de cotejo previa a la entrega
N°	Criterio	Listo
1	El repositorio es accesible y ambos integrantes aparecen como colaboradores.	
2	El README identifica el proyecto, a ambos integrantes y su usuario de GitHub.	
3	El diagrama está en la carpeta diagramas e incrustado en el README.	
4	Cada clase del diagrama tiene atributos con tipo y visibilidad.	
5	Cada método del diagrama tiene sus parámetros y su tipo de retorno.	
6	El README justifica las clases escogidas y las descartadas.	
7	Ambos integrantes tienen commits propios con mensajes descriptivos.	
8	Existe al menos una rama por integrante, además de la principal.	
9	Hay al menos dos solicitudes de incorporación cerradas.	
10	CONFLICTO.md responde las cuatro preguntas e incluye el fragmento con los marcadores.	
11	La bitácora de uso de IA está en el README.	
12	El .gitignore está presente y no se publicaron carpetas de compilación.	
13	Ambos integrantes publicaron el enlace en el Aula Virtual.	

Una recomendación que le va a servir en la Semana 15. Este repositorio se convierte en el repositorio oficial del Proyecto Programado en la Semana 7. Todo lo que construyan aquí —la estructura, los hábitos de commit, el reparto del trabajo— se arrastra hasta la defensa. Vale la pena hacerlo bien desde el inicio, porque en la defensa oral cada integrante responde por los commits que llevan su nombre.
8. Consultas
Ing. Bryan Alejandro Vega Rondón · bryan.vega4@ulatina.net · BIS04 Programación II · Escuela de Ingeniería de Sistemas.