# sistemas distribuidos

app web | movil con mucho transito -usan-> sist distibuidos

usuarios -se conectan-> cliente-servidor
cliente: navegador
servidor: -es su propio-> sistema distribuido
-siguen un patron -> por capas
-se utiliza un equilibrador de carga para delefar las solicitudes a muchos nodos logicos de servidor que se comunican a traves de sistemas de cola de mensajes

    Kubernetes:
    herramienta -usada en-> sistemas distribuidos
    puede crear un SD a partir de una coleccion de contenedores.
    los contenedores -crean-> nodos del SD
    K -orquesta-> la --comunicacion de red-- entre esos nodos
    K -gestiona-> el escalado dinamicos X,Y de los nodos del sistema

sistemas centralizados -evolucionan a-> sistemas distribuidos para gestionar escalado
