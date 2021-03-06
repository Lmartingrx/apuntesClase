# Apuntes de clase

**Esto pretende ser un repositorio sobre las cosas que vamos viendo en clase y material extra al respecto**

## 1 - Comandos básicos de consola Cygwin

La consola Cygwin es un emulador de la consola de Linux en Windows."Se encarga de que instrucciones para sistemas Unix funcionen en un entorno Windows." Más información sobre Cygwin e instalación [aquí](https://fuubar.wordpress.com/2014/01/14/cygwin-creyendome-un-chico-linux-en-windows-parte-i./). Para profundizar más en los comandos de Linux, mirar [este índice](http://ss64.com/bash/).
<ul>
  <li>
  <code>$</code>Indica que somos usuarios normales.
  </li>
  
  <li>
  <code>#</code> Indica que somos administradores.
  </li>
  
  <li>
  <code>pwd </code>Print Working directory. Te dice el punto de partida en la estructura de ficheros.
  </li>
  
  <li>
  <code>ls</code> Te da información sobre los ficheros que hay en un directorio.
  </li>
  
  <li>
  <code>cd </code>Change Directory. Te traslada a otro directorio. cd / nos lleva a la raíz del sistema.
  </li>
  <li>
  <code>mv </code>cambiar nombre de directorio o fichero. El comando "mv mitexto.txt mitextoNuevo.txt" Cambiara el nombre del fichero mitexto por el otro.
  </li>
  
  <li>
  <code>mkdir nuevaCarpeta</code> Crea una nueva carpeta.
  </li>
  
  <li>
  <code>touch nuevoFichero</code> Crea un fichero.
  </li>
  
  <li>
  <code>file nuevoFichero</code> Te da la metadata de nuevoFichero.
  </li>
   <li>
  <code>echo "Empieza el Readme" > Readme.md</code> Crea un readme con las palabras que están entre comillas.
  </li>
  <li>
  <code>echo "Continua el Readme" >> Readme.md</code> Continua el readme anterior con las palabras que están entre comillas.
  </li>
  <li>
  <code>rm -rf nombreCarpeta</code> Borra una carpeta del sistema. -r quiere decir que se borre todo el contenido de la carpeta. -f quiere decir que se borre absolutamente del sistema.
  </li>
  <li>
  <code>more nombreFichero</code> Ver contenido del fichero
  </li>
  <li>
  <code>unzip nombreZip</code> Descomprimir zip
  </li>
  <li>
  <code>mv nombreDirectorio/ otroDirectorio/</code>mover nombreDirectorio a otroDirectorio
  </li>
   <li>
  <code>mc nombreZip</code> copiar zip
  </li>
  <li>
  <code>cd</code> Volver a la raíz
  </li>
</ul>
### 1.1 - El archivo .bash_history
corresponde a un archivo de registro o logs que guarda los comandos ejecutados en bash por un usuario en particular, cuando un usuario ingresa vía ssh a un sistema por ejemplo, ejecuta los típicos comandos “dir, cd, ls” y estos quedan registrados. [Más información](https://blog.zerial.org/seguridad/cosas-que-encontramos-en-los-archivos-bash_history/).

### 1.2 - Cambiar la ruta absoluta en Cygwin
De la carpeta de instalación a windows. Se hace de la siguiente manera: llendo al archivo de configuración con Emacs (/etc/nsswitch.conf), o navegando a través del interfaz del sistema operativo. Después se abre este archivo (nsswitch.conf) con Emacs o con otro editor de texto y se pone windows en la variable db_home. Dejando comentado lo demás.

## 2 - Atajos en Emacs
Emacs es un editor de texto con una gran cantidad de funciones, muy popular entre programadores y usuarios técnicos. [Mas info](https://es.wikipedia.org/wiki/Emacs).
*     ctrl x + ctrl f
en emacs: te lleva a ruta de fichero para abrir
*     ctrl x + ctrl w
en emacs: guardar archivo
*     ctrl + y
pegar
*     ctrl x + b
modelo de varios buffers
*     ctrl x + 1
salir

## 3 - Instalando git a través de Cygwin
<ol>
  <li>bajarse el setup de cygwin e inicializarlo</li>
  <li>En select package, elegir <strong>git distributed version control system</strong></li>
  <li>Otros programas que también nos hemos descargado: git teaseratct, imagemagic xpdf</li>
</ol>

## 4 - Pasos en Github
1. <code>echo "Descripcion del fichero" >> Readme.md</code> crear un fichero Readme con una descripción.
1. <code>git init</code> iniciar un repositorio git local en tu máquina.
2. <code>git add README.md</code> vincular al repositorio git el Readme.
3. <code>git commit -m "first commit"</code> realizar un primer commit.
4. <code>git remote add origin https://github.com/Antonio-HR/gds.git</code> añadir al repositorio git remoto, el origen.
5. <code>git push -u origin master</code> subir al repositorio.







   





