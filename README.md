# SDR
## TEMA 0
### ACTIVIDADES DE INTRODUCCION

## Tema 1. Servidores Web
### Activity#1 - Instalación de Apache

#### 1. La arquitectura Web es un modelo compuesto de tres capas, ¿cuáles son y cuál es  la función de cada una de ellas?

1. Capa de Presentación (Frontend o Interfaz de Usuario)


Función: Es la capa con la que interactúa directamente el usuario. Se encarga de mostrar la información y capturar las entradas del usuario.
Tecnologías comunes: HTML, CSS, JavaScript, frameworks como React, Angular o Vue.js.

Responsabilidades:

Mostrar datos de forma amigable.
Validar entradas del usuario (validación básica).
Enviar solicitudes al servidor (por ejemplo, mediante llamadas API).
Recibir y renderizar respuestas del servidor.

2. Capa de Lógica de Negocio (Backend o Aplicación)

Función: Procesa las solicitudes del usuario, aplica las reglas del negocio y coordina la comunicación entre la capa de presentación y la capa de datos.
Tecnologías comunes: Lenguajes como Java, Python, PHP, Node.js, C#, junto con frameworks como Django, Spring, Express, etc.

Responsabilidades:

Validar y procesar los datos recibidos del frontend.
Aplicar reglas de negocio (por ejemplo, cálculos, autorizaciones, flujos de trabajo).
Gestionar la autenticación y autorización.
Interactuar con la capa de datos para almacenar o recuperar información.

3. Capa de Datos (Base de Datos o Almacenamiento)

Función: Almacena y gestiona los datos de forma persistente y segura.
Tecnologías comunes: Sistemas de gestión de bases de datos como MySQL, PostgreSQL, MongoDB, Oracle, SQL Server, etc.

Responsabilidades:

Almacenar datos de manera estructurada o no estructurada.
Permitir operaciones de lectura, escritura, actualización y eliminación (CRUD).
Garantizar la integridad, seguridad y disponibilidad de los datos.

#### 2. Una plataforma web es el entorno de desarrollo de software empleado para  diseñar y ejecutar un sitio web; destacan dos plataformas web, LAMP y WISA. Explica en qué consiste cada una de ellas.

1. LAMP

LAMP es un acrónimo que representa una pila (stack) de software de código abierto muy popular para el desarrollo y despliegue de aplicaciones web. Está compuesta por:

L – Linux: Sistema operativo base. Proporciona un entorno estable, seguro y de alto rendimiento.
A – Apache: Servidor web. Se encarga de recibir las solicitudes HTTP de los clientes (navegadores) y servir las páginas web.
M – MySQL: Sistema de gestión de bases de datos relacional. Almacena y gestiona los datos de la aplicación (aunque a veces se sustituye por MariaDB u otras bases de datos).
P – PHP: Lenguaje de programación del lado del servidor. Se utiliza para generar contenido dinámico. También puede referirse a Perl o Python, aunque en la práctica casi siempre es PHP.

Características de LAMP:

Es de código abierto y gratuito.
Muy utilizada en servidores web (especialmente en entornos Linux).
Altamente personalizable y con una gran comunidad de soporte.
Ideal para aplicaciones web dinámicas como WordPress, Drupal, Joomla, etc.

2. WISA

WISA es una pila tecnológica basada en productos de Microsoft, diseñada principalmente para entornos empresariales que utilizan infraestructura Windows. El acrónimo significa:

W – Windows Server: Sistema operativo del servidor. Proporciona el entorno base para ejecutar los demás componentes.
I – IIS (Internet Information Services): Servidor web de Microsoft. Gestiona las solicitudes HTTP/HTTPS y sirve contenido web.
S – SQL Server: Sistema de gestión de bases de datos relacional desarrollado por Microsoft. Ofrece alta integración con otras herramientas de la empresa.
A – ASP.NET: Marco de desarrollo de aplicaciones web de Microsoft, que puede usar lenguajes como C# o VB.NET para crear aplicaciones dinámicas.

Características de WISA:

Es una solución comercial (aunque existen versiones gratuitas limitadas, como SQL Server Express).
Ofrece una alta integración entre sus componentes gracias al ecosistema Microsoft.
Muy utilizada en entornos corporativos que ya emplean tecnologías Microsoft (como Active Directory, Azure, etc.).
Requiere licencias para su uso en producción, lo que puede incrementar costos.

#### 3. Lee el siguiente artículo e instala Apache en Ubuntu:
INSTALACIÓN APACHE

Una vez con el ubuntu instalado primero pasaremos a instalar el apache

primero haremos un apt update

<img width="520" height="352" alt="image" src="https://github.com/user-attachments/assets/bcbfd58e-2647-4c7a-83b9-285dee36488f" />

y ahora el siguiente para instalar apache

<img width="587" height="173" alt="image" src="https://github.com/user-attachments/assets/0b0ac66b-82ff-4b0f-8a19-157297c79185" />

cuando nos pregunte le decimos que si

<img width="614" height="403" alt="image" src="https://github.com/user-attachments/assets/a654c54c-a4d9-4d56-b45b-59504b57874e" />

despdespués haremos el siguiente comando

<img width="594" height="121" alt="image" src="https://github.com/user-attachments/assets/5523f0e1-d235-40cd-85df-999e8bc34a85" />

vamos a elegir apache para permitir el tráfico solo en el puerto 80
<img width="599" height="77" alt="image" src="https://github.com/user-attachments/assets/5e845385-89ac-4a9f-b5be-85cda1991f91" />

para verificar el cambio hacemos el siguiente comando
primero lo activamos y después un status

<img width="594" height="208" alt="image" src="https://github.com/user-attachments/assets/60595b4f-e4f7-4624-88f2-bfe04568db79" />

y como podemos ver buscando la ip de nuestro servidor nos sale apache

<img width="603" height="380" alt="image" src="https://github.com/user-attachments/assets/1194a340-af56-45ca-9e8c-1abc110a604d" />

ahora el siguiente paso es instalar mysql

<img width="605" height="26" alt="image" src="https://github.com/user-attachments/assets/6a5ac6a3-8ea3-4b8e-adf1-5bcf5f045f7d" />

y le decimos que si

<img width="599" height="397" alt="image" src="https://github.com/user-attachments/assets/74a76f1d-d20b-4d0c-8a21-7d94a285c1f9" />

despeus hacemos este comando

<img width="595" height="30" alt="image" src="https://github.com/user-attachments/assets/0f4db5d3-cd89-4104-be6e-be6e52730344" />

le decimos que si

<img width="602" height="198" alt="image" src="https://github.com/user-attachments/assets/b4e0f10c-96af-425d-b2b0-50a1d8697673" />

y ahora elegimos 1

<img width="596" height="131" alt="image" src="https://github.com/user-attachments/assets/b733886d-4668-4cb6-9365-b0cf55f79b20" />

le decimos que si

<img width="599" height="144" alt="image" src="https://github.com/user-attachments/assets/b7a38044-0354-445d-93fc-2e964307d95b" />

le decimos que si

<img width="592" height="104" alt="image" src="https://github.com/user-attachments/assets/7bc65f85-dc56-436e-9898-97371f3ef668" />

como podemos ver ya lo tenemos

<img width="597" height="237" alt="image" src="https://github.com/user-attachments/assets/ed37d788-07e2-43bc-9d89-7c6121a84f55" />



siguiente paso es instalar php
ponemos el siguiente comando

<img width="600" height="232" alt="image" src="https://github.com/user-attachments/assets/6a02b122-64bd-46dc-b882-e15e358a628f" />

y le ponemos la contraseña

<img width="597" height="225" alt="image" src="https://github.com/user-attachments/assets/4ae14315-e3ec-4733-80b8-c8913146122d" />

ahora una vez acabe la instalación hacemos el siguiente paso para ver su versión

<img width="599" height="121" alt="image" src="https://github.com/user-attachments/assets/ddeeaa13-46a4-4f98-9310-202ee546d1b6" />

ahora creamos el host virtual

<img width="600" height="48" alt="image" src="https://github.com/user-attachments/assets/76a143fd-0671-4fda-9e44-bdb0e65fc84e" />

ahora asignamos al usuario actual el domino

<img width="605" height="57" alt="image" src="https://github.com/user-attachments/assets/75cf0576-2ba4-4725-a97a-d1e0afd1294c" />

