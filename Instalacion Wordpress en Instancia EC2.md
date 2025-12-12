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

en configuracion de instancia ponemos la db.t3.micro

<img width="1467" height="386" alt="image" src="https://github.com/user-attachments/assets/a2973159-4d39-477e-919b-763e5de8626e" />

ahora en el apartado de conectividad tenemos que poner que no se conecte a un recurso informatico que use la nuve VCT que creamos antesy tenemos que crer un nuevo grupo de seguridad

<img width="1311" height="848" alt="image" src="https://github.com/user-attachments/assets/7a404363-faa0-47bb-9522-0b71b478a33c" />

es importante en configuracion adicional poner el nombre para la base de datos inicial

<img width="1225" height="413" alt="image" src="https://github.com/user-attachments/assets/88531bc2-e89e-4c1b-a699-1420498c234e" />

