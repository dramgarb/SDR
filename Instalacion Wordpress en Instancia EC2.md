# Practica de instalacion de wordpress en instacia EC2

primero tenemos que crear la vpc antes de comenzar la practica como tal


<img width="1911" height="960" alt="image" src="https://github.com/user-attachments/assets/565ef4fd-b311-473e-b638-7496d6fc422d" />

la tendremos que configurar

<img width="1794" height="915" alt="image" src="https://github.com/user-attachments/assets/d9505d9d-2543-4ac2-a113-837b2b43f46f" />

despues crearemos la instancia primero esta parte

<img width="1213" height="862" alt="image" src="https://github.com/user-attachments/assets/c698f6c0-5702-4e76-a00d-92def74ff02f" />

y despues esta parte

<img width="1262" height="899" alt="image" src="https://github.com/user-attachments/assets/a8e942ff-b786-4242-a69b-8e806acace0c" />

ahora nos conectamos y primero hacemos un update

<img width="860" height="396" alt="image" src="https://github.com/user-attachments/assets/a764f7ed-d8fd-49c9-9154-55e776a49581" />

ahora instalamos apache

<img width="851" height="520" alt="image" src="https://github.com/user-attachments/assets/4766b207-71ef-43c8-9ccf-35c6dccce72e" />

ahora arrancamos el servidor y hacemos que se inicie siempre automaticamente

<img width="821" height="73" alt="image" src="https://github.com/user-attachments/assets/26b43868-0b1a-4b15-8e6d-552fec718454" />

como vemos aqui lo tenemos

<img width="1031" height="998" alt="image" src="https://github.com/user-attachments/assets/8ceae75d-a92e-4571-961a-948fddc016ea" />

ahora vamos a instarlar php

<img width="817" height="449" alt="image" src="https://github.com/user-attachments/assets/b4cf4b8c-053b-4cf4-95b7-07f396d76df2" />

ahora reiniciamos apache y vemos la version de php

<img width="516" height="118" alt="image" src="https://github.com/user-attachments/assets/989ec8ba-5882-4b69-866a-51df5d9ee5e9" />

ahora instalamos el conector para la base de datps

<img width="443" height="76" alt="image" src="https://github.com/user-attachments/assets/c6bfa49a-3e2c-4707-b6e2-a0e87a724309" />

reiniciamos apache

<img width="445" height="32" alt="image" src="https://github.com/user-attachments/assets/a0789eb3-ea23-4372-88e0-507a7ebe2a79" />

ahora volvemos a la web de AWS y tenemos que enrar en el recurso de RDS y darle a crear una base de datos

<img width="1898" height="918" alt="image" src="https://github.com/user-attachments/assets/80b520e9-86a2-42e8-a2e1-d14c74879179" />

ahora aqui tenemos que configurar varias cosas como elegir creacion estandar y como motor elegimos MySQL

<img width="1833" height="822" alt="image" src="https://github.com/user-attachments/assets/e1894ffa-7e8a-44d0-af94-21ef62ce0b94" />

y aqui elegimos el desarrollo y pruebas como plantilla y de disponibilidad y durabilidad elegimos la de una instancia y disponibilidad unica

<img width="1699" height="768" alt="image" src="https://github.com/user-attachments/assets/3dc398e2-f168-4b37-a81d-d486f64f276f" />

ahora elegimos identificador, usuario. elegimos poder poner la contraseña, y ponemos una en mi caso Usuaio-1

<img width="1655" height="702" alt="image" src="https://github.com/user-attachments/assets/535ded04-3423-4a36-86a0-1c979b4618c5" />

tenemos que poner esto en la de almacenamiento

<img width="1411" height="410" alt="image" src="https://github.com/user-attachments/assets/be1db02a-44c3-4584-bdff-a00f5086534a" />

en configuracion de instancia ponemos la db.t3.micro

<img width="1467" height="386" alt="image" src="https://github.com/user-attachments/assets/a2973159-4d39-477e-919b-763e5de8626e" />

ahora en el apartado de conectividad tenemos que poner que no se conecte a un recurso informatico que use la nuve VCT que creamos antesy tenemos que crer un nuevo grupo de seguridad

<img width="1311" height="848" alt="image" src="https://github.com/user-attachments/assets/7a404363-faa0-47bb-9522-0b71b478a33c" />

es importante en configuracion adicional poner el nombre para la base de datos inicial

<img width="1225" height="413" alt="image" src="https://github.com/user-attachments/assets/88531bc2-e89e-4c1b-a699-1420498c234e" />

despues de la configuracion le damos a crear y empezara el proceso

<img width="1905" height="496" alt="image" src="https://github.com/user-attachments/assets/d5121c5f-2e82-469c-936b-9053d4061db9" />

al los minutos nos saldra ya un mensaje diciendo que se a crado correctamente

