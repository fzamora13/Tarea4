# Tarea4
Tarea 4 del curso Modelos probabilísticos de señales y sistemas de Fabián Zamora B57983

Parte I:
Para crear un esquema de modulación BPSK se debe saber que para cuando llegue un 1 se tendrá un valor positivo de la función seno y cuando llegue un 0 se tendrá un valor negativo de la función seno. 
El código se comienza con cualidades básicas de la onda portadora como la como frecuencia, periodo, número de muestreo y número de bits. Se observa la onda en la figura con el nombre correspondiente. La onda portadora se observa como una función seno de amplitud unitaria y con el periodo establecido.
Se establece la frecuencia de muestreo, la línea temporal de la señal modulada y su forma. Finalmente se crea la BPSK con un for que recorre todo el arreglo y con la forma matemática correcta de una BPSK. Se comprueba con una visualización para los primeros 50 bits. Es satisfactorio notar que los valores oscilan de la manera esperada para los 1's y 0's.

Parte II:
Se conoce la fórmula para la potencia promedio y se implementa. Se calcula la potencia promedio y se anota su valor en pantalla. Se obtiene que es de 0.2450 W. Se utiliza el comando de integrate.trapz.

Parte III:
Dada la SNR deseada de 3dB se crea la potencia correspondiente. A partir de ella se obtiene su desviación estándar que se utiliza para crear el ruido que se agrega a la señal "normal" o bien, sin ruido. Esta combinanción representa el canal para el cual luego se obtiene la visualización de los primeros 50 bits. Se comparan las figuras de la parte I y III y se observa como el ruido aumenta la amplitud y muestra más desorden y menos nitidez en la señal. 

Parte IV:
Se grafica con la herramienta "welch" la densidad espectral de potencia antes del canal y después del canal. Es muy interesante notar como la densidad es mayor (antes y después) en frecuencias bajas, lo cual es esperable ya que la frecuencia del sistema es de 5kHz. Más aún, la densidad de potencia tiene su pico alrededor de dicho punto. La densidad decae notablemente (antes y después) en frecuencias altas pero la energía permanece constante para después del canal. Se tiene entonces que antes del canal la energía va paulatinamente bajando pero con picos cada ciertas frecuencias y después del canal no se presentan picos sino un comportamiento casi que constante. 

Parte V:

Para esta sección se tomaron los primeros 50 bits, no todos los del arreglo. Se decodifica la señal y se obtiene el error y el BER para una tasa de error del 54%. 

Parte VI:

