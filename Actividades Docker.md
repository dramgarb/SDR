## Actividad 0 y 1


primero actualizamos el sistema

<img width="564" height="164" alt="image" src="https://github.com/user-attachments/assets/fb06168e-19fb-4a13-9ece-58cc059d8b52" />

instalamos docker por el script oficial

<img width="1016" height="180" alt="image" src="https://github.com/user-attachments/assets/41f77913-e2e6-4b05-9c55-736781d78cb0" />

ahora le damos permisos al usuario

<img width="336" height="51" alt="image" src="https://github.com/user-attachments/assets/48e952aa-ab36-49f2-8542-95b6971af406" />

ahora vemos el hello world

<img width="1001" height="376" alt="image" src="https://github.com/user-attachments/assets/4a00d954-c1dd-471b-8bbc-3e6c848a010f" />

ahora la imagen y la verificamos

<img width="1014" height="229" alt="image" src="https://github.com/user-attachments/assets/47b5c239-0a3d-4f62-a4de-9389efc87c3d" />

y arrancamos el contenedor

<img width="552" height="36" alt="image" src="https://github.com/user-attachments/assets/d569f0c2-8ae5-4f67-9d90-9281a7b6b2c7" />

creamos un volumen

<img width="387" height="36" alt="image" src="https://github.com/user-attachments/assets/86a9fdbb-a176-4040-b18f-adbab219afbb" />

## Actividad 2

vamos a crear el contenedor interactivo

<img width="656" height="176" alt="image" src="https://github.com/user-attachments/assets/e575f45a-e558-4ae3-a56a-5312ce5672b1" />

este el contenedor en segundo plano

<img width="677" height="264" alt="image" src="https://github.com/user-attachments/assets/fe12045a-9a82-4910-a510-6b9704988e74" />

los listamos y hay los vemos

<img width="1032" height="167" alt="image" src="https://github.com/user-attachments/assets/cab0dfaa-2ebd-4446-84a9-7ef4e80b892a" />

y ahora lo paramos lo borramos y vemos que no esta

<img width="803" height="153" alt="image" src="https://github.com/user-attachments/assets/cc8bb261-d2d1-4b97-9703-3f1f9d8a1958" />

## Actividad 3

primero descargamos la imagen de ubuntu

<img width="588" height="113" alt="image" src="https://github.com/user-attachments/assets/124de823-553c-4027-a95a-07029dd3b4a2" />

ahora la de hello world

<img width="606" height="103" alt="image" src="https://github.com/user-attachments/assets/6a946c8e-b6ed-4dcb-9ac8-04c5cbd770ee" />

descargamos la de nginx

<img width="655" height="101" alt="image" src="https://github.com/user-attachments/assets/28dd1308-b09e-4af9-bdf9-104bdeb6426a" />

y aqui las vemos

<img width="716" height="117" alt="image" src="https://github.com/user-attachments/assets/deb2535e-fd6f-4eae-9cbe-102b3bab4631" />

ahora vamos a ejecutar hello world con nombres

<img width="913" height="284" alt="image" src="https://github.com/user-attachments/assets/46b38408-1bb5-4cd1-be21-aacb9ad8a7c3" />

<img width="816" height="310" alt="image" src="https://github.com/user-attachments/assets/914e1f62-ab93-4bde-a52d-32ce00ff6d4c" />

<img width="724" height="323" alt="image" src="https://github.com/user-attachments/assets/1112035e-ffe4-4012-b9d0-c19266bebb44" />

y aqui las vemos

<img width="963" height="134" alt="image" src="https://github.com/user-attachments/assets/a7446548-c9a7-4d1a-b37c-6a62020b781e" />

para pararlos seria

docker stop myhello1
docker stop myhello2

ahora borramos el 1

<img width="941" height="140" alt="image" src="https://github.com/user-attachments/assets/b87aac48-4d9d-4dcd-815a-3ba6e330165e" />

y para borrar todos el siguiente

<img width="529" height="132" alt="image" src="https://github.com/user-attachments/assets/81f7b0dd-1260-4249-aa76-bbbed7cbf848" />

## Actividad 4

Vamos a crear una carpeta en tu servidor Ubuntu, meter un archivo HTML y hacer que un contenedor Nginx lo lea

