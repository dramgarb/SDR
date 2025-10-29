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

### Activity 3 - Directorios

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
