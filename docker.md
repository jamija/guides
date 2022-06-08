# Docker

administador de sistemas

la aplicacion se va a ejecutar en un entorno de produccion

contendores -- instalar

imagenes:

crear una imagen para nuestra aplicacion, loq ue luego nos va a permitir crear multiples instancias para nuestra imagen
docker build -t (taggg) nombreDeLaNuevaEtiqueta . (directorio donde esta la config, osea el dockerfile,)

docker run -p 7000:80 -d --name AppDeLaImagen LaNuevaImagen

ejecuto en el puerto 7000 de mi compu lo que vive en el puerto 80 del servidor
dockerHub: subir mis propias imagenes

docker build -t jamija/website .

docker login

docker push jamija/website

estamos subiendo
codigo biblioteca dependencias TODO

ejecutar el programa en otra compu...

integrar varios contenedores en tu imagen...
dockercompose.yml
docker compose --> especificar multiples contenedores y como se van a estar comunicando (networks)

---

postgres y pg admin en un contendor de docker en lugar de instalarlo localmente

crear programas para proyectos

cada servicio es un contendor ....
va a estar basado en una imagen ( osea en que instalador de docker)
port:

- puerto en el que quier que este disponible local: puerto en el que corre en gral

environments!!! darle configuracion inicial cuando inicie

depends_on: service1 (para que se ejecute despues de ese servicio)

dockerfile --->

especifica dependencias a nivel de sistema

WIP
