# SDR
## TEMA 0
### ACTIVIDADES DE INTRODUCCION

## Tema 1. Servidores Web
### Activity#1 - Instalación de Apache

#### 1. La arquitectura Web es un modelo compuesto de tres capas, ¿cuáles son y cuál es  la función de cada una de ellas?

#### 2. Una plataforma web es el entorno de desarrollo de software empleado para  diseñar y ejecutar un sitio web; destacan dos plataformas web, LAMP y WISA. Explica en qué consiste cada una de ellas.

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


