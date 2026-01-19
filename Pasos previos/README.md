# 1º Foto del circuito de encendido alternativos.

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/2f0c0628-2f93-43a0-be24-33f6f21e959d" />

Este es el pantallazo de circuito de arduino, esta dividido en dos placas, uno es la placa de arduino y otro es la placa de prototipado.

La placa de protodipado esta dividido en varios agujeros y estan conectado en cinco en cinco a dirección horizontal.

La placa de arduino es donde ponemos todas las materiales que necesitamos, los dos que parecen bombilla uno de color rojo y el otro de azul se llaman diodo led, tienen dos palillos metálicos que se llaman cátodo y ánodo, el cátodo es negativo y el ánodo es positivo, los dos tienen el cátodo conectado GND ( tierra ) y los ánodos en resistencia de 220 voltios, sabemos que la resistencia es de 220V por su color de rojo rojo y marrón, y por último el otro lado de los dos resistencia tiene que estar conectado en algún pin y asi ya funciona.

# Foto de la programación de circuito.

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/509c851b-c719-4488-88e7-2d59050d8a3a" />

Mi programa empieza con dos int(esto es la variable) en este caso esta en el 7 y el 8.

Después sigue con el void setup (funciona en que se ejecuta una sola vez al inicio del programa), dentro de void setup esta el pinmode(terminal7, OUTPUT) y el pinmode(terminal7, OUTPUT), esto es que el 7 y el 8 esta como salida.

Después en seguida esta el void loop (es para crear un bucle), dentro de el está el digitalwrite(terminal7, HIGH) y el digitalwrite(terminal8, LOW), estos significa que un pin digital esta en alto (HIGH) y el otro en bajo (LOW) , y el delay(10) significa que al terminar los anteriores se espera 10 milisegundos y asi sigue la segunda parte pero cambiando el alto y el bajo de sitios(osea si en el anterios es 7 en lato y el 8 en bajo, en este caso es lo contrario, el 7 en bajo y el 8 en alto) y asi termina el programa.

# 2º Foto del circuito de pulsador.

<img src= "Imagenes/Fantastic Fulffy-Rottis.png" width="500" height="500" />

Este circuito su objetivo es al principio tiene que tener un diodo led encendido y cuando le das al pulsador enciende el que esta apagado y se apaga el que esta encendido y si sueltas el pulsador vuelve al principio de circuito.

# Foto de la programación de circuito.

<img src= "Imagenes/Captura de pantalla 2025-10-20 133800.png" width="500" height="500" />

Este programa enmpieza con cuatro variales que dos estan en terminales 7 y 8, uno es el pulsador y otro es su valor. 

Se sigue con un void setup, dentro suya tiene tres pinmode y un serial.begin, los tres pinmode tiene las dos terminales en outout(salida) y un pulsador en input(entrada), y el serial.begin(9600) es la velocidad que pasa desde el puerto USB a circuito. 

Después sigue con un void loop, dentro de el tiene el valor2= digitalRead(pulsador) (significa que el valor2 es igual que lee el pin digital de pulsador), después tiene dos if(comparación), en dentro de la primera tiene el valor que esta en alto, dos digitalWrite(escribir digitalmente) que uno dice que el terminal8 esta en bajo y el terminal 7 en alto, y un serial.println(pulsado) (significa que hace esto si esta pulsado) y asi inversamente.

# 3º Foto de potenciómetro.

<img src= "Imagenes/Smashing Amur.png" width="500" height="500" />

El objetivo de este programa es al cambiar el valor del potenciómetro la ilumidad del diodoled va cambia en que brilla más o menos.

# Foto de programación de circuito.

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/11d57d4d-09f8-4bce-93a5-29ee866e69ce" />

Este programación empieza con un variable int que dice que P2 = A2, después sigue con dos float(tipo de dato numérico que representa números de punto flotante o con decimales), uno que es el valor = 0, y el otro es el de ceroauno.

