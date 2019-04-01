
# Proyecto-TJBot_txt
## Manual del ejercicio TJBot en texto
### 2.	PROYECTO TJ BOT
<div id="texto1">En esta sección vamos a juntar todo lo aprendido anteriormente para construir un TJBot con el <br>
que poder mantener una conversación. [6] </div>
<br> 
<br>
<br>
<div id="texto2">Para ello vamos a utilizar una Raspberry Pi3, la cual conectaremos a los servicios de conversación <br>
de Watson y así poder hacer hablar a nuestro robot.</div>
<br> 
<br>
<br>
<div id="texto2">Para ello vamos a utilizar una Raspberry Pi3, la cual conectaremos a los servicios de conversación <br>
de Watson y así poder hacer hablar a nuestro robot.</div>
<img id="img1" src="imagenes/Imagen1.png"> <br>
<p id="texto3"> El objetivo final será hacer que nuestro TJBot sea capaz de mantener una conversación con nosotros y obedezca algunas órdenes.</p>
<b> 1.1.	CÓMO CREAR A TJBOT </b> <br>
<b> 1.1.1.	RAPSBERRY PI3 </b>
<div id="texto4">Raspberry Pi es un computador de placa única. <br> <br> <br>
Para trabajar con la Raspberry Pi3 vamos a necesitar un  <br>
monitor, un ratón, un teclado y una fuente de <br>
alimentación para trabajar con ella. También debemos <br>
tener una tarjeta micro SD con el sistema operativo <br>
instalado, en este caso trabajaremos con el sistema <br>
operativo Raspbian.</div>
<img id="img2"src="imagenes/Imagen2.png"> <br><br>
<div id="texto5"> Para crear nuestro TJBot hace falta conectar algunos componentes más a nuestra placa: </div>
<div id="lista"> 
<ul> 
<li>Un micrófono</li>
<li>Un altavoz</li>
<li>Una cámara</li>
<li>Un servomotor</li>
<li>LED</li>
</ul>
</div> <br> 
<b> 1.2.	MONTANDO A TJBOT </b> <br>
<div id="texto6"> 
Para comenzar a trabajar con TJBot, lo primero que debemos hacer es obtener las piezas para <br>
poder montarlo.
<br> <br>
Este robot es DY (Do it yourself) y puede conseguirse imprimiendo las piezas en una impresora <br>
3D. Las piezas que se deben imprimir pueden encontrarse en la siguiente web:
<br> <br> <br> 
<a href="https://ibmtjbot.github.io/#gettj"> https://ibmtjbot.github.io/#gettj</a> <br> <br> <br>
Las piezas que conseguiremos serán las siguientes: <br> <br>
<img src="imagenes/Imagen3.png" id="img3"> <br> <br> <br>
¿Cómo lo montamos? <br> <br> <br>
<div> Primero, insertamos las piernas en la mandíbula. Las piernas entran en los agujeros en forma de <br>
 L en la mandíbula. Inserta desde la parte superior de la mandíbula hacia abajo. </div> <br> <br> <br>
<img src="imagenes/Imagen4.png" id="img4"> <br>
<div> Después, cogemos la pieza "leg brace". Se encuentra en los dos orificios rectangulares en las <br>
patas debajo de la mandíbula. Mantiene las piernas rectas y soporta la mandíbula. Debemos <br>
 asegurar que esté orientada de modo que haga contacto con la parte inferior de la mandíbula. </div> <br> <br>
<img src="imagenes/Imagen5.png"id="img5"> <br> <br> <br>
<div> Ahora, cogemos los pies y los insertamos en las muescas de la pierna como se muestra a <br>
 continuación. Inserta los pies desde el exterior de cada pierna. </div> <br> <br> <br>
<img src="imagenes/Imagen6.png" id="img6"> <br> <br> <br>
<div> Si tenemos un servo motor, es hora de insertarlo en el orificio del lado izquierdo en la mandíbula. <br>
Cogemos el retenedor inferior y lo deslizamos hacia abajo a través de los agujeros en forma de L <br>
en las patas. Los brazos de soporte en la parte inferior de este retenedor deben caber en las <br>
 muescas de acoplamiento en la mandíbula. </div> <br> <br> <br>
<img src="imagenes/Imagen7.png" id="img7"> <br> <br> <br>
<div> A continuación, insertaremos la Raspberry Pi. Se monta boca abajo, con sus puertos expuestos a <br>
través de los tres agujeros en la mandíbula. <br> <br>
Si tenemos una cámara: tomamos el soporte de montaje de la cámara. Deslizamos los dos <br>
montajes laterales de la cámara en las muescas en la parte delantera del retenedor. Deslizamos <br>
la cámara Pi en el soporte y luego agregue los reforzadores superior y frontal para mantener la <br>
 cámara ajustada. </div> <br> <br> <br> 