creamos el siguiente archivo para después poner la configuración

<img width="604" height="35" alt="image" src="https://github.com/user-attachments/assets/d20af1c2-408b-4984-9e4e-05bc0b9739ad" />


ahora vamos a habilitar un host virtual

<img width="594" height="91" alt="image" src="https://github.com/user-attachments/assets/ead819c4-c1f0-4487-9732-5581bf60692d" />

después hacemos los siguientes pasos
deshabilitamos el sitio por defecto que viene instalado en apache

<img width="600" height="95" alt="image" src="https://github.com/user-attachments/assets/82bc0f0c-a374-4090-b762-ac4094585988" />

y ahora para asegurarnos de que no tenga errores hacemos el siguiente

<img width="600" height="118" alt="image" src="https://github.com/user-attachments/assets/32f59c16-bb55-43a2-a41a-2d3daf1b86e8" />

ahora volvemos a cargar apache para que los cambios tengan efecto

<img width="595" height="51" alt="image" src="https://github.com/user-attachments/assets/1045b2f5-71b0-48bf-af59-240aa1ea09cd" />

ahora vamos a crear el index

<img width="600" height="37" alt="image" src="https://github.com/user-attachments/assets/4b37f654-1983-486c-b048-47a0294a9f72" />

<img width="598" height="184" alt="image" src="https://github.com/user-attachments/assets/bcb05463-ee19-48dc-a674-28e1e318bedd" />


### Activity#2 - Configuración básica de Apache


#### 1. Apache utilizará el puerto 81 además del 80

para que apache utilize el 81 ademas del 80 tendremos que entrar en este archivo

<img width="871" height="318" alt="image" src="https://github.com/user-attachments/assets/471a9aaa-cbcb-4fb9-9c6a-cf8ec22f5865" />

y modificar lo siguiente añadiendo la linea de Listen 81 y ya estaria

<img width="834" height="535" alt="image" src="https://github.com/user-attachments/assets/31475976-18d5-4e06-9ae9-eb2818acf05b" />

#### 2. Añadir el dominio “marisma.intranet” en el fichero “hosts”

ahora tenemos que entrar en este archivo

<img width="983" height="280" alt="image" src="https://github.com/user-attachments/assets/61d0388a-8e12-4c04-91d5-c9ebb85ec7f9" />

y añadir lo siguiente

<img width="972" height="657" alt="image" src="https://github.com/user-attachments/assets/650839cf-a66f-44d8-8097-071c6c138a06" />

#### 3. Cambia la directiva “ServerTokens” para mostrar el nombre del producto.

primero entramos aqui

<img width="816" height="71" alt="image" src="https://github.com/user-attachments/assets/a38a48dc-b281-468d-bc24-58cc9d293d0a" />


y cambiamos esa linea

<img width="941" height="681" alt="image" src="https://github.com/user-attachments/assets/2224cd33-9fc4-4437-a551-9015cbe81123" />

#### 4. Comprueba si se visualiza el pie de página en las páginas generadas por Apache (por ejemplo, en las páginas de error). Cambia el valor de la directiva “ServerSignature” y comprueba que funciona correctamente. 

para configurar esto debemos de entrar en este archivo

<img width="875" height="307" alt="image" src="https://github.com/user-attachments/assets/8df349f4-8408-4add-9eac-236a15ace9d4" />

y tendremos que cambiar esta liena que viene en On y la ponemos en Off

<img width="950" height="599" alt="image" src="https://github.com/user-attachments/assets/ce1ee160-e88a-4db1-93eb-e444e7118300" />

#### 5. Crea un directorio “prueba” y otro directorio “prueba2”. Incluye un par de páginas en cada una de ellas.

<img width="913" height="521" alt="image" src="https://github.com/user-attachments/assets/acd4c468-07d3-4bef-845f-6f5e53ea76a5" />

### Activity#3 - Directorios

1. Crea un directorio llamado "dir1" y otro llamado "dir2" 

<img width="741" height="59" alt="image" src="https://github.com/user-attachments/assets/a6f3a127-92bf-4da8-8709-d97401510720" />

