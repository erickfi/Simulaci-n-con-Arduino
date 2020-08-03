## UNIVERSIDAD DE LAS FUERZAS ARMADAS ESPE
![](https://github.com/erickfi/Practica-5/blob/master/Img/Escudo.jpg)
### Práctica de laboratorio N° 6
## Teorema de la Máxima Transferencia de Potencia
**Autores:** Figueroa Erick, León Jipshon,Viracucha William.
### 1. PLANTEAMIENTO DEL PROBLEMA
Al momento de diseñar un circuito eléctrico, por lo general, se busca que el circuito cumpla su trabajo, es decir, que los elementos electrónicos del mismo realicen el trabajo, pero no se toma en cuenta la eficacia para realizar este trabajo, recordando que la potencia representa la tasa de la energía que se convierte en trabajo, existen circuitos que buscan precisamente este objetivo, entregar la máxima potencia de tal forma que el trabajo se realice de ser posible sin pérdida de energía.

Por otro lado, para conocer la potencia que entrega un circuito es necesario analizar todos los componentes del mismo, aunque este proceso se puede simplificar si usamos el [Teorema de Thévenin](https://github.com/erickfi/Practica-5), de esta forma simplificamos el circuito y obtenemos un circuito simplificado para carga variable, su aplicación en la ingeniería es fundamental, ya que es importante en los procesos de automatización donde se busca que las máquinas funcionen a su máxima capacidad, es decir, que tengan una máxima potencia.


### 2. OBJETIVOS
#### Objetivo General
- Comprobar experimentalmente el Teorema de la Máxima Transferencia
#### Objetivos Específicos
- Calcular y comparar los valores de potencia en un circuito de dos terminales de forma analítica y experimental.
- Demostrar de manera experimental que si RL es diferente de RTh el circuito no alcanzará la potencia máxima.
- Analizar y determinar el menor error porcentual posible
### 3. MARCO TEÓRICO
El **Teorema de la Máxima Transferencia de Potencia** estable:
> "La máxima potencia se transfiere a la carga cuando la resistencia de la carga es igual a la resistencia de Thévenin vista desde la carga (RL=RTh).Sadiku(2006)

Es por esto que la forma más fácil de analizar la potencia suministrada a una carga es simplificando un circuito de dos terminales a un circuito de Thévenin.

![](https://github.com/erickfi/Practica-5/blob/master/Img/Cambio%20circuito.PNG)

Si graficamos la potencia suministrada en función de la variación de la carga obtenemos un gráfica similar a una campana de Gauss.

![](https://github.com/erickfi/Laboratorio-6/blob/master/Img/Grafica.PNG)

En la cuál podemos observar que el punto más alto de transferencia es alcanzado cuando RL=RTh, si esto ocurre la potencia máxima se puede calcular como:

![](https://github.com/erickfi/Laboratorio-6/blob/master/Img/Con%20RTH.PNG)

Sin embargo, en los circuitos que se realizan en la vida real es poco probable que esto sucede, por lo general la resistencia que presenta la carga (RL) es diferente a la resistencia de la fuente (RTh), es por ello que para calcular la potencia se utiliza:

![](https://github.com/erickfi/Laboratorio-6/blob/master/Img/Con%20RL.PNG)

Ya que RL y RTh no son iguales no se puede alcanzar una _transferencia máxima de potencial ideal,_ pero este valor se puede aproximar variando la resistencia de la carga hasta que sea similar a la resistencia de la fuente pero sin que el funcionamiento del resto de elementos del circuito se vea afectado.


### 4. DIAGRAMAS
**Diagrama del circuito**

![](https://github.com/erickfi/Laboratorio-6/blob/master/Img/Diagrama.PNG)

**Medición de valores**

![](https://github.com/erickfi/Laboratorio-6/blob/master/Img/Thinker%206.1.PNG)
![](https://github.com/erickfi/Laboratorio-6/blob/master/Img/Thinker%206.2.PNG)
![](https://github.com/erickfi/Laboratorio-6/blob/master/Img/Thinker%206.3.PNG)

### 5. LISTA DE COMPONENTES

![](https://github.com/erickfi/Laboratorio-6/blob/master/Img/Materiales.PNG)

### 6. TABLA DE RESULTADOS

***Tabla 1. Parámetros eléctricos del circuito***

|   RL (Ω)  | Corriente  |   Voltaje  | Potencia calculada | Potencia calculada | Error |
|:---------:|:----------:|:----------:|:------------------:|:------------------:|:-----:| 
|           |  Medida    |   medido   | Experimentalmente  | teóricamente       |       |
|           |   (mA)     |    (V)     |       (mW)         |        (mW)        |  (%)  |
|   220     |   10.6     |   2.32     | 24.592             | 24.548             | 0.18  |
|   470     |   8.98     |   4.22     | 37.895             | 37.918             | 0.06  |
|   680     |   7.98     |   5.43     | 43.311             | 43.288             | 0.1   |
|   820     |   7.43     |   6.09     | 45.248             | 45.216             | 0.07  |
|   1000    |   6.82     |   6.82     | 46.512             | 46.487             | 0.05  |
|   1500    |   5.56     |   8.33     | 46.314             | 46.296             | 0.04  |
|   1800    |   5        |   9        | 45                 | 45                 | 0     |
|   2200    |   4.41     |   9.71     | 42.821             | 42.82              | 0.002 |
|   3900    |   2.94     |   11.5     | 33.81              | 33.737             | 0.216 |
|   4700    |   2.54     |   11.9     | 30.226             | 30.379             | 0.5   |



### 7. Explicación de Código Fuente

- 1. Armar el circuito tal como se muestra en el diagrama.
- 2. Medir la corriente y voltaje de la resistencia de carga para cada valor que adquiere esta resistencia mediante un multímetro, específicamente se debe realizar las mediciones para 220 Ω, 470 Ω, 680 Ω, 820 Ω, 1000 Ω, 1500 Ω, 1800 Ω, 2200 Ω, 3900 Ω, 4700 Ω. En total son 10 mediciones de voltaje y 10 mediciones de corriente.

### 8. CONCLUSIONES

- Una fuente de voltaje entrega la máxima transferencia de potencia cuando necesariamente su resistencia interna es igual a la resistencia de la carga, en este caso la resistencia de Thévenin debe ser obligadamente el mismo valor de la resistencia de la carga.
- Las resistencias mas próximas a 1200 Ohmios como la de 1000 y 1500, entregan una potencia casi próxima a la potencia máxima, entonces podemos decir que entre mas cercano sea el valor de la resistencia interna, al valor de la resistencia de carga, la potencia tiende a su valor máximo, pero no la van a superar.
- Para que la potencia sea máxima P= 46.875 mW, la resistencia de la carga RL debe ser igual a la de la fuente RTh, por lo tanto, RL= RTh= 1200 Ω.
- Se cumple el Teorema de la Máxima Transferencia de Potencia, al observar que la potencia suministrada por todas las resistencias utilizadas es menor a la cálculada si RL=1200 Ω.
- Dentro de las resistencias utilizadas se obtiene que la resistencia de 1000 Ω, es la que más se aproxima al valor de la potencia máxima, la cuál entrega una potencia de 46.487 mW.

### 9. RECOMENDACIONES

- Una forma de comprobar el teorema de máxima transferencia de potencia es dar valores a la resistencia de carga muy cercanos a la resistencia interna, y observar que la potencia va a estar al limite de la potencia máxima

### 10. CRONOGRAMA

![](https://github.com/erickfi/Laboratorio-6/blob/master/Img/Cronograma%206.PNG)

### 11. REFERENCIAS
- [1] M. A. Sadiku.Fundamentos de circuitos eléctricos. Mc Graw Hill, third edition, 2006
### 12. ANEXOS
- [Cálculos análiticos](https://github.com/erickfi/Laboratorio-6/blob/master/Anexos/Anexos%20lab%206.pdf)
- [Cómo funciona el circuito](https://www.youtube.com/watch?v=pdyatt-rUAg&feature=youtu.be)
- [Cómo se implementó el circuito](https://www.youtube.com/watch?v=wW0A3P_5MHM&feature=youtu.be)