<img src="imagenes/Imagen8.png" id="img8"> <br> <br> <br>
<div> El siguiente retenedor es el que tiene el pequeño círculo grabado en él. Lo añadimos a TJBot <br>
deslizándolo a través de los orificios en forma de L, con el círculo pequeño orientado hacia la <br>
derecha. Deslizamos el retenedor hacia abajo hasta que se encuentre con la parte superior de la <br>
 Raspberry Pi.</div> <br> <br> <br>
<img src="imagenes/Imagen9.png" id="img9"> <br> <br> <br>
 <div> Insertamos el LED en el orificio central del retenedor pequeño. </div> <br> <br> <br>
<img src="imagenes/Imagen10.png" id="img10"> <br> <br> <br>
Por último, colocamos la cabeza. <br> <br> <br>
<img src="imagenes/Imagen11.png" id="img11"> <br> <br> <br>
¡Ya está listo nuestro TJBot! <br> <br> <br>
</div> <br>
<b> 1.2.1. CÓMO CONECTAR LOS COMPONENTES </b> <br> <br>
<div id="texto7">A continuación, se muestra un esquema de la conexión de los diferentes componentes electrónicos que forman parte de nuestro TJBot. <br> <br> <br>
<img src="imagenes/Imagen12.png" id="img12"> <br> <br>
</div>
<b> 1.3.	SERVICIOS DE WATSON </b> <br>
<div id="texto8"> Para realizar el proyecto final del TJBot, vamos a utilizar tres servicios de Watson: Text to Speech,<br>
 Speech to Text y Watson Assistant.</div>
<b> 1.3.1.	TEXT TO SPEECH </b> <br> <br>
<div id="texto9"> El servicio Text to Speech proporciona una interfaz de programación de aplicaciones que utiliza  <br>
las capacidades de síntesis de voz de IBM para convertir texto escrito en voz de sonido natural. <br> <br> <br>
Para crear un servicio Text to Speech de Watson, debemos buscarlo en el catálogo de IBM Cloud. <br> <br> <br>
</div>
<img src="imagenes/Imagen13.png" id="img13"> <br> <br>
<div id="texto10"> Una vez seleccionado el servicio deseado, le damos al botón de "Crear" para poder empezar a trabajar.</div> <br> <br>
<img src="imagenes/Imagen14.png" id="img14"> <br> <br>
<div id="texto11"> Cuando ya tenemos nuestro servicio creado, podemos acceder a él desde nuestro Dashboard.</div> <br> <br>
<img src="imagenes/Imagen15.png" id="img14"> <br> <br>
<div id="texto12"> En el apartado Service credentials (credenciales del servicio) podemos ver nuestro usuario y <br>
contraseña, que necesitaremos incluir más adelantes cuando configuremos el servicio Text to <br>
Speech en nuestra Raspberry Pi3.</div> <br>
<div id="texto13"> ¡Hemos creado nuestro servicio Text to Speech! </div> <br> <br>
<b> 1.3.2.	SPEECH TO TEXT </b> <br> <br>
<div id="texto14"> Para crear un servicio Speech to Text de Watson, debemos buscarlo en el catálogo de IBM Cloud.</div> <br>
<img src="imagenes/Imagen16.png" id="img16"> <br> <br>
<div id="texto15"> Una vez seleccionado el servicio deseado, le damos al botón de "Crear" para poder empezar a trabajar.</div> <br> <br>
<img src="imagenes/Imagen17.png" id="img17"> <br> <br>
<div id="texto16"> Cuando ya tenemos nuestro servicio creado, podemos acceder a él desde nuestro Dashboard.</div> <br> <br>
<img src="imagenes/Imagen18.png" id="img18"> <br> <br>
<div id="texto17"> En el apartado Service credentials (credenciales del servicio) podemos ver nuestro usuario y <br>
contraseña, que necesitaremos incluir más adelantes cuando configuremos el servicio Speech to <br>
Text en nuestra Raspberry Pi3. </div> <br> 
<div id="texto18">¡Hemos creado nuestro servicio Speech to Text!</div>
<b> 1.3.3.	ASSISTANT </b> <br>
<div id="texto19"> Para crear un servicio de Watson Assistant, debemos buscar el servicio deseado en el catálogo de IBM Cloud.</div> <br> <br>
<img src="imagenes/Imagen19.png" id="img19"> <br> <br>
<div id="texto20"> Una vez seleccionado el servicio Assistant, le damos al botón de "Crear" para poder empezar a trabajar.</div> <br> <br>
<img src="imagenes/Imagen20.png" id="img20"> <br> <br>
<div> Cuando ya tenemos nuestro servicio creado, podemos acceder a él desde nuestro Dashboard.<br>
Una vez la página principal de nuestro servicio, debemos buscar el botón "Launch tool" que nos llevará a la herramienta <br>
en la que configuraremos y desarrollaremos nuestra conversación. <br>
En el apartado Service credentials (credenciales del servicio) podemos ver nuestro usuario y contraseña, que <br>
 necesitaremos incluir más adelantes cuando configuremos el servicio Assistant en nuestra Raspberry Pi3. <br> <br>
