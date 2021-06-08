# born2beroot

### ¿Qué es una máquina virtual?
Una máquina virtual es un entorno simulado o virtual que funciona como un sistema con su propia CPU, memoria, interfaz de red y almacenamiento. Sin embargo, este entorno virtual se crea en un sistema de hardware físico. El software utilizado por una VM recibe el nombre de hipervisor, y su función es separar los recursos de la máquina del sistema de hardware e implementarlo adecuadamente para que la VM pueda acceder a ellos.
Toda máquina física equipada con un hipervisor se denomina host o anfitrión. Las diferentes VM que utilizan los recursos de la máquina host reciben el nombre de guests o invitados. El hipervisor gestiona así todos los recursos de la máquina host para que puedan ser utilizados por todas las máquinas guest.<br>
<br>
Una máquina virtual se encuentra aislada del resto del sistema, aunque puede haver más de una VM en un mismo sistema de hardware (servidor). Con esto, se consiguen ejecutar varios OS diferentes a la vez desde una misma máquina.

### ¿Cómo funciona una máquina virtual?
Las máquina virtuales se basan en el concepto de virtualización. La virtualización permite a un equipo compartir un mismo sistema con varios entornos virtuales. El hipervisor getiona el sistema de hardware y separa los recursos físicos de los entornos virtuales. Los recursos se dividen según las necesidades. Cuando la VM está en ejecución y un programa o un usuario requieren recursos adicionales del sistema, el hipervisor recibe la solicitud para posteriormente aceptarla o rechazarla.

### ¿Es aconsejable utilizar máquinas virtuales?
A día de hoy, la mayoría de las aplicaciones y OS que conforman un servidor solo necesitan utilizar una pequeña cantidad de los recursos físicos disponibles al momento de usarse. Si virtualizamos los servidores, podremos colocar muchos servidores virtuales para hacer un uso más eficiente de los recursos del hardware, sin necesidad de comprar o adquirir componentes extras.<br>
Por otro lado, al ser independiente al resto del sistema, todo lo que realicemos dentro de la VM solo afectarán a la propia VM. Así, son muy útiles para probar aplicaciones de prueba o nuevas distribuciones las cuales pueden llegar a ser inestables. Cualquier modificación que hagamos en alguno de estos programas, si lo hacemos dentro de una VM, no perjudicará al sistema en caso de error.

### ¿Qué es VirtualBox?
Software libre para la virtualización de equipos con arquitectura x86. Funciona como un hipervisor, creando una máquina virtual donde el usuario podrá ejecutar otros OS.<br>
El sistema operativo en el que se ejecuta VirtualBox es el host, mientras que el OS que utiliza la máquina es el invitado.

### ¿Por qué necesito un archivo .iso?
Para poder instalar un sisema operativo dentro de nuestra máquina virtual necesitaremos un archivo .iso, pero antes de explicar qué es y por qué lo necesitamos, es importante saber qué son los discos ópticos y para qué sirven:

<hr>
Los discos ópticos son unidades de almacenamiento de datos en formato digital. Tienen una forma circular y se suelen utilizar para guardar archivos multimedia como películas, imágenes y audio (aunque admite cualquier formato que pueda ser digitalizado). Para leer el contenido de los discos se utilizan unidades del disco óptico que leen la información por medio de un haz de luz laser. Para guardar la información, se utiliza el mismo concepto del haz de luz laser. Así, podemos clasificar los discos ópticos en:
<ul>
   <li>Read Only: solo se puede guardar información.</li>
   <li>Recordable: solo se permite una grabación.</li>
   <li>Rewritable: se puede almacenar información más de una vez. Se sobrescribe la información nueva.</li>
</ul>
Por otro lado, los discos ópticos pueden clasificarse (en función de su capacidad) en:
<ul>
   <li>CD: disco compacto conocido como CD-ROM, es la unidad de almacenamiento más simple. Se puede utilizar para almacenar cualquier información (predomina en archivos de audio).</li>
   <li>DVD: disco versátil digital, tiene mayor capacidad de almacenamiento que el CD.</li>
   <li>HD DVD: versión mejorada del DVD.</li>
   <li>Blue-Ray: tipo de disco estándar utilizado para archivos de formato vídeo en alta resolución.</li>
   <li>UMD: universal media disk, diseñado por Sony para almacenar juegos.</li>
</ul>
<hr>

Un archivo ISO es un archivo de almacenamiento que contiene una copia (o imagen) idéntica de los datos encontrados en un disco óptico, como un CD o un DVD. La mayoría de los OS permiten montar una imagen ISO como un disco virtual, en cuyo caso todas sus aplicaciones lo tratan como si se hubiese insertado un disco óptico real. A día de hoy es una práctica muy habitual instalar programas y OS a través de imágenes ISO ya que permiten descargar mucho archivos (incluidas dependencias de programas) con tan solo la descarga de un archivo .iso. Por tanto, nuestra imagen .iso será la que utilicemos para descargar nuestro OS dentro de nuestra máquina virtual, siendo totalmente igual a si introdujésemos un CD en el ordenador para instalar dicho OS.

### Debian vd CentOS
Para este projecto, solo podemos elegir entre Debian o CentOS. Por este motivo, tenemos que saber primero cuáles son las similitudes entre ambos, cuáles son sus diferencias y para qué uso está recomendado cada uno.
COMPARACION   | DEBIAN       | CENTOS
:-----------  | :----------- | :-----------
Nivel de experiencia necesario | Intermedio | Intermedio/Avanzado
Usuario Objetivo | Distribución de uso general | Centrado en administración de servidores y sistemas
Soporte Software | 10/10 | 8/10
Soporte Hardware | 9.5/10 | 7/10
Estabilidad | 10/10 | 9.5/10
Caso específico | Crear OS libre que puede ser instalado en casi todos los hardware y con gran estabilidad | Administrar un sistema con las ventajas que RHEL ofrece

### Diferencias entre apt y aptitude

### ¿Qué es KDump, SELinux y AppArmor?

### ¿Qué es una partición?

### ¿Qué es LVM?

### ¿Qué es el protocolo SSH?

### ¿Qué UFW?