Después sigue con un void setup, dentro de el tiene un serial.begin(9600).

Después sigue con un void loop, que dentro de el tiene el valor = analogRead(P2) (significa que el valor que en este casa que es 0 es igual que lea el estado del pin 2), después tiene un serial.println(valor) (significa que el valor se envía al puerto serie) y por lo último un delay(20) (significa se retrasa 20 milisegundos) y asi termina la programa.

# 4º Foto de mapeado.

<img src= "Imagenes/IMG_8885.jpeg" width="500" height="500" />

El objetivo de este es parecido al potenciómetro solo que lo hacemos a mano de práctica que es de usar en este caso un tornillo y va cambiando el valor del potenciómetro y la ilumidad va cambiando o brilla más o brilla menos.

# Foto de prgramación de mapeado.

<img src= "Imagenes/Programación mapeado.png" width="500" height="500" />

Este programa enpieza con 4 variables int, uno es de LED5 = 5, el P2 = A2, uno que es lecturapotenciometro y otro de DutyCycle (en este caso es la luz del led.

Después sigue un void setup, que en dentro de el tenemos un pinMode(LED5, OUTPUT) (significa que el led 5 es en salida), y un serial.begin(9600).

Después sigue con un void loop, que dentro de el tenemos un lecturapotenciometro = analogRead(P2) (significa que el valor que tenga el potenciometro es igual a la lectura analógica de potenciómetro), después tenemos un DutyCycle = map(lecturapotenciometro, 16, 991, 0, 225) (esto significa que el valor de DutyCycle(variable) es igual que el mapeo(el mapeo es que dentro de ella se hace una regla de tres, se coge de 16 a 991 porque normalmente un potenciómetro puede llegar desde 0 a 1023 pero lo nuestro no llega y tiene un mínimo y un máximo que son estos números, después es el de 0 a 225 porque el diodoled que usamos tiene un mínimo de 0 y un máximo de 225 de valor), después sigue con un analogWrite(LED5, DutyCycle) (esto significa que está enviando una deñal al pin5 utilizando el DutyCycle que en este caso es el valor de mapeado), después tenemos un: Serial. print("lecturapotenciometro: "); Serial. print(lecturapotenciometro); Serial. print(" Dutycycle: "); Serial.print(Dutycycle) ,todo esto significa que tomamos los datos que nos han salido para que lo tengamos en cuenta. Y por último tenemos un delay(20) que es un tiempo de espera de 20 milisegundos y así termina este programa.

# 5º Foto de ultrasonido.

<img src= "Imagenes/IMG_8997.jpeg" width="500" height="500" />

<img src= "Imagenes/IMG_8996.jpeg" width="500" height="500" />

<img src= "Imagenes/IMG_8998.jpeg" width="500" height="500" />

El objetivo de este es que el ultrasonido va detectando la distancia, lo lee y cada vez que vayas cambiando la distancia, el valor que lee se cambia y saldrá otros valores.

# Foto de programación ultrasonido.

<img src= "Imagenes/ultrasonido.png" width="500" height="500" />

Este programa empieza en una una serie que dice que esta incuido el "Ultrasonic.h" (significa que todo el programación esta incluido el ultrasonido), después sigue con dos variables int que uno es TRIG_PIN=7 y el ECHO_PIN=8 (esto significa que el pin 7 está utilizando como el trigger y el pin 8 como el eco), después sigue con el Ultrasonic Tripitropi(TRIG_PIN, ECHO_ PIN, 60000) (esto significa que usamos un el ultrasonido de nombre como Tripitropi, junto con el trigger y el eco, que envian y reciben de un tiempo máximo de espera de 60000 microsegundos).

Después sigue con un void setup, dentro tiene un Serial.begin(9600), y dos Serial.println, el primero te dice que este programa es de Ultrasonic Distance Measerement y el otro te dice que este programa esta hecho por quien, y solo hacen eso en la programación, no hacen nada más.

Después sigue con un void loop, dentro tiene un Serial.print(Tripitropi.Ranging(CM)) (esto significa que lee la distancia y lo combierta en CM que en este caso es el variable Tripitropi), después sigue con un Serial.print("cm") (esto significa que lee el centímetros), y después tiene un delay(100), y se sigue haciendo lo mismo pero en INC (esto es en inches) y al final de programa tiene un delay(500) (todos son milisegundos, y así termina este programa.

# 6º Foto de control de iluminosidad con ultrasonido.

<img src= "Imagenes/IMG_0677.jpeg" width="500" height="500" />

<img src= "Imagenes/IMG_0678.jpeg" width="500" height="500" />

<img src= "Imagenes/IMG_0679.jpeg" width="500" height="500" />

<img src= "Imagenes/IMG_0680.jpeg" width="500" height="500" />

El objetivo de este circuito es que tiene un límite de distancia que es 225cm, si es dentro de esta distsncia, cuando más acerque iluminará más y cuando más lejos este iluminará menos, y si se pasa de 225 se apaga y no hace nada.

"NO TENGO VIDEO PORQUE TODO ESTABA BIEN PERO LA PLACA NO FUNCIONABA Y NO PUDÍ GRABARLO"

# Foto de programación.

<img src= "Imagenes/iluminacion.png" width="500" height="500" />

Este programa empieza diciendo que esta incuido el ultrasonido, después tiene 4 variables int, que uno es que te dice que el LED9 es igual a 10, otro te dice que el trigger esta en el 7, otro que dice que el eco esta en el 8 y el último es un variable que se llama Cantidadluz.

Después tenemos un void setup, dentro de el tenemos un Serial.print(9600) (milisegundos) y un pinMode LED9 OUTPUT, lo que hace es que al principio el led esta como salida.

Después tenemos un void loop, dentro tenemos que te dice que la camtidadlez es igual que la distancia que esta midiendo en CM, después tenemos dos if (comparación), en el primero tenemos que si 225 es más grande que la cantidadluz (osea si la distancia aue esta midiendo es mayor que 225), el led estará en bajo(osea apagado), después em el otro if, tenemos si es de 225 es menor o igual que cantidadluz, la iluminación del led es 225 menos la distancia que medirá y acabará con un delay(30) para tener un tiempo.

# 7º Foto de circuito de servomotor

| Foto 1 | Foto 2 | Foto 3 |
| - | - | - |
| <img src= "Imagenes/IMG_9513.jpeg" width="500" height="500" /> | <img src= "Imagenes/IMG_9514.jpeg" width="500" height="500" /> | <img src= "Imagenes/IMG_9515.jpeg" width="500" height="500" /> |

El objetivo de este circuito es que el motor iba girando por grados (primero esta en 00, despues gira hacia 90, después gira hacia 180 y vuelve otra vez a 00 y asi continuamente).

# Foto de programación.

<img src= "Imagenes/servomotor.png" width="500" height="500" />

Este circuito empieza diciendo aue esta incluido el Servo, y después dice que el nombre del Servo se llama serviMotor. También tiene dos variables int, que uno es cosnt int pinMotor = 5(significa que es constante la variable, no se puede cambiar) y otra variable int que se llama posicion.

Después tenemos un void setup, dentro de el tenemos un Serial.begin(9600) (milisegundos), un pinMode (pinMotor, OUTPUT) (significa aue el pinMotor esta en salida) y un servoMotor.attach(pinMotor) (significa que vinculan el servoMotor al pinMotor).

Después tenemos un void loop, dentro de el tenemos que primero tenemos la posicion en 00(significa que la posición esta en 0), un servoMotor.write(posicion) (significa que la escritura del servoMotor es la posicion), un Serial.println(posicion) (significa que la posicion se envía al puerto serie) y un delay(1000) (milisegundos), y así con los dos siguientes solo cambiando el valor de la posición y así termina este programa.

# 8º Foto de circuito de control de potenciómetro con servomotor.

| Foto 1 | Foto 2 | Foto 3 |
| - | - | - |
| <img src= "Imagenes/IMG_9513.jpeg" width="500" height="500" /> | <img src= "Imagenes/IMG_9514.jpeg" width="500" height="500" /> | <img src= "Imagenes/IMG_9515.jpeg" width="500" height="500" /> |

El objetivo de este circuito es que tiene conectado el potenciometro al motor, y al girar el potenciometro, el motor se gira hacia un lado o hacia otro.

# Foto de programación.

<img src= "Imagenes/programacion final proyecto.png" width="500" height="500" />

Este programa empieza diciendo que esta incluido el Servo, después dice que el nombre del Servo se llama servoMotor, después tiene un variable const int pinMotor = 5 (significa que es constante el variable), una variable int que dice que la posicion = 0, una variable int P3 = A3, y lecturapotenciometro = 0.

Después tenemos un void setup, dentro de el tenemos un Serial.begin(9600) (milisegundos), un pinMode (pinMotor, OUTPUT) (significa aue el pinMotor esta en salida) y un servoMotor.attach(pinMotor) (significa que vinculan el servoMotor al pinMotor).

Después tenemos un void loop, dentro de el tenemos que lecturapotenciometro = analogRead(P3) ((significa que el valor que tenga el potenciometro es igual a la lectura analógica de potenciómetro), después tenemos un posicion = map(lecturapotenciometro, 16, 991, 0, 180) (significa que el valor de posicion(variable) es igual que el mapeo(el mapeo es que dentro de ella se hace una regla de tres, se coge de 16 a 991 porque normalmente un potenciómetro puede llegar desde 0 a 1023 pero lo nuestro no llega y tiene un mínimo y un máximo que son estos números,después el 0 y el 180 porque nosotros tenemos el motor de grados desde 0 a 180)), un servoMotor.write(posicion) (significa que la escritura del servoMotor es la posicion) y un delay(20) milisegundos y así termina el programa.

# 9º Foto de circuito de control de ultrasonido con servomotor.

| Foto 1 | Foto 2 | Foto 3 |
| - | - | - |
| <img src= "Imagenes/IMG_0350.jpeg" width="500" height="500" /> | <img src= "Imagenes/IMG_0351.jpeg" width="500" height="500" /> | <img src= "Imagenes/IMG_0352.jpeg" width="500" height="500" /> |

El objetivo de este circuito es controlar la posición del servomotor mediante el ultrasonido que nos sirve para medir la distancia.

# Foto de programación.

<img src= "Imagenes/Tripitropi.png" width="500" height="500" />

Este programa empieza diciendo que contiene dos librerias, que uno es el de ultrasonic y otro de servo, despues te dice que el servo se va a llamar servoMotor, y a continuación tiene cinco variables, que uno tiene variable constante que te dice que pinmotor esta en el 5, uno que es posición es 0, uno que el TRIG esta en el 7, otro que el ECHO esta en el 8 y por lo último una de distancia, y al final tenemos que te dice que el ultrasonic se va a llamar Tripitropi, que dentro de el esta el trigger y el eco, que envian y reciben de un tiempo máximo de espera de 60000 microsegundos.

Después teneos un void setup, que dentro de el tenemos que el Serial.begin es de 9600 milisegundos, un pinMode que dice que el pinMotor al principio esta en salida y el servoMotor.attach que se vincula con el pinMotor.

Después tenemos un void lood, que dentro de el tenemos Serial.print(Tripitropi.Ranging(CM)) que te dice que lee la distancia y lo combierta en CM del variable Tripitropi, después dice que la distancia es el CM del variable Tripitropi, después la posición es el mapeado de la distancia de un mínimo de 2 y un máximo de 300 ( en el programa es 100 porque estabamos haciendo pruebas) y de 0 a 180, tiene una escritura de servoMotor que escribe la posición de lo que lee, que sirve para medir la distancia y un delay de 200 milisegundos y así termina el programa.









