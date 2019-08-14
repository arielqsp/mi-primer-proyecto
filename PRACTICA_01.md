<h1 align="center">PRÁCTICA N°1</H1>
<H2 align="center">Sistemas empresariales</h2>

|**Carrera:**|Ingeniería de Sistemas |
|:--------|:----------|
|**Materia:**|Tecnologías Emergentes II|
|**Apellidos y nombres:**|Quispe Paye Ariel|
|**C.I.:**|6869625LP|
|**Lugar y fecha:**|El Alto, 14 de Agosto de 2019|


### 1) Explique que son los sistemas empresariales
<p align="justify">Un Sistema de Información Empresarial es un sistema que tiene un impacto muy importante en el funcionamiento de la organización o negocio y cuya falla traería graves consecuencias. Normalmente que ofrece alta calidad de servicio, gestiona con grandes volúmenes de datos, disponible de forma continua y es capaz de soportar cualquier organización grande.</p>

### 2)Describa cuales son las caracteristicas màs importantes de una aplicaciòn empresarial.
- *Operaciones transaccionales*
- *Seguras*
- *Permiten la integración*
- *Acceso a bases de dato*
- *Arquitectura multicapa*
- *Escalables*
- *Disponibles*

### 3) Investigue y proponga cinco instituciones que requieran aplicaciones de misión crítica. Justifique su respuesta.
|INSTITUCIÓN|*RESPUESTA* |
|----------|-----------------------------|
|Universidades |*Tiene que adaptarse al constante incremento de registro de estudiantes*|
|Entidades Bancarias|*Los usuarios necesitan acceder a sus cuentas desde cualquier dispositivo móvil*|
|Centros de Salud|*Deben actualizar la información constantemente*|
|INE|*Manejan datos estadísticos según los datos recientes*|
|FACEBOOK|*Necesita contar con una seguridad avanzada  ante cualquier vulnerabilidad*|

###  4) Explique cuáles son las diferencias entre la escalabilidad horizontal y escalabilidad vertical.
**Escalabilidad vertical**. Se refiere a actualizaciones o modernización de componentes existentes.

**Escalabilidad horizontal**. Se refiere a aumentar el número de componentes.

### 5) Que es un servidor Web y que es un servidor de aplicaciones.
<p align="justify">Un <b>Servidor web</b> o servidor HTTP es un programa informático que procesa una aplicación del lado del servidor, realizando conexiones bidireccionales o unidireccionales y síncronas o asíncronas con el cliente y generando o cediendo una respuesta en cualquier lenguaje o Aplicación del lado del cliente.</p>
<p align="justify">Un  <b>Servidor de aplicaciones</b> es un dispositivo de de software que proporcionan servicios de aplicación a las computadoras cliente. Generalmente gestiona la mayor parte (o la totalidad) de las funciones de la lógica de negocio y acceso a los datos de la aplicación. Los beneficios de la aplicación de la tecnología de servidores de aplicación son la centralización y al disminución de la complejidad en el desarrollo.</p>

### 6) Con un gráfico explique cómo funciona el protocolo HTTP
![protocolo HTTP](http://www.hermosaprogramacion.com/wp-content/uploads/2015/01/http-protocolo-peticion.png)

### 7) Explique los elementos importantes de REQUEST en HTTP
1. Método HTTP (la acción a realizar)
2. La página para acceder (una URL).
3. Parámetros de forma (como argumentos de un método)

### 8) Explique los elementos importantes de RESPONSE en HTTP
1.	 Un código de estado (para saber si la solicitud fue exitosa)
2.	 Tipo de contenido (texto, imagen, HTML, etc.) 
3.	 El contenido (el HTML real, la imagen, etc.)

### 9)Describa con un grafico la arquitectura Java EE
![Arquitectura de JAVA EE](http://2.bp.blogspot.com/-VDPKj1Exx5A/U9-yuzabmbI/AAAAAAAAAO0/AJMNzN8D3P0/s1600/Captura.PNG)

### 10) Explique cuales son los contenedores, componentes y servicios de Java EE
- <p align="justify">Un <b>contenedor</b> es un entorno de ejecución que provee al componente una serie de servicios. Los <b>tipos de contenedores</b> son: Contenedor Web, contenedor de negocio (o de EJBS).</p>
- <p align="justify">Un <b>componente</b> es una unidad de software que forma parte de una aplicación. Los <b> tipos de componentes </b>son los siguientes: Componente cliente ( <i>Cliente AWT, wing,  pplet y navegador Web</i>),  componente web (<i> Servlet, JSP y JSF</i>), componente de negocio (<i> EJB</i>)
- <p align="justify">Los <b>Servicios Java EE</b>, son los servicios que deben ofrecer los contenedores Java EE definiéndose así los siguientes servicios:<b>de directorio</b>( <i>para la indexación y búsqueda de componentes y recursos</i>),<b>de despliegue</b>(<i> para poder personalizar los componentes y recursos</i>), <b>de transaccionalidad</b>(<i>para poder ejecutar distintas acciones en una misma unidad transaccional</i>), <b>de seguridad</b>(<i> para poder autenticar y autorizar a los usuarios de la aplicación</i>), <b>de acceso a datos</b>(<i>para facilitar el acceso a Bases de Datos</i>), <b>de conectividad</b>( <i>para poder acceder fácilmente a distintos EIS</i>) y <b>de mensajería</b>(<i>para poder comunicarse con otros componentes, aplicaciones o EIS</i>)</p>
<p align="justify">Para que un entorno de ejecución pueda decir que es Java EE debe implementar y soportar todos los tipos de componente, de contenedores y de servicios.</p>

<h3 align="justify">11) Investigue los metodos mas utilizados de las clases HttpServlet, HttpServletRequest y HttpServletResponce y para cada uno muestre un ejemplo. </h3>

#### Clase Httpservlet

- <p align="justify"><b>doGet(HttpServletRequest req, HttpServletResponse resp):</b> Es el método llamado para procesar información que haya sido enviado con el método GET. Este método es llamado concurrentemente para cada cliente por lo que hay que estar atento por posibles variables compartidas que causen problemas.</p>
- <p align="justify"><b>doPost(HttpServletRequest req, HttpServletResponse resp):</b> Ídem al anterior pero para el método POST, en general se implementa sólo un método y el otro lo referencia.</p>

####  Clase HttpServletRequest

- <p align="justify"><b>getHeader(String name):</b> Permite obtener el valor de los Headers de HTTP con que fue llamado el servlet.</p>
- <p align="justify"><b>getCookies():</b> Retorna un arreglo que contiene todas las cookies que el cliente envía al servlet.</p>
- <p align="justify"><b>getSession():</b> Retorna la sesión en la cual se encuentra el cliente.</p>

#### Clase HttpServletResponse

- <p align="justify"><b>addCookie(Cookie cookie): </b>Para definir nuevas cookies en el cliente.</p>
- <p align="justify"><b>setHeader(String name, String value):<b> Para definir un header HTTP a enviar al cliente.</p>
- <p align="justify"><b>sendRedirect(String location): </b>Envía un mensaje al cliente para redireccionar la respuesta a la dirección señalada.</p>











