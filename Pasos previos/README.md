# 1º Foto del circuito de encendido alternativos.

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/2f0c0628-2f93-43a0-be24-33f6f21e959d" />

Este es el pantallazo de circuito de arduino, esta dividido en dos placas, uno es la placa de arduino y otro es la placa de prototipado.
La placa de protodipado esta dividido en varios agujeros y estan conectado en cinco en cinco a dirección horizontal.
La placa de arduino es donde ponemos todas las materiales que necesitamos, los dos que parecen bombilla uno de color rojo y el otro de azul se llaman diodo led, tienen dos palillos metálicos que se llaman cátodo y ánodo, el cátodo es negativo y el ánodo es positivo, los dos tienen el cátodo conectado GND ( tierra ) y los ánodos en resistencia de 220 voltios, sabemos que la resistencia es de 220V por su color de rojo rojo y marrón, y por último el otro lado de los dos resistencia tiene que estar conectado en algún pin y asi ya funciona.

# Foto de la programación de circuito.

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/509c851b-c719-4488-88e7-2d59050d8a3a" />

Mi programa empieza con dos int(esto es la variable) en este caso esta en el 7 y el 8, después sigue con el void setup (funciona en que se ejecuta una sola vez al inicio del programa), dentro de void setup esta el pinmode(terminal7, OUTPUT) y el pinmode(terminal7, OUTPUT), esto es que el 7 y el 8 esta como salida, desùés en seguida esta el void loop (es para crear un bucle), dentro de el está el digitalwrite(terminal7, HIGH) y el digitalwrite(terminal8, LOW), estos significa que un pin digital esta en alto (HIGH) y el otro en bajo (LOW) , y el delay(10) significa que al terminar los anteriores se espera 10 milisegundos y asi sigue la segunda parte pero cambiando el alto y el bajo de sitios(osea si en el anterios es 7 en lato y el 8 en bajo, en este caso es lo contrario, el 7 en bajo y el 8 en alto) y asi termina el programa.

# 2º Foto del circuito de pulsador.

<img src= "Imagenes/Fantastic Fulffy-Rottis.png" width="500" height="500" />

Este circuito su objetivo es al principio tiene que tener un diodo led encendido y cuando le das al pulsador enciende el que esta apagado y se apaga el que esta encendido y si sueltas el pulsador vuelve al principio de circuito.

# Foto de la programación de circuito.

<img src= "Imagenes/Captura de pantalla 2025-10-20 133800.png" width="500" height="500" />

Este programa enmpieza con cuatro variales que dos estan en terminales 7 y 8, uno es el pulsador y otro es su valor. Se sigue con un void setup, dentro suya tiene tres pinmode y un serial.begin, los tres pinmode tiene las dos terminales en outout(salida) y un pulsador en input(entrada), y el serial.begin(9600) es la velocidad que pasa desde el puerto USB a circuito. Después sigue con un void loop, dentro de el tiene el valor2= digitalRead(pulsador) (significa que el valor2 es igual que lee el pin digital de pulsador), después tiene dos if(comparación), en dentro de la primera tiene el valor que esta en alto, dos digitalWrite(escribir digitalmente) que uno dice que el terminal8 esta en bajo y el terminal 7 en alto, y un serial.println(pulsado) (significa que hace esto si esta pulsado) y asi inversamente.

# 3º Foto de potenciómetro.

<img src= "Imagenes/Smashing Amur.png" width="500" height="500" />

El objetivo de este programa es al cambiar el valor del potenciómetro la ilumidad del diodoled va cambia en que brilla más o menos.

# Foto de programación de circuito.

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/11d57d4d-09f8-4bce-93a5-29ee866e69ce" />

Este programación empieza con un variable int que dice que P2 = A2, después sigue con dos float(tipo de dato numérico que representa números de punto flotante o con decimales), uno que es el valor = 0, y el otro es el de creoauno, después sigue con un void setup, dentro de el tiene un serial.begin(9600), después sigue con un void loop, que dentro de el tiene el valor = analogRead(P2) (significa que el valor que en este casa que es 0 es igual que lea el estado del pin 2), después tiene un serial.println(valor) (significa que el valor se envía al puerto serie) y por lo último un delay(20) (significa se retrasa 20 milisegundos) y asi termina la programa.

# 4º Foto de mapeado.

<img src= "Imagenes/IMG_8885.jpeg" width="500" height="500" />

# Foto de prgramación de mapeado.

<img src= "Imagenes/Programación mapeado.png" width="500" height="500" />

# 5º Foto de ultrasonido.

<img src= "Imagenes/IMG_8997.jpeg" width="500" height="500" />

<img src= "Imagenes/IMG_8996.jpeg" width="500" height="500" />

<img src= "Imagenes/IMG_8998.jpeg" width="500" height="500" />

# Foto de programación ultrasonido.

<img src= "Imagenes/ultrasonido.png" width="500" height="500" />









