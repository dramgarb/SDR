# Practica 1 Trimestre 2025

primero un update

<img width="887" height="148" alt="image" src="https://github.com/user-attachments/assets/11893856-cbb2-4c29-8ec9-498898b4bdc6" />

despues instalamos apache, mysql y php

<img width="1887" height="484" alt="image" src="https://github.com/user-attachments/assets/567b5a14-08f8-41f4-b768-6d741b5def18" />

ahora para preparar la base de datos hacemos lo siguiente

<img width="943" height="571" alt="image" src="https://github.com/user-attachments/assets/3d2fbe07-c9eb-4302-b6c4-8caa21ba984a" />

ahora vamos a descargar wordpress

haciendo el tercer comando se me an perdido y no he podido capturar pero serian estos los que hay que hacer

cd /tmp
wget https://wordpress.org/latest.tar.gz
tar -xzvf latest.tar.gz
sudo mv wordpress /var/www/centro
sudo chown -R www-data:www-data /var/www/centro
sudo chmod -R 755 /var/www/centro


ahora ceamos el virtual host

<img width="823" height="111" alt="image" src="https://github.com/user-attachments/assets/445e7b93-7b1e-4895-89f8-60e1165c0250" />

<img width="1206" height="851" alt="image" src="https://github.com/user-attachments/assets/3b528d88-f87b-4395-9fd2-f20c731c7e84" />

y lo activamos

<img width="837" height="183" alt="image" src="https://github.com/user-attachments/assets/7a2ab757-77c1-41d7-b8b2-1ff18c9589e5" />

instalamos el modulo WSGI

<img width="784" height="107" alt="image" src="https://github.com/user-attachments/assets/6f43f117-2d85-4353-a5d1-112de9f7aedb" />

creamos la app python 

<img width="795" height="129" alt="image" src="https://github.com/user-attachments/assets/cf8d79e9-4f65-4895-9eb1-90f174049931" />

<img width="749" height="101" alt="image" src="https://github.com/user-attachments/assets/4481e48e-f9e6-42e5-a84c-d04a7a2b7ca0" />

y ponemos este codigo dentro

<img width="1203" height="838" alt="image" src="https://github.com/user-attachments/assets/ed84bb62-ce10-4e27-b306-c49ea1e07701" />

creamos un virtual host

<img width="926" height="108" alt="image" src="https://github.com/user-attachments/assets/60c76b18-af64-4972-afc5-b58dafbc4442" />

dentro ponemos esto

<img width="1302" height="845" alt="image" src="https://github.com/user-attachments/assets/317ba48e-32bb-4d3d-a215-2bce40f98fde" />

ahora lo activamos

<img width="712" height="189" alt="image" src="https://github.com/user-attachments/assets/c3f0f835-7fb7-4d91-a24f-796d84156fcb" />

instalamos awstats

<img width="616" height="89" alt="image" src="https://github.com/user-attachments/assets/a2f7cb72-79ea-4d98-a9b0-273c6e107b39" />

<img width="1050" height="121" alt="image" src="https://github.com/user-attachments/assets/c373676c-3469-44b3-9564-40799cb9813d" />

habilitamos el modulo CGI en apache

<img width="631" height="204" alt="image" src="https://github.com/user-attachments/assets/55acdfbe-ddc4-4cda-be47-083937e05c8b" />

instalamos nginx

<img width="638" height="108" alt="image" src="https://github.com/user-attachments/assets/6874ad16-d7c3-4ab4-8dbc-93d062cb020d" />

cambiamos el puerto

<img width="772" height="110" alt="image" src="https://github.com/user-attachments/assets/d01332d9-0307-495e-a87b-da8733471a5e" />

cambiamos esas lineas

<img width="1156" height="826" alt="image" src="https://github.com/user-attachments/assets/2937ca21-6593-4bf1-9c45-cfb634f31969" />

reiniciamos

<img width="829" height="109" alt="image" src="https://github.com/user-attachments/assets/ca403bff-1ae9-4d4b-803b-4606c823ec30" />

instalamos php para nginx

<img width="694" height="115" alt="image" src="https://github.com/user-attachments/assets/8b18b1dc-54a3-4c17-907e-0d08a174f1a3" />

instalamos phpmyadmin

<img width="744" height="113" alt="image" src="https://github.com/user-attachments/assets/b4e693e9-1705-469b-85bd-2ba0c20d0001" />

ahora conectamos phpmyadmin y nginx

<img width="819" height="108" alt="image" src="https://github.com/user-attachments/assets/d8082a9e-d599-4af3-bbcd-d87939505fd9" />

configurar nginx para procesar php

<img width="809" height="104" alt="image" src="https://github.com/user-attachments/assets/030883a7-2e90-42ba-90a2-5833ae656601" />

lo ponemos asi

<img width="1064" height="823" alt="image" src="https://github.com/user-attachments/assets/58610306-b37b-479d-a875-6529f0c220eb" />

revisamos que esta bien

<img width="629" height="142" alt="image" src="https://github.com/user-attachments/assets/2764d303-ea2a-4adc-8379-71ecb4505898" />

reiniciamos

<img width="570" height="113" alt="image" src="https://github.com/user-attachments/assets/42d0def0-f962-4db5-94e9-03d99f58aa8e" />

COMPROBACIONES

<img width="1639" height="834" alt="image" src="https://github.com/user-attachments/assets/db3e6536-c52b-41cb-ba14-c946bcf93f0a" />

<img width="1401" height="473" alt="image" src="https://github.com/user-attachments/assets/5e6332c3-8388-44a1-83f0-0703cb83dad9" />

