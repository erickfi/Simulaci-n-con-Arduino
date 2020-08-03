## UNIVERSIDAD DE LAS FUERZAS ARMADAS ESPE
![](https://github.com/erickfi/Practica-5/blob/master/Img/Escudo.jpg)
### Simulación con Arduino
**Autor:** Figueroa Erick.

### ¿Qué es Arduino?

![](https://github.com/erickfi/Simulaci-n-con-Arduino/blob/master/Imgs/Arduino.PNG)

En la actualidad la tecnología está presente de forma más significativa en nuestro diario vivir, desde sus inicios su objetivo ha sido mejorar la calidad de vida de las personas, actualmente gracias al desarrollo tecnológico podemos comunicarnos grandes distancias en cuestión de segundos y en tiempo real, e incluso poder controlar nuestro hogar desde nuestro celular, esto se debe al uso e instalación de componentes electrónicos, lo cuáles están presentes en todo nuestro alrededor.

Uno de los componentes más utilizados, de fácil control y operación es el [Arduino](https://www.arduino.cc/), que podemos llamarlo el punto de partida en el inicio de la automatización de control de un sistema con componentes electrónicos y/o mecánicos, una de sus principales aplicaciones es el control de las luces de los semáforos, no obstante, no es la única que existe.

Para las personas que empiezan a involucrarse en el mundo de la electrónica y el control, usar el Arduino se convierte en una herramienta indispensable, existen varias definiciones o interpretaciones al momento de referirnos a que es Arduino, sin embargo, la más conocida y aceptada es:

> El arduino es una placa que tiene todos los elementos necesarios para conectar periféricos a las entradas y salidas de un microcontrolador. Es decir, es una placa impresa con los componentes necesarios para que funcione el microcontrolador y su comunicación con un ordenador a través de la comunicación serial.

### Objetivos
- Comprender qué es y como funciona un Arduino.
- Realizar simulaciones de procesos usando un Arduino como controlador del proceso.

### ¿Cómo funciona Arduino?
Anteriormente se habia asociado al arduino con los microcontroladores por lo que su funcionamiento va a ser similar.
- **Cuenta con una interfaz de entrada.** Esta puede estar directamente unida a los periféricos , o conectarse a ellos a través de puertos.
- **La interfaz de entrada** Tiene como objetivo trasladar la información al microcontrolador.
- **El microcontrolador** Es la pieza que se encarga de procesar esos datos. Además, varía dependiendo de las necesidades del proyecto en el que se desee usar la placa, y existe una gran variedad de fabricantes y versiones disponibles.
- **Interfaz de salida.** Este se encarga de llevar la información procesada a los periféricos autorizados de hacer el uso final de esos datos. En algunos casos puede tratarse de otra placa en la que se centraliza y procesa la información de forma totalmente renovada, o sencillamente, puede ser una pantalla o un altavoz encargado de mostrar la versión final de los datos.

Al permitir realizar diferentes controles gracias a su variada gama de componentes, para realizar un proceso en específico se debe programar en lenguaje C.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## PROGRAMACIÓN DE MÓDULOS LED RGB
Una de las prácticas más comunes al comenzar a usar arduino como microcontrolador de sistemas con componentes electrónicos es el control de luces, ya sea por períodods de tiempo o variación de funciones, a continuación de presenta una guía de como realizar el control, esto se realizará usando un sotfware de simulación, para evitar adentrarse en las especificaciones técnicas de programación en un determinado lenguaje.

### Componentes
Para realizar la práctica se requieren diversos componentes en caso de que quiera realizarlo usando elementos físicos.
- Un arduino o una placa compatible con arduino.
- Un [módulo LED RGB](https://www.iberobotics.com/producto/modulo-led-rgb/).
- 4 Cables de puente hembra-hembra, de preferencia naranja, rojo, azul y verde.
- Para la simulación se ha usado el programa [visuino o visualino](http://visuino.com/).

### Conectar el módulo LED.

![](https://github.com/erickfi/Simulaci-n-con-Arduino/blob/master/Imgs/modulo%20led.PNG)

Para observar paso a paso como conectar el módulo led al arduino, en se siguiente [video](https://www.youtube.com/watch?time_continue=10&v=QC-8zglK8GA&feature=emb_logo) se explica el preoceso.

### Programa con visuino
Al iniciar el programa, en la opción de ***herramientas*** del arduino, seleccionar el tipo de Arduino a utilizar.

![](https://github.com/erickfi/Simulaci-n-con-Arduino/blob/master/Imgs/visuino%20img%201.PNG)

#### 1. Configuración de componentes del generador analógico sinusoidal.
Vamos a realizar el control de 3 diferentes colores de luces, rojo, azul y verde en el led, para ello se usa generadores analógicos sinusoidales, los cuáles para obtener el efecto esperado deberán variar su frecuencia.

**1.1** En el buscador del programa escriba ***sine*** y seleccione la opción ***SineAnalogGenerator*** y arrastre 3 a la pantalla de trabajo.

![](https://github.com/erickfi/Simulaci-n-con-Arduino/blob/master/Imgs/generadores%20anal%C3%B3gicos.PNG)

Al seleccionar los generadores analógicos procedemos a variar su frecuencia, 0.3 y 0.1 para el ***SineAnalogGenerator2*** y ***SineAnalogGenerator3*** respectivamente.

**1.2** Conecte los componentes al simulador del arduino.
- El pin **Out** de los ***SineAnalogGenerator 1, 2 y 3*** al ping de entrada ***Analog*** de los ***canales digitales 3, 5 y 6*** respectivamente.

![](https://github.com/erickfi/Simulaci-n-con-Arduino/blob/master/Imgs/conexion%201.PNG)

### 5. LISTA DE COMPONENTES



### 6. TABLA DE RESULTADOS



### 7. Explicación de Código Fuente



### 8. CONCLUSIONES



### 9. RECOMENDACIONES


### 11. REFERENCIAS
### 12. ANEXOS