<img width="749" height="44" alt="image" src="https://github.com/user-attachments/assets/76f061b2-38ca-45b9-a224-4b67ad93e205" />

 

2. Explica qué diferencia existe entre ambos y muestra su equivalencia con la directiva Require: 

- El orden es Denegar, Permitir. Esto significa que primero se evalúan las reglas Deny y luego las Allow.

<Directory /var/www/example1> Order Deny,Allow 

Deny from All 

Allow from 192.168.1.100 

</Directory> 

- El orden es Permitir, Denegar. La última regla que coincide (o la regla final si no coincide ninguna) determina el resultado.

<Directory /var/www/example1> Order Allow,Deny 

Deny from All 

Allow from 192.168.1.100 

</Directory> 


Equivalencia con Require:

Ambos ejemplos (donde solo se permite el acceso a 192.168.1.100) son equivalentes a:

<Directory /var/www/example1>
    Require ip 192.168.1.100
</Directory>

 
3. Para dir1 
a Permite el acceso de las peticiones provenientes de 10.3.0.100 
b Permite el acceso desde "marisma.intranet" 
c Permite el acceso desde cualquier subdominio de "marisma.intranet" 
d Permite el acceso de las peticiones provenientes de "10.3.0.100" con máscara "255.255.0.0"

 <img width="912" height="28" alt="image" src="https://github.com/user-attachments/assets/ce5c45e0-3f04-497b-abd7-2537916086c8" />

<img width="1031" height="318" alt="image" src="https://github.com/user-attachments/assets/bec4a761-01e2-4a7c-bee8-df28c6977ea3" />

Modifica la configuración de forma que el acceso a dir1: 

Se permita a "marisma.intranet" y no se permita desde 10.3.0.101" 

<img width="717" height="225" alt="image" src="https://github.com/user-attachments/assets/1ebd7d62-ef2f-4d55-bae0-43c150f3c115" />

5. Modifica la configuración de forma que el acceso a dir2: 

Se permita a "10.3.0.100/8" y no a "marisma.intranet" 

<img width="558" height="221" alt="image" src="https://github.com/user-attachments/assets/ee23d852-df8a-47bc-b9b4-5e3e65dff1e8" />

Reiniciamos apache

<img width="668" height="69" alt="image" src="https://github.com/user-attachments/assets/a20a5aec-b016-442e-a516-6b0276611aec" />

### Activity#4 - Expresiones regulares

Aqui probamos com palabras

<img width="676" height="213" alt="image" src="https://github.com/user-attachments/assets/59244992-b07e-4408-9ead-ec3a477a1c54" />

Y aqui probamos con numeros telefonicos

<img width="687" height="227" alt="image" src="https://github.com/user-attachments/assets/67d72bea-cde1-437e-b201-a7e24083fabb" />

Ahora creamos un archivo

<img width="607" height="31" alt="image" src="https://github.com/user-attachments/assets/f851b974-3c07-4b85-b8cb-7b489de5dbfb" />

ahora escribimos expresiones dentro

<img width="686" height="368" alt="image" src="https://github.com/user-attachments/assets/9da2f054-7d34-4b20-bb3e-ffa998278cee" />

probamos el email con el archivo

<img width="685" height="183" alt="image" src="https://github.com/user-attachments/assets/95abed99-33cf-4697-933c-7521743b937b" />

probamos los numeros

<img width="683" height="111" alt="image" src="https://github.com/user-attachments/assets/2a27fa9f-1a93-46ed-af06-0abe1e0b899c" />

ahora entramos en este archivo para añadir lo que necesitamos para el redireccionamiento

<img width="696" height="49" alt="image" src="https://github.com/user-attachments/assets/0ebd85a4-9a0a-4657-8433-89be9a12452f" />

añadirmos esta linea

<img width="690" height="487" alt="image" src="https://github.com/user-attachments/assets/76078140-da77-4c76-9377-d40223303919" />

y probamos

<img width="860" height="406" alt="image" src="https://github.com/user-attachments/assets/9567f7d9-719d-4d43-951c-7f894061cd54" />

y ahora solo nos faltaria probar uno que funcione y otro que falle para verlo

<img width="995" height="96" alt="image" src="https://github.com/user-attachments/assets/55d9b0cd-1655-4694-ba17-0641768f874d" />


### Activity#5 - Reescritura

primero tenemos que instalar php para ello hacemos lo siguiente

<img width="662" height="67" alt="image" src="https://github.com/user-attachments/assets/337ae8d6-11d6-4a96-9a1b-6d35bc95fc38" />

y instalamos

<img width="869" height="38" alt="image" src="https://github.com/user-attachments/assets/33386ab1-0c87-4414-bb5a-19541330f33b" />

habilitamos el modo rewrite en apache

<img width="640" height="71" alt="image" src="https://github.com/user-attachments/assets/14e73a17-2208-45c2-8b29-c76e7c1888fb" />

y reiniamos apache para aplicar los cambios

<img width="758" height="56" alt="image" src="https://github.com/user-attachments/assets/6ded4433-c8eb-4f25-ba95-5dac217cea92" />

ahora creamos este fichero

<img width="765" height="37" alt="image" src="https://github.com/user-attachments/assets/d9029d5d-6b40-48e3-a77e-e1da3002edf5" />

y le ponemos esto

<img width="1074" height="680" alt="image" src="https://github.com/user-attachments/assets/8cd63aee-dc99-4352-afd2-4515075d353e" />

ahora abrimos el archivo de configuracion

<img width="900" height="36" alt="image" src="https://github.com/user-attachments/assets/abf36b9b-5f5e-4db5-b58c-6abb201e3b34" />

y le añadimos esto

<img width="1088" height="681" alt="image" src="https://github.com/user-attachments/assets/38ece3e5-4b0e-454a-8886-54970f118307" />

comprobamos si esta bien escrito

<img width="1035" height="114" alt="image" src="https://github.com/user-attachments/assets/23ee6b82-d42b-41ef-a02c-bbdb0928ac09" />

reiniciamos apache

<img width="685" height="58" alt="image" src="https://github.com/user-attachments/assets/c0fd8aa6-bcd4-4cf9-bafc-7aa46442c910" />

y comprobamos

<img width="1042" height="310" alt="image" src="https://github.com/user-attachments/assets/de844caa-5167-4f9c-b51a-83c0ad82ade4" />


### Activity#6 - Virtual Host

primero vamos a crear la estructura de directorios que necesitamos para esta practica

<img width="805" height="148" alt="image" src="https://github.com/user-attachments/assets/07292230-94dd-4cfd-a4aa-22367fd18ced" />

ahora creamos contenido de prueba

<img width="1029" height="205" alt="image" src="https://github.com/user-attachments/assets/59a59d77-eecc-4654-8c29-70f6ad1b064b" />

ahora creamos el primer archivo

<img width="876" height="49" alt="image" src="https://github.com/user-attachments/assets/ffd0d719-f04c-42b3-8342-00f609211ef7" />


y le ponemos el siguiente contenido

<img width="764" height="291" alt="image" src="https://github.com/user-attachments/assets/d23bf7ac-3492-48ad-baa0-e87dbf117390" />


hacemos lo mismo con el segundo

<img width="874" height="40" alt="image" src="https://github.com/user-attachments/assets/fa33c2bb-4264-4990-8127-cd04a06e61ec" />

y le pegamos el contenido

<img width="809" height="302" alt="image" src="https://github.com/user-attachments/assets/04f3c5ab-cb53-4672-a02c-b431793b39a0" />

habilitamos los nuevos sitios y reiniciamos apache para que se aplique la configuracion

<img width="687" height="218" alt="image" src="https://github.com/user-attachments/assets/88b2751b-a7ec-4206-8537-356983d7854e" />

ahora tenemos que editar este archivo

<img width="712" height="45" alt="image" src="https://github.com/user-attachments/assets/f36f5e2a-b013-49e7-8fee-3e602a094f7d" />

para añadir estas dos lineas

<img width="705" height="329" alt="image" src="https://github.com/user-attachments/assets/ffa3c09c-f9de-4577-a3c4-926123fdba88" />

ahora solo falta probarlos

el sitio1

<img width="884" height="306" alt="image" src="https://github.com/user-attachments/assets/46794de5-1803-4361-962e-2be242771615" />

el sitio2

<img width="889" height="312" alt="image" src="https://github.com/user-attachments/assets/f0839e96-0fa3-42a6-8e4f-2dfa93787b6e" />


### Activity#7 - Autentificacion

primero tenemos que instalar esto

<img width="697" height="25" alt="image" src="https://github.com/user-attachments/assets/c2709927-aee6-4e60-8739-b47ecb0c7807" />

ahora creamos los usuario

<img width="697" height="25" alt="image" src="https://github.com/user-attachments/assets/58fef301-ed42-4289-9d2e-5e6b23db7f06" />

y ahora estos cuatro

<img width="893" height="341" alt="image" src="https://github.com/user-attachments/assets/702ffa5b-6ebf-4ec6-8d51-17482f585d80" />

ahora tenemos que crear los grupos para ello primero creamos el archivo

<img width="793" height="56" alt="image" src="https://github.com/user-attachments/assets/876ceb39-cc20-4b82-b672-abaf44bd151e" />

y le ponemos este contenido

<img width="749" height="179" alt="image" src="https://github.com/user-attachments/assets/0b463b3d-08bf-4926-b3fd-c63ce8ff90cc" />

para crear las carpetas hacemos lo siguiente

<img width="764" height="82" alt="image" src="https://github.com/user-attachments/assets/aaa6dfd3-8e0e-4156-b4bc-891f0c196118" />

ponemos algo para ver que funcionan

<img width="1029" height="147" alt="image" src="https://github.com/user-attachments/assets/162a6545-d09c-4f70-a2b1-6de8d902c055" />

ahora editamos el archivo de configuracion para proteger estas carpetas

<img width="978" height="35" alt="image" src="https://github.com/user-attachments/assets/1b815ea9-f2da-47d6-a220-3a829340457a" />

y le agregamos esto despues de la parte de la actividad anterior

<img width="652" height="368" alt="image" src="https://github.com/user-attachments/assets/da683458-8612-4fd2-b671-48d7cf19e04b" />

ahora comprobamos si esta bien escrito y reiniciamos

<img width="1023" height="128" alt="image" src="https://github.com/user-attachments/assets/ec6092ed-8252-462c-866e-4e7bd841a883" />


### Acivity#8 - Autentificacion

primero activamos el modulo y reiniciamos apache

<img width="801" height="179" alt="image" src="https://github.com/user-attachments/assets/95aaaea0-c99b-4859-b310-c7acabb3b5ce" />

ahora vamos a crear las carpetas

<img width="861" height="94" alt="image" src="https://github.com/user-attachments/assets/d9e9b60b-1585-4ab8-8da8-41b6f6d87cc3" />

creamos un archivo de prueba para cada uno

<img width="1026" height="150" alt="image" src="https://github.com/user-attachments/assets/fd411e85-68c7-46b9-ae96-dea1f73459ab" />

creamos el usuario y el archivo

<img width="892" height="136" alt="image" src="https://github.com/user-attachments/assets/dd2c4978-f2aa-45e5-8fa4-d359944c0f69" />

creamos el sugundo usuario

<img width="896" height="147" alt="image" src="https://github.com/user-attachments/assets/7f30c92a-163a-49bb-a9d8-f2cca64943e2" />

ahora tenemos que configurar el archivo de configuracion

<img width="993" height="39" alt="image" src="https://github.com/user-attachments/assets/9b496a03-1518-4b1f-a06a-f9a1b49eccb4" />

y añadimos esta configuracion

<img width="992" height="617" alt="image" src="https://github.com/user-attachments/assets/fe39cad3-6c0a-4497-b075-bada9ecc65b8" />

verificamos la sintaxis

<img width="1027" height="149" alt="image" src="https://github.com/user-attachments/assets/a0d06470-b6cb-4008-ae08-386f9595c11b" />

y reiniciamos apache

<img width="749" height="53" alt="image" src="https://github.com/user-attachments/assets/f2f451a4-3005-42a7-932c-aff9d77f8c2a" />

ahora intentamos entrar como pepe al grupo 1 

<img width="657" height="361" alt="image" src="https://github.com/user-attachments/assets/c24a4c94-3547-416f-83fc-d8a2baa23f69" />

y como podemos ver va

<img width="661" height="135" alt="image" src="https://github.com/user-attachments/assets/7775abbb-a7ba-49f6-a08a-6294e64a4468" />

ahora para esta vamos a hacer que falle primero intentando entrar con pepe

<img width="876" height="340" alt="image" src="https://github.com/user-attachments/assets/2c1fb355-42eb-4649-a9ac-b721514b8bd4" />

como se puede ver no entra y vuelve a pedir usuario y contraseña ahora le vamos a poner juan

<img width="923" height="334" alt="image" src="https://github.com/user-attachments/assets/335f2d18-15fc-48b7-b688-7d983355094d" />

y como se puede ver entra perfectamente

<img width="622" height="150" alt="image" src="https://github.com/user-attachments/assets/72d9060c-7597-4db8-9986-e28d2e575372" />


### Activity#9 - Autentificacion

primero tenemos que instalar los paquetes necesarios

<img width="897" height="439" alt="image" src="https://github.com/user-attachments/assets/16045761-df8a-4fe8-a91a-aee148c428e8" />

<img width="1014" height="435" alt="image" src="https://github.com/user-attachments/assets/874c19b1-e94f-40cc-ac5e-188822b42b4f" />

ahora necesitaremos activar el modulo de apache para la base de datos

<img width="836" height="182" alt="image" src="https://github.com/user-attachments/assets/65945db2-6cfa-4d12-b9d6-111cad50f1e9" />

ahora tenemos que preparar la base de datos

<img width="703" height="212" alt="image" src="https://github.com/user-attachments/assets/1b3cfcec-6a0a-43da-87c5-19d58c2b06e8" />

creamos

<img width="423" height="56" alt="image" src="https://github.com/user-attachments/assets/9872511c-a5bc-48ac-a5f1-822d0b11321a" />

ponemos para usar la base de datos

<img width="328" height="60" alt="image" src="https://github.com/user-attachments/assets/7d449216-505e-483d-96e9-3ec661eb2925" />

creamos la tabla de usuarios

<img width="541" height="169" alt="image" src="https://github.com/user-attachments/assets/fc68d44d-daf9-4bac-8c87-33d25cf805a7" />

creamos un usuario

<img width="893" height="61" alt="image" src="https://github.com/user-attachments/assets/4ab886bb-9230-483b-9348-6349c14f1a36" />

y le damos permisos

<img width="732" height="61" alt="image" src="https://github.com/user-attachments/assets/a6a8faba-d730-4a61-801e-93141041acb3" />

ahora insertamos un usuario de prueba

<img width="993" height="102" alt="image" src="https://github.com/user-attachments/assets/ba6f2122-afee-4cc5-980f-0e96e9f6ef01" />

nos salimos

<img width="437" height="90" alt="image" src="https://github.com/user-attachments/assets/2d75ef87-133c-4e72-b04b-d5c7433a2818" />

ahora creamos la carpeta que vamos a proteger

<img width="1031" height="129" alt="image" src="https://github.com/user-attachments/assets/9e058f94-23ba-42d1-b81a-13aafce7c568" />

editamos el archivo de configuracion

<img width="926" height="30" alt="image" src="https://github.com/user-attachments/assets/b53976a3-9411-4c9b-b269-34492bdf27ba" />

y le añadimos esto

<img width="958" height="537" alt="image" src="https://github.com/user-attachments/assets/e2885d7e-72ad-498e-8d69-8b3be2e29538" />

comprobamos la sintaxis

<img width="1028" height="116" alt="image" src="https://github.com/user-attachments/assets/edb13617-2f3f-4fa7-ae9c-bb7e2ed4cde9" />

reiniciamos apache

<img width="697" height="52" alt="image" src="https://github.com/user-attachments/assets/8f63c652-d429-4020-ba6d-61db15820f66" />

ahora comprobamos entrando a la url y poniendo usuario y contraseña

<img width="788" height="328" alt="image" src="https://github.com/user-attachments/assets/87646d98-96ca-405a-a3b3-13424ccc3127" />


<img width="621" height="151" alt="image" src="https://github.com/user-attachments/assets/71736021-8e89-4327-bd5e-9e914efe08db" />


### Activity#10 - SSL

en nuestra instancia de AWS tenemos que instalar apache para ello primero hacemos un update

