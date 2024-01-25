<p align="center" style="margin-top: 50px; margin-bottom: 50px; font-family: Arial, sans-serif;">
  <p align="center">
    <img src="https://semanadelcannabis.cayetano.edu.pe/assets/img/logo-upch.png" width="300" alt="Facultad de Ciencias e ingeniería logo">
  </p>  
  <h1 align="center" style="margin-top: 30px; margin-bottom: 0px;">Facultad de Ciencias e ingeniería “Alberto Cazorla Talleri”</h1>
</p>

<h2 align="center" style="font-family: Arial, sans-serif;">Taller 03: Internet de las Cosas (IoT)</h2>

<strong> Docentes:</strong>
- Mg Umbert Lewis De La Cruz
- Mg. Paulo Camilo Vela Antón 
- Mg. Moises Stevend Meza Rodriguez 
- Dr. Harry Anderson Rivera Tito 
- Ing. Juan Manuel Zuñiga Mamani  
- Ing. Renzo José Chan Ríos

<strong>Elaborado por:</strong>
- Amparo Marleny Vidaurre Juárez
- Edwin Junior Jara Bocanegra
- Antony Iván Mendoza Villar
- Josue Jhordan Poma Arrieta
- Aracely Nicoll Dueñas Condori
</p>

<hr style="border: 1px solid #ccc; margin-top: 50px; margin-bottom: 50px;">

## 1. Introducción
<p align="justify">
El IoT se refiere  a la interconexión de dispositivos físicos a través de internet, permitiéndoles recopilar y compartir datos. Esta red de dispositivos abarca desde electrodomésticos y vehículos hasta dispositivos médicos y equipos industriales. La IoT tiene el potencial de revolucionar la forma en que interactuamos con el mundo que nos rodea, al proporcionar una mayor eficiencia, comodidad y control. Estos datos pueden ser utilizados para automatizar procesos, tomar decisiones informadas, monitorear el rendimiento de los dispositivos y mejorar la eficiencia operativa en una amplia gama de aplicaciones.
</p>

## 2. Descripción de Internet de las cosas (IoT)

### Características y componentes del  Internet de las cosas  (IoT)
- **Dispositivos Conectados:** Estos son los componentes físicos que forman parte del IoT, como sensores, actuadores, cámaras, medidores, etc.
- **Conectividad:** Los dispositivos IoT se conectan a través de redes inalámbricas, como Wi-Fi, Bluetooth, etc.
- **Plataformas de Gestión de Datos:** Estas plataformas permiten la recopilación, almacenamiento y análisis de grandes volúmenes.
- **Seguridad:** Dado que los dispositivos IoT recopilan y transmiten datos sensibles, la seguridad es fundamental para proteger la integridad y la privacidad de la información.
- **Protocolos de Comunicación:** Estos son los estándares que permiten la comunicación entre los dispositivos IoT y los sistemas de gestión.

### Importancia del  IoT  como herramienta para recopilar y transmitir información.
<p align="justify">
El Internet de las Cosas (IoT) es crucial para recopilar y transmitir información de manera automatizada, permitiendo la toma de decisiones informadas, el monitoreo remoto, la optimización de procesos y la innovación de productos y servicios.
</p>

## 3. Materiales
- Arduino MKR WiFi 1010
- MKR ioT Carrier
- Cable Micro USB
- Pug-and-play cables 
- Batería

<p align="center">
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/FotoTaller30.jpg" width="300px">
</p>

## 4. Ensamblado de componentes
<p align="justify">
Este proyecto prescinde de sensores externos. La operación se logra al montar la placa Arduino MKR WIFI 1010 sobre la MKR IoT Carrier y conectarla a la computadora.
</p>

<div align="center"; style="display: flex; justify-content: space-between;">
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/FotoTaller31.jpg" width="300px"/>
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/FotoTaller32.jpg" width="300px"/>
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/FotoTaller33.jpg" width="300px"/>
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/FotoTaller34.jpg" width="300px"/>
</div>

## 5. Ejercicios
### Ejercicio 1: Ejecutar el código de la sección "CONOCE EL KIT"
<p align="justify">
Luego de copiar el código al editor online nos encontramos con el error técnico de conectarlo con nuestra placa. Para lo cual, se decidió usar la app arduino IDE para ejecutar el siguiente código:
</p>