<img width="531" height="50" alt="image" src="https://github.com/user-attachments/assets/90ae1982-6465-4c7f-b051-98eed88e7c72" />

creamos un index

<img width="412" height="34" alt="image" src="https://github.com/user-attachments/assets/74287d25-3e11-438c-9f5f-52509c4f70bb" />

y lanzamos el contenedor

<img width="782" height="90" alt="image" src="https://github.com/user-attachments/assets/7f0b3b18-d6bc-4c0f-b34a-12a6b4dc2ed7" />

ahora creamos un volumen y vemos que esta

<img width="542" height="94" alt="image" src="https://github.com/user-attachments/assets/21fa912b-1299-4517-a737-94f8478f3d65" />

Arrancamos un contenedor Ubuntu interactivo montando ese volumen en /datos

<img width="716" height="35" alt="image" src="https://github.com/user-attachments/assets/377d0179-a12f-429e-b2eb-31c70869c1ee" />

creamos un archivo dentro de datos

<img width="321" height="20" alt="image" src="https://github.com/user-attachments/assets/06f0a9f8-e146-4658-8b10-3a89a125c9cb" />

ahora borramos el contenedor

<img width="453" height="44" alt="image" src="https://github.com/user-attachments/assets/933dc7c7-1e11-49fe-8423-6ec098b1c255" />

creamos un contenedor nuevo usando el mismo volumen

<img width="770" height="38" alt="image" src="https://github.com/user-attachments/assets/e2c30893-a4b4-418f-af65-9fc4321a3c73" />

y vemos que el archivo sigue estando

<img width="724" height="99" alt="image" src="https://github.com/user-attachments/assets/78a65635-4674-428e-97cb-413291b2f503" />

y limpiamos el entorno

<img width="521" height="83" alt="image" src="https://github.com/user-attachments/assets/bac65c9e-0c28-4864-abd8-fb72dee0e902" />

## Actividad 5

Ejemplo 1: Despliegue básico de un servicio
Creamos un archivo `docker-compose.yml` para levantar un servidor web Nginx, mapeando el puerto 8082. 
\`\`\`bash
docker compose up -d
docker compose ps
\`\`\`

Ejemplo 2: Aplicación Multicontenedor (WordPress + MariaDB)
Definimos una infraestructura más compleja con dos servicios interconectados. Compose se encarga de crear automáticamente una red interna para que WordPress pueda comunicarse con la base de datos MariaDB utilizando variables de entorno.
\`\`\`bash
docker compose up -d
\`\`\`

Ejemplo 3: Gestión del ciclo de vida (Logs y Down)
Comprobamos el funcionamiento de los servicios inspeccionando los registros combinados y, posteriormente, destruimos la infraestructura de forma limpia. El comando `down` elimina los contenedores y la red creada específicamente para ellos, dejando el sistema limpio.
\`\`\`bash
docker compose logs
docker compose down
\`\`\`

## Actividad 6

Ejemplo 1: Creación de imagen a partir de un contenedor (`docker commit`)
Lanzamos un contenedor basado en Ubuntu, le instalamos paquetes adicionales y creamos un archivo en su interior. Posteriormente, detuvimos el contenedor y guardamos su estado actual como una nueva imagen utilizando `docker commit`.
\`\`\`bash
docker commit mi_ubuntu_base mi_imagen_manual:v1
docker images | grep mi_imagen_manual
\`\`\`

Ejemplo 2: Creación automatizada mediante `Dockerfile`
Aplicamos las buenas prácticas del sector creando un archivo `Dockerfile`. Partiendo de una imagen base ligera (`nginx:alpine`), copiamos un archivo `index.html` personalizado hacia la ruta pública del servidor y expusimos el puerto 80.
\`\`\`bash
docker build -t mi_web_nginx:v1 .
\`\`\`


Ejemplo 3: Versionado e inspección del historial de capas
Para comprender cómo Docker optimiza el almacenamiento, utilizamos `docker history` para visualizar las distintas capas que componen nuestra imagen generada por el `Dockerfile`. Finalmente, usamos el comando `docker tag` para añadir una etiqueta de versión adicional (`latest`).
\`\`\`bash
docker history mi_web_nginx:v1
docker tag mi_web_nginx:v1 mi_web_nginx:latest
docker images | grep mi_web_nginx
\`\`\`