<img width="1109" height="649" alt="image" src="https://github.com/user-attachments/assets/8e868ebd-6c55-4691-9ca8-60013b74fa5f" />

y despues instalamos apache

<img width="1449" height="258" alt="image" src="https://github.com/user-attachments/assets/fac03d3b-7c26-4611-9d78-7bd45aa82df9" />

como podoemos ver entrando a la ip desde el navegador nos sale ya la pagina de por defecto de apache

<img width="1113" height="994" alt="image" src="https://github.com/user-attachments/assets/fa38a814-a726-49ce-9c55-e3698f8b758e" />

ahora tendremos que activar el modulo SSL

<img width="1012" height="301" alt="image" src="https://github.com/user-attachments/assets/7a2c83bc-fb8c-483d-8c99-b01434955639" />

y reinicamos apache

<img width="673" height="132" alt="image" src="https://github.com/user-attachments/assets/d434463e-f318-4222-a035-d6f8b8cae680" />

ahora vamos a generar el certificado, ejecutamos el siguiente comando
tenemos que responder las siguientes preguntas para hacerlo en la captura se ve, y en la ultima ponemos nuestra ip publica

<img width="1919" height="528" alt="image" src="https://github.com/user-attachments/assets/93028441-670f-4f71-9b33-2258ce256d60" />

ahora tenemos que en los archivos de configuracion decir donde tenemos los archivos nuevos

<img width="878" height="118" alt="image" src="https://github.com/user-attachments/assets/a39bf14e-cc50-4c85-9ba5-68a8a3c74bb6" />

y tenemos que modificar las dos lineas marcadas en el cuadro rojo para dar la ubicacion correcta

<img width="1312" height="839" alt="image" src="https://github.com/user-attachments/assets/e740454c-65bd-49ad-872d-7b2eedf957f5" />

ahora tenemos que "encender" el sitio web y reiniciar apache despues

<img width="668" height="198" alt="image" src="https://github.com/user-attachments/assets/1df6d1f6-7aa0-44db-a960-5a0213295ef5" />

ahora entramos a la https://(la ip publica) y como vemos nos aparece la pantalla de que nos es seguro

<img width="1576" height="626" alt="image" src="https://github.com/user-attachments/assets/82334224-1198-4d28-8037-ab6eb5b8c0b7" />

ahora tenemos que consegui que nuestra web sea segura para ello primero entraremos en esta web

<img width="1905" height="1007" alt="image" src="https://github.com/user-attachments/assets/e0594f1d-9448-489a-9356-50218d405971" />

en la que nos vamos a registrar y haremos clic despues donde pone dynamic DNS hostname

<img width="1919" height="910" alt="image" src="https://github.com/user-attachments/assets/4ab74301-a2f1-41a4-91f6-6b820b07b51e" />

y despues le damos a create hostname

<img width="1919" height="600" alt="image" src="https://github.com/user-attachments/assets/3533b6a3-981f-414f-a871-07d5f4b6f9d1" />

aqui tendremos que ponerle nombre y poner la ip publica de nuestra maquina en mi caso va a ser asi

<img width="1522" height="453" alt="image" src="https://github.com/user-attachments/assets/ccd5aa95-ca72-4f6f-9c79-fb05c5e9533b" />

ahora vamos a instalar cerbot para ello vovemos a la maquina

<img width="1895" height="328" alt="image" src="https://github.com/user-attachments/assets/1cc5672d-e146-4c56-bb9b-72a1cda7a563" />

ahora validamos nuestro domino

<img width="726" height="155" alt="image" src="https://github.com/user-attachments/assets/5a23856b-fc50-498f-84e2-1a364aa21b08" />

tendremos que responder a estas preguntas y al final poner el nombre que hemos elegido antes

<img width="1719" height="811" alt="image" src="https://github.com/user-attachments/assets/37593d4f-08c1-447a-a7e5-866f8a1adfd3" />

y ahora la prueba definitivaa vamos a entrar desde el navegador con el nombre que hemos elegido y no tendrias que salir que es peligroso

<img width="1203" height="1000" alt="image" src="https://github.com/user-attachments/assets/bd73111b-3e5f-485c-be39-99950b4c311e" />