```cpp
/*
  Explore IoT - Activity 01
 
  Read values from a temperature and humidity sensor
  and print it in Serial Monitor and on a colored display.
 
  This example uses the IoT carrier and the MKR WiFi 1010.
 
  Based on code by
  (c) 2019 D. Cuartielles for Arduino
 
  Written by:
  (c) 2020 K. SÃ¶derby for Arduino
 
  This code is Free Software licensed under GPLv3
*/
 
#include <Arduino_MKRIoTCarrier.h>
MKRIoTCarrier carrier;
 
float temperature = 0;
float humidity = 0;
 
void setup() {
  Serial.begin(9600);
  //Wait to open the Serial monitor to start the program and see details on errors
  
 
  //Set if it has the Enclosure mounted
  CARRIER_CASE = false;
  //Initialize the IoTSK carrier and output any errors in the serial monitor
  carrier.begin();
}
 
void loop() {
  // read the sensor values
  temperature = carrier.Env.readTemperature();
  humidity = carrier.Env.readHumidity();
 
  //Update touch buttons
  carrier.Buttons.update();
 
  // print each of the sensor values
  Serial.print("Temperature = ");
  Serial.print(temperature);
  Serial.println(" Â°C");
 
  Serial.print("Humidity = ");
  Serial.print(humidity);
  Serial.println(" %");
 
  //function to print out values
  if (carrier.Buttons.onTouchDown(TOUCH0)) {
    printTemperature();
  }
 
  if (carrier.Buttons.onTouchDown(TOUCH1)) {
    printHumidity();
  }
}
 
 
void printTemperature() {
  //configuring display, setting background color, text size and text color
  carrier.display.fillScreen(ST77XX_RED); //red background
  carrier.display.setTextColor(ST77XX_WHITE); //white text
  carrier.display.setTextSize(6); //large sized text
 
  carrier.display.setCursor(30, 50); //sets position for printing (x and y)
  carrier.display.print("Temp: ");
  carrier.display.setTextSize(4); //decreasing text size
  carrier.display.setCursor(40, 120); //sets new position for printing (x and y)
  carrier.display.print(temperature);
  carrier.display.print(" C");
}
 
void printHumidity() {
  //configuring display, setting background color, text size and text color
  carrier.display.fillScreen(ST77XX_BLUE); //red background
  carrier.display.setTextColor(ST77XX_WHITE); //white text
  carrier.display.setTextSize(2); //medium sized text
 
  carrier.display.setCursor(20, 110); //sets position for printing (x and y)
  carrier.display.print("Humi: ");
  carrier.display.print(humidity);
  carrier.display.println(" %");
}
```

**Explicación de código**
<p align="justify">
- Se ha hecho uso de la librería Arduino MADRId Carrier: 
<code> #incluir <Arduino_MKRIoTCarrier.h> </code>
- La variable <code>CARRIER_CASE</code> debe estar como <code> TRUE</code>, porque estamos usando la caja de plástico.
<code> CARRIER_CASE = true; </code>
- Los botones táctiles <code>printTemperature(); y printHumidity(); </code> nos permite hacer el cambio de pantalla para mostrar los valores de la temperatura y humedad respectivamente.
</p>

```cpp
  if (carrier.Buttons.onTouchDown(TOUCH0)) {
    printTemperature();
  }
 
  if (carrier.Buttons.onTouchDown(TOUCH1)) {
    printHumidity();
  }
```

<p align="justify">
- Para el funcionamiento correcto del anterior segmento de código se hizo lo siguiente dentro de cada función, donde podemos cambiar el color de la pantalla, el tamaño de letra, la ubicación del cursor para el texto y el color de letra:
</p>

```cpp
void printTemperature() {
  //configuring display, setting background color, text size and text color
  carrier.display.fillScreen(ST77XX_RED); //red background
  carrier.display.setTextColor(ST77XX_WHITE); //white text
  carrier.display.setTextSize(6); //large sized text
 
  carrier.display.setCursor(30, 50); //sets position for printing (x and y)
  carrier.display.print("Temp: ");
  carrier.display.setTextSize(4); //decreasing text size
  carrier.display.setCursor(40, 120); //sets new position for printing (x and y)
  carrier.display.print(temperature);
  carrier.display.print(" C");
}
```

<p align="justify">
El código fue ejecutado con éxito y a continuación se evidencia el correcto funcionamiento de está actividad, donde muestra valores reales de la temperatura y la humedad del laboratorio de prototipado.
</p>

<div align="center"; style="display: flex; justify-content: space-between;">
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/FotoTaller35.jpg" width="300px"/>
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/FotoTaller36.jpg" width="300px"/>
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/FotoTaller37.jpg" width="300px"/>
</div>

### Ejercicio 2: Implementar código para cambiar datos de la temperatura en las escalas convencionales
<p align="justify">
Para lograr este desafío nos ayudamos de las fórmulas físicas revisadas en google, obteniendo lo siguiente:
</p>

```cpp
void printTemperature() {
  //configuring display, setting background color, text size and text color
  carrier.display.fillScreen(ST77XX_RED); //red background
  carrier.display.setTextColor(ST77XX_WHITE); //white text
  carrier.display.setTextSize(6); //large sized text
 
  carrier.display.setCursor(30, 50); //sets position for printing (x and y)
  carrier.display.print("Temp: ");
  carrier.display.setTextSize(4); //decreasing text size
  carrier.display.setCursor(40, 120); //sets new position for printing (x and y)
  carrier.display.print(temperature);
  carrier.display.print(" C");
}
```

