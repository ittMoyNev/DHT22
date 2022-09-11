# DHT22
Exposiciones de los sensores del Simulador - DHT22

# ¿Qué es el DHT22?
El DHT22 es un sensor de temperatura y humedad con unas prestaciones que lo acercan mucho a los de alta precisión. Lo puedes encontrar fácilmente en tiendas especializadas o grandes superficies. Eso te permite no tener que depender de un sensor de temperatura y otro de humedad por separado, sino tenerlo todo integrado en un mismo dispositivo.

[![dht22.jpg](https://i.postimg.cc/SRVDkYyd/dht22.jpg)](https://postimg.cc/XBGwgJBB)

Lo puedes encontrar suelto o en módulos especialmente diseñados para Arduino, es decir, el DHT22 montado sobre una placa PCB ya lista para usar, sin tener que agregar resistencias pull-up, etc. Hasta aquí todo se parece bastante el DHT11. Y también tendrás una alta fiabilidad y estabilidad en las mediciones debido a la señal digital calibrada que usa.

# Pinout, características y datasheet
En la imagen anterior puedes ver una comparación del pinout del DHT22 y DHT11, y como puedes apreciar son idénticos en cuanto a patillas. Por eso, su montaje sería exactamente igual, y lo mejor, podrías sustituir en cualquier momento el DHT11 por un DHT22, y viceversa, en tu proyecto sin hacer demasiados cambios.

Recuerda que tienen 3 pines que debes usar: GND, Vcc y Datos. El pin #3 no se usa y en los módulos viene anulado, es decir, solo verás tres pines. Si quieres ver más detalles sobre el producto que has adquirido, puedes buscar los datasheets del modelo y fabricante concreto para obtener toda la información completa. Aunque la mayor parte de valores pueda parecerte igual, podría haber alguna pequeña variación de uno a otro. Sus características técnicas más importantes son:

    -Alimentación de 3,3v a 6v
    -Consumo de corriente de 2,5mA
    -Señal de salida digital
    -Rango de temperatura de -40ºC a 125ºC
    -Precisión para medir temperatura a 25ºC de 0.5ºC de variación
    -La resolución para medir temperatura es de 8-bit, 0,1ºC
    -La humedad puede medir desde 0% RH hasta los 100% RH
    -Con precisión para la humedad del 2-5% RH para temperaturas que se encuentren entre 0-50ºC
    -La resolución es de 0,1% RH, no puede captar variaciones por debajo de esa
    -Frecuencia de muestreo de 2 muestras por segundo: 2Hz
    -Datasheet de Sparkfun
Si has leído nuestro manual sobre el DHT11 sabrás que transmite en digital por su pin Data, por tanto, otra ventaja para estos sensores. No habrá que generar código en Arduino IDE para pasar de analógico a valores comprensibles para el humano, sino que se puede tratar directamente la señal digital para pasarla a grados o porcentaje de humedad relativa.

En parte, por eso también es tan preciso, ya que con la trama de 40-bits que transmite, la precisión es más elevada. Incluso incluye unos bits de paridad para detectar fallos en la señal. Eso con una señal analógica no lo tienes, a parte de que la analógica es muy sensible a las variaciones de voltaje…
[![pinout-dht11.jpg](https://i.postimg.cc/DwCkBmLq/pinout-dht11.jpg)](https://postimg.cc/5XFRt4P0)

# Especificaciones tecnicas
    -Voltaje de Operación: 3V - 6V DC
    -Rango de medición de temperatura: -40°C a 80 °C
    -Precisión de medición de temperatura: <±0.5 °C
    -Resolución Temperatura: 0.1°C
    -Rango de medición de humedad: De 0 a 100% RH
    -Precisión de medición de humedad: 2% RH
    -Resolución Humedad: 0.1%RH
    -Tiempo de sensado: 2s
    -Interface digital: Single-bus (bidireccional)
    -Modelo: AM2302
    -Dimensiones: 20*15*8 mm
    -Peso: 3 gr.
    -Carcasa de plástico blanco
    
# Referencias
https://naylampmechatronics.com/sensores-temperatura-y-humedad/58-sensor-de-temperatura-y-humedad-relativa-dht22-am2302.html
https://www.geekfactory.mx/tienda/sensores/dht22-sensor-de-temperatura-y-humedad-relativa/
https://www.hwlibre.com/dht22/




