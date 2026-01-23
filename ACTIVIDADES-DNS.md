## Actividad 5

Primero hacemos un update

<img width="1056" height="531" alt="image" src="https://github.com/user-attachments/assets/d250163b-6a42-42a4-8640-ab06467ea3da" />

Instalar BIND9 y utilidades

<img width="1308" height="341" alt="image" src="https://github.com/user-attachments/assets/8edf6350-09d6-4c6f-8014-d7b8f9ba1172" />

Y verificamos que esta

<img width="1846" height="491" alt="image" src="https://github.com/user-attachments/assets/cab75cc3-37fe-45e8-ab6d-e41514d86272" />

Ahora configuramos para servidor cache

vamos al directorio de configuracion

<img width="680" height="117" alt="image" src="https://github.com/user-attachments/assets/2afd5a8e-7824-4be5-a435-a9a3eb0bf60a" />

y editamos el archivo de configuracion

<img width="1042" height="109" alt="image" src="https://github.com/user-attachments/assets/24485b7f-a708-4c58-9e81-7b68d7573da2" />

y lo ponemos asi

<img width="996" height="810" alt="image" src="https://github.com/user-attachments/assets/ae182d68-0423-4b0b-b558-25668e8b4eb3" />

comprobamos la sintaxis

<img width="537" height="121" alt="image" src="https://github.com/user-attachments/assets/513ded0e-dc9e-40ff-a23b-cc044741d885" />

y reiniciamos

<img width="648" height="113" alt="image" src="https://github.com/user-attachments/assets/51178a62-358a-4df9-992b-28a7b66adc21" />

verificamos que no hay errores en el registro

<img width="1424" height="467" alt="image" src="https://github.com/user-attachments/assets/24b62cb1-7bd4-4f6b-b158-4f6f6fdad7b6" />

Configuración como Servidor Forwarding 

Ahora cambiamos la configuración,  en vez de preguntar a los raíces, le pasamos el trabajo a Google (8.8.8.8)

<img width="564" height="92" alt="image" src="https://github.com/user-attachments/assets/3753a727-8baf-43b2-afb2-ecde157fb2c8" />

y le cambiamos esto

<img width="1111" height="808" alt="image" src="https://github.com/user-attachments/assets/988eec8f-5daf-4554-9912-d9e846cba009" />

comprobacion de sintaxis

<img width="561" height="124" alt="image" src="https://github.com/user-attachments/assets/dc638992-fac0-41c5-9841-5a6788c48046" />

reiniciamos el servicio

<img width="685" height="118" alt="image" src="https://github.com/user-attachments/assets/33d0e7b3-373a-46d6-afa4-cff846a7ebad" />

volvemos a mirar que arranco bien

<img width="1424" height="207" alt="image" src="https://github.com/user-attachments/assets/b8185b85-9fa8-4172-976e-6f96d006a57d" />

ahora vamos a hacer una prueba como vemos en una hay respuesta de tiempo y la otra tiene 0 de tiempo de respuesta

<img width="934" height="820" alt="image" src="https://github.com/user-attachments/assets/82b43da5-24eb-4b9a-b81e-5bbdfc0b7d32" />


## Actividad 6

Primero, debemos decirle a BIND que él es el maestro de la zona

<img width="1050" height="418" alt="image" src="https://github.com/user-attachments/assets/41aa2464-ba98-4965-a19e-0e13c2d85844" />

y le ponemos esto

<img width="1387" height="472" alt="image" src="https://github.com/user-attachments/assets/e1ecb3e7-c970-4b82-b08c-f56a580fb8f2" />

Aquí definimos los nombres (ns1, www, mail) y les asignamos IPs.

<img width="861" height="37" alt="image" src="https://github.com/user-attachments/assets/c573e736-9727-4a2d-8183-ada5d9f9d84f" />

<img width="1231" height="827" alt="image" src="https://github.com/user-attachments/assets/cba1ba97-d7f0-4d20-a7e8-a569455859d6" />

ahora vamos a crear el archivo de la zona inversa

<img width="764" height="130" alt="image" src="https://github.com/user-attachments/assets/485244cf-5f79-46bd-8078-b4ac12b1d1b9" />

y dentro le ponemos esto

<img width="1267" height="821" alt="image" src="https://github.com/user-attachments/assets/b4e8c325-21f2-4ec1-a8d6-3a2efc9857cd" />

comprobamos que no hay errores

<img width="923" height="244" alt="image" src="https://github.com/user-attachments/assets/89dd86ac-3911-43a0-a576-c480e2d33955" />

reiniciamos

<img width="738" height="140" alt="image" src="https://github.com/user-attachments/assets/bb7972d2-9710-49b7-8f58-357d4e87b1a3" />

ahora para poder usar el windows de mi ordenador vamos a hacer lo siguiente

<img width="1821" height="801" alt="image" src="https://github.com/user-attachments/assets/a53f61c0-33dc-4407-927e-7a930700f531" />

y tenemos que modificar este archivo

<img width="825" height="181" alt="image" src="https://github.com/user-attachments/assets/e7f5b074-cd12-45e8-aa76-312269d11f63" />

ahora desde el windows hacemos lo siguiente

primero limpiamos el dns

<img width="557" height="193" alt="image" src="https://github.com/user-attachments/assets/3b5e1466-6f2b-4dcd-85d5-d285e4d82d26" />