**Explicación de las partes añadidas en el código:**
<p align="justify">
Dentro del <code> void loop() </code>  se llamaron a las funciones creadas para mostrar las diferentes escalas de temperatura. Esto con el fin de realizar la misma secuencia usada anteriormente para actualizar la lectura y ver los diferentes tipos de datos con los botones táctiles del MKR IoT carrier, es decir, se hizo uso de los <code> TOUCH1 TOUCH2  TOUCH3 </code>.
</p>

```cpp
void printTemperature() {
  //configuring display, setting background color, text size and text color
  carrier.display.fillScreen(ST77XX_RED); //red background
  carrier.display.setTextColor(ST77XX_WHITE); //white text
  carrier.display.setTextSize(6); //large sized text
 
  carrier.display.setCursor(30, 50); //sets position for printing (x and y)
  carrier.display.print("Temp: ");
  carrier.display.setTextSize(4); //decreasing text size
  carrier.display.setCursor(40, 120); //sets new position for printing (x and y)
  carrier.display.print(temperature);
  carrier.display.print(" C");
}
```

<p align="justify">
Los códigos usados en las funciones  <code> printTemperatureF() y printTemperatureK() </code> se ha reutilizado de la función <code> printTemperature() </code> . Pero con el único cambio en que se imprime la nueva variable asignada a su respectiva conversión de escala.
</p>

```cpp
void printTemperature() {
  //configuring display, setting background color, text size and text color
  carrier.display.fillScreen(ST77XX_RED); //red background
  carrier.display.setTextColor(ST77XX_WHITE); //white text
  carrier.display.setTextSize(6); //large sized text
 
  carrier.display.setCursor(30, 50); //sets position for printing (x and y)
  carrier.display.print("Temp: ");
  carrier.display.setTextSize(4); //decreasing text size
  carrier.display.setCursor(40, 120); //sets new position for printing (x and y)
  carrier.display.print(temperature);
  carrier.display.print(" C");
}
```

<div align="center"; style="display: flex; justify-content: space-between;">
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/FotoTaller38.jpg" width="300px"/>
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/FotoTaller39.jpg" width="300px"/>
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/FotoTaller40.jpg" width="300px"/>
</div>

**Ejercicio 3: Implementar código para centrar  y aumentar el tamaño de las letras de la Humedad**
<p align="justify">
Para esta parte tan solo modificamos los valores del tamaño del texto en la pantalla y donde debería de estar el curso al mostrar cada texto en su respectiva lectura.
</p>

```cpp
void printTemperature() {
  //configuring display, setting background color, text size and text color
  carrier.display.fillScreen(ST77XX_RED); //red background
  carrier.display.setTextColor(ST77XX_WHITE); //white text
  carrier.display.setTextSize(6); //large sized text
 
  carrier.display.setCursor(30, 50); //sets position for printing (x and y)
  carrier.display.print("Temp: ");
  carrier.display.setTextSize(4); //decreasing text size
  carrier.display.setCursor(40, 120); //sets new position for printing (x and y)
  carrier.display.print(temperature);
  carrier.display.print(" C");
}
```

<div align="center"; style="display: flex; justify-content: space-between;">
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/FotoTaller41.jpg" width="300px"/>
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/FotoTaller42.jpg" width="300px"/>
</div>

### Ejercicio 4: Cambio en el nivel de temperatura ( Temperatura del laboratorio = Rojo, Temperatura del aire acondicionado = Azul)

<div align="center"; style="display: flex; justify-content: space-between;">
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/FotoTaller43.jpg" width="300px"/>
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/FotoTaller44.jpg" width="300px"/>
</div>

## 6. Observaciones
<p align="justify">
En cuanto al uso de pilas en los dispositivos IoT, es cierto que muchos de ellos utilizan pilas como fuente de energía. Esto se debe principalmente a que los dispositivos IoT suelen ser pequeños y diseñados para ser autónomos, lo que significa que no siempre tienen acceso a una fuente de alimentación externa, como una toma de corriente. Por lo tanto, las pilas son 
una opción conveniente y práctica para alimentar estos dispositivos. En todos los ejercicios realizados anteriormente se confirmó ello, ya que al colocar una pila al dispositivo ioT, lo hizo más práctico al momento de utilizarlo.
</p>

## 7. Evidencias del desarrollo de ejercicios

<div align="center"; style="display: flex; justify-content: space-between;">
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/FotoTaller48.jpg" width="250px"/>
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/FotoGrupal06.jpg" width="400px"/>
</div>

## 8. Conclusiones

<p align="justify">
El Internet de las Cosas (IoT) ofrece un potencial significativo para la interconexión y el control de dispositivos físicos a través de Internet. Además, la capacidad de convertir temperaturas entre diferentes escalas a medida que se adapta , ajustar el formato de la humedad y crear un sensor de proximidad que el sensor presienta el movimiento  y prenda luces de colores verdes. Asimismo , se vio que la capacidad de reconocer la temperatura y cambiar el color del indicando que a temperatura ambiente sea de color  rojo  y cuando le acercamos al aire acondicionado sea de color azul. Esta interconexión brinda la posibilidad de controlar y monitorear dispositivos de manera remota, lo que conduce a beneficios significativos en términos de automatización, eficiencia y comodidad.
</p>