<img width="1909" height="572" alt="image" src="https://github.com/user-attachments/assets/6aa3f64f-89bd-4c85-9185-3ca7030f4b25" />

tendremos que marcarla y darle a acciones y a configurar conexion de EC2

<img width="1652" height="769" alt="image" src="https://github.com/user-attachments/assets/017ff6fc-d847-4880-b41a-ff1533c16623" />

marcamos la nuestra y le damos a continuar

<img width="1559" height="608" alt="image" src="https://github.com/user-attachments/assets/62c780fd-7ca3-43c1-b611-059d97cd9249" />

despues nos saldra el mensaje de que la conexion se a realizado con exito

<img width="1627" height="512" alt="image" src="https://github.com/user-attachments/assets/0b9d3620-5c18-4147-8d46-e3ed7e2de2a6" />

ahora tenemos que pasar a la parte de crear un dico duro compartido para ello buscamos este servicio

<img width="992" height="866" alt="image" src="https://github.com/user-attachments/assets/33b1f14e-57d4-4716-aa44-1bff76784bd6" />

y le damos a cerar un sistema de archivos

<img width="1753" height="838" alt="image" src="https://github.com/user-attachments/assets/ebfb8a6b-9564-4acb-b2fd-0bd15f552609" />

aqui elegimos el nombre y marcamos la VPC que creamos

<img width="868" height="864" alt="image" src="https://github.com/user-attachments/assets/c4307a59-1ad4-44f5-8e56-273335106856" />

y hay lo tendremos nos saldra el mensaje de listo

<img width="1716" height="586" alt="image" src="https://github.com/user-attachments/assets/e039c3e5-db4f-4d4b-9ce3-32c9d0bb6272" />

he perdido las capturas de todos los pasos que he avanzado en una hora voy a poner las cosas hechas

entramos en grupo de seguridad

<img width="926" height="906" alt="image" src="https://github.com/user-attachments/assets/1d8062bd-c4c6-48d5-b8cb-175dd9636f4c" />

entramos en el default

<img width="746" height="307" alt="image" src="https://github.com/user-attachments/assets/997416ca-ccab-49b9-9420-2e4c9b0877ac" />

y lo configuramos asi

<img width="1786" height="704" alt="image" src="https://github.com/user-attachments/assets/30502b08-2e17-489f-a4fa-222881669ba0" />

y despues los comando que he ejecutado fueron los siguiente

<img width="448" height="41" alt="image" src="https://github.com/user-attachments/assets/21111402-4271-41ef-884b-1d6688fd950c" />

<img width="258" height="39" alt="image" src="https://github.com/user-attachments/assets/d903f7a8-2264-4a20-a14b-438d44910c14" />

despues en AWS tenemos que copiar ese comando el primero poniendolo en IP y lo ejecutamos en la conexion ssh

<img width="1821" height="620" alt="image" src="https://github.com/user-attachments/assets/16cc08ff-6ab0-44e6-97f7-ecf7ed4ad1e9" />

<img width="853" height="53" alt="image" src="https://github.com/user-attachments/assets/e5ac19c5-789e-435c-b42d-745606e6ed83" />

despues nos vamos a esa carpeta

en estos comandos completamos los siguientes pasos:
- nos vamos a la carpeta
- borramos el archivo de bienvenida
- descargamos wordpress
- descomprimimos el archivo
- movemos los archivos a la carpeta principal
- y eleminamos la carpeta vacia y el comprimido

<img width="346" height="49" alt="image" src="https://github.com/user-attachments/assets/ed9ad7b7-c58a-4436-98fc-c8fc8224b9ef" />

<img width="363" height="30" alt="image" src="https://github.com/user-attachments/assets/5ad4fffc-143d-4f71-b63b-f49e074cae8c" />

<img width="564" height="44" alt="image" src="https://github.com/user-attachments/assets/4879416e-0ae7-4b4f-a595-1a2337964a53" />

<img width="499" height="25" alt="image" src="https://github.com/user-attachments/assets/b426951c-5b6d-47ba-bbb7-5245b2738708" />

<img width="358" height="32" alt="image" src="https://github.com/user-attachments/assets/6258d29f-c0b8-4475-b7e2-90128aa47654" />

<img width="398" height="35" alt="image" src="https://github.com/user-attachments/assets/d3b9c3e5-bb6a-4926-b7a4-303fa5d00eb4" />

<img width="413" height="53" alt="image" src="https://github.com/user-attachments/assets/3361f9e3-47a2-4081-b78d-ab54ea71c970" />


despues de esto ya puedo continuar por donde iba antes de perderlo todo

instalamos el cliente mysql

<img width="843" height="377" alt="image" src="https://github.com/user-attachments/assets/b4a594c0-1c8e-4ae8-a981-5067177605ed" />