</div>
<b> 1.4.	CONFIGURAR A TJBOT  </b> <br> <br>
<b> 1.4.1.	CONFIGURAR LA RASPBERRY PI 3  </b> <br> <br>
Como ya hemos mencionado, Raspberry Pi es similar a un computador completo, lo que significa que se necesita un monitor, ratón y teclado para utilizarla. [1] <br> <br>
Se puede conectar a un televisor a través de un cable HDMI. <br>
También será necesario conectar la Raspberry a la Wifi. <br>
En la mayoría de los kits Pi, la tarjeta SD ya está precargada con una imagen del sistema operativo Raspberry Pi.  <br>
Se debe colocar la tarjeta SD en la Pi, encender la Pi y seguir las instrucciones en la pantalla para completar la <br>
instalación del sistema operativo. <br>
Una vez tenemos todo preparado, hay que configurar los paquetes para empezar a trabajar. <br>
<br>
<br>
Abrimos un terminal en el Pi y ejecutamos los siguientes comandos para instalar la última versión de Node.js y <br>
npm (Node Package Manager). Necesitará estos paquetes más tarde para ejecutar su código. <br>
Para ello utilizamos el siguiente comando: <br>
curl -sL http://ibm.biz/tjbot-bootstrap | sudo sh - <br>
A continuación, será necesario configurar la salida de audio; el audio puede tener 2 opciones: <br>
HDMI o Jack. <br>
Abrimos un terminal, y escribimos el siguiente comando, para abrir la configuración de las Raspberry: <br> <br>
sudo raspi-config <br>
</div>
<img src="imagenes/Imagen21.png"> <br> <br>
<div> Seleccionamos "Opciones avanzadas" y luego seleccionamos "Audio". Elegimos el canal correcto <br>
para el audio de salida. Si hemos conectado un altavoz externo a la toma de audio, debemos seleccionar la toma de 3,5 mm.
</div> <br> 
<img src="imagenes/Imagen22.png"> <br> <br>
<b> 1.4.2.	OBTENER EL CÓDIGO PARA TJBOT </b> <br> 
<div> Una vez tenemos todo configurado, necesitamos descargar el código base para el TJBot. <br>
Podemos hacerlo mediante los siguientes comandos: <br> <br> 
git clone https://github.com/ibmtjbot/tjbot.git cd tjbot/recipes/conversation <br>
npm install <br>
Una vez tenemos el código instalado, tenemos que empezar a configurar los servicios de Watson. <br>
Como ya hemos dicho, los servicios que vamos a utilizar son 3: Text to Speech, Assistant y Speech to Text.
</div>
<img src="imagenes/Imagen23.png"> <br> <br>
<div> Recordemos que los tres servicios estaban ya creados; ahora lo único que necesitaremos serán <br>
las credenciales para poder añadirlas al código de configuración del TJBot. <br>
Necesitamos abrir el archivo config.js para actualizar dicha información. Para ello, primero <br>
hacemos una copia del archivo original (config.default.js) mediante el siguiente comando: <br>
cp config.default.js config.js <br>
Una vez hecho, abrimos el archive config.js y actualizamos las credenciales de los servicios. <br>
Será necesaria la password, el username y en el caso de Watson Assistant, el WorkspaceID. <br>
</div>
<img src="imagenes/Imagen24.png"> <br> <br>
<b> 1.4.3.	PROBANDO A TJBOT </b> <br> 
<div> Una vez tenemos todo configurado y la conversación creada, podemos probar a TJBot. <br>
Abrimos el terminal y ejecutamos el siguiente comando: <br>
sudo node conversation.js <br>
</div>
<b> ¡Ya puedes hablar con TJBot! </b>

