# Estado del Arte
## Contexto científico
### Artículo 1
### Desarrollo de un sistema de adquisición de datos de campo para variables ambientales y de un sensor de viento, ambos de bajo costo y de arquitectura abierta
<p align="justify">
Esta iniciativa se centra en el inicio de la implementación de una estructura abierta orientada a la recopilación de datos ambientales. Asimismo, sienta las bases para explorar la posibilidad de utilizar sensores piezoeléctricos en la medición de la velocidad del viento en al menos una dirección. El estudio está desglosado en dos bloques principales, resaltando la interoperabilidad. Se evidencia que la implementación completa de este sistema puede lograrse a un costo considerablemente inferior en comparación con los sistemas convencionales empleados para medir la velocidad del viento, abriendo así nuevas perspectivas de investigación. El diseño propuesto es económico, presenta una capacidad de memoria destacada y capitaliza los avances en tecnología de memorias con conexión USB (Quesada-Kimsey et al., 2009).
</p>

<p align="center">
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/E04Imagen01.png" width="350" style="margin: auto;">
</p>

<p align="justify">
Se realizaron pruebas para evaluar la velocidad del viento mediante un mecanismo específico. Se ajustaron las velocidades del viento utilizando una secadora de pelo de 2 velocidades, ubicada a diversas distancias del sensor (50 cm, 75 cm, 110 cm y 150 cm). Se desactivó la función de calentamiento de la secadora para asegurar un flujo uniforme, a diferencia de los abanicos de computadora. Para obtener mediciones estándar de velocidad del viento, se empleó un anemómetro de cazoletas Thies Clima como punto de referencia. La digitalización de los datos se realizó mediante el datalogger CEC webDAQ/100. La información recopilada del medidor de velocidad del viento con cazoletas fue analizada mediante C#, el cual transformó la frecuencia a velocidades en m/s y km/h. (Quesada-Kimsey et al., 2009).
</p>

### Artículo 2
### Diseño IoT y validación de un sistema de medida para generación fotovoltaica
<p align="justify">
Este artículo analiza el aumento en el uso de sistemas fotovoltaicos (FV) en la generación de electricidad en Brasil. Este crecimiento se atribuye a la disminución de los costos de los módulos FV y a la introducción del sistema de compensación de energía eléctrica por parte de las empresas de suministro eléctrico. Este cambio ha motivado a los consumidores a invertir en microgeneración FV con el objetivo de reducir sus gastos de energía. El enfoque principal del texto se centra en el desarrollo de un sistema completo, en el contexto del Internet de las Cosas, para supervisar un sistema FV conectado a la red en una institución educativa.
</p>
<p align="justify">
La aplicación de este sistema IoT ofrece una solución educativa asequible y de código abierto, con hardware programable. Este sistema envía datos a una base que se encuentra ubicada en la nube, permitiendo el acceso remoto desde cualquier lugar. Los resultados obtenidos mediante la metodología de análisis de datos validaron con un error inferior al 1 % los valores medidos de tensión y corriente adquiridos durante un día, demostrando la eficacia del sistema IoT para la medición en sistemas FV, según lo indicado por Dos Santos y colaboradores en 2022. Este enfoque resalta no solo la eficiencia del sistema, sino también su capacidad para ofrecer una solución integral y accesible en el monitoreo de sistemas FV, especialmente en entornos educativos (Dos Santos et al., 2022).
</p>

<p align="center">
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/E04Imagen02.png" width="500" style="margin: auto;">
</p>

### Artículo 3
### A Neural Network Based Intelligent Predictive Sensor for Cloudiness, Solar Radiation and Air Temperature (Un sensor predictivo inteligente basado en una red neuronal para la nubosidad, la radiación solar y la temperatura del aire)

<p align="justify">
Este artículo presenta un sensor predictivo inteligente que utiliza redes neuronales avanzadas para medir y prever nubosidad, radiación solar y temperatura del aire, representando un hito en la monitorización climática. Empleando redes neuronales de última generación, el sensor analiza datos históricos y adapta su aprendizaje en tiempo real, permitiendo predicciones precisas en entornos dinámicos. Su capacidad para realizar predicciones multivariables, anticipando cambios simultáneos en varias variables climáticas, mejora significativamente la precisión global en comparación con sensores convencionales. La asombrosa optimización de la eficiencia operativa en entornos solares se logra anticipando cambios en la radiación solar, permitiendo ajustes precisos en la generación y almacenamiento de energía para maximizar el rendimiento.
</p>
<p align="justify">
La adaptabilidad a condiciones locales, respaldada por el entrenamiento con datos específicos de ubicación, garantiza pronósticos más precisos y relevantes para cada entorno. La interfaz de usuario intuitiva no solo simplifica la configuración y visualización de datos, sino que también democratiza el acceso al sensor, haciendo que profesionales de diversas disciplinas aprovechen sus beneficios, más allá de los expertos en inteligencia artificial. Además, la integración eficiente en sistemas de Internet de las Cosas (IoT) amplía su utilidad, facilitando la monitorización remota y la transmisión de datos en tiempo real, esencial para aplicaciones a gran escala y entornos distribuidos. La validación empírica respalda la eficacia del sensor, demostrando su precisión y fiabilidad mediante rigurosas pruebas en diversas condiciones climáticas, (Scopus 2012).
</p>

#### Ilustración de las funcionalidades requeridas del dispositivo
<p align="center">
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/E04Imagen03.png" width="500" style="margin: auto;">
</p>

## Contexto Comercial
## Productos
### Producto 1: Medidor de radiación solar Fluke IRR1-SOL<br>
**Creador:** Fluke corporation<br>

<p align="center">
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/E04Imagen04.png" width="400" style="margin: auto;">
</p>

<p align="justify">
El Fluke IRR1-SOL es un medidor de radiación, ha sido desarrollado con el propósito de simplificar el proceso de instalación, puesta en marcha y mantenimiento de sistemas fotovoltaicos a través de un único dispositivo fácil de manejar. Este instrumento portátil posibilita la medición de radiación solar, temperatura, inclinación y dirección de los paneles, cumpliendo con los estándares de la normativa IEC 62446-1. Gracias a su diseño compacto y robusto, acompañado de una pantalla LCD de alto contraste, su utilización se facilita en diversos entornos. Equipado con funciones como brújula integrada y sensor de inclinación, el IRR1-SOL permite medir y documentar de manera eficiente la orientación del techo, la instalación, así como el ángulo e inclinación de los paneles. Asimismo, puede emplearse para el diseño, supervisión y comparación del rendimiento de sistemas fotovoltaicos, asegurando que estos generen la potencia eléctrica prevista en relación con la radiación solar recibida.
</p>

Extraído de:<br>
https://www.fluke.com/es-pe/producto/comprobacion-electrica/herramientas-de-energia-solar/flk-irr1-sol#<br>
https://dam-assets.fluke.com/s3fs-public/flk-220224-200400-es-naam-RR1-Soi-irradiance-meter-ds-w_0.pdf?isQmPxDLBawuwtd21Lok8Xi0DWvXM9Dd

### Producto 2: Anemómetro digital portátil con sensor de temperatura AN200 EXTECH
<p align="center">
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/E04Imagen05.png" width="500" style="margin: auto;">
</p>

<p align="justify">
El AN200 de EXTECH destaca como un minitermoanemómetro excepcional con un enfoque especial en la medición del viento. Este dispositivo versátil no solo cuenta con un termómetro infrarrojo para medir la temperatura de superficies remotas hasta 500 °F (260 °C) con puntero láser, sino que también tiene la capacidad de mostrar simultáneamente el flujo de aire o la velocidad del viento junto con la temperatura ambiente. Sus características avanzadas incluyen la memorización de dimensiones de área configurables (ft² o m²) para mayor comodidad. Con una rueda de paleta de baja fricción y una precisión de velocidad del 3%, el AN200 proporciona mediciones precisas y fiables del viento. Viene completo con una batería de 9 voltios, funda protectora de goma y estuche, siendo una herramienta integral y práctica para profesionales que buscan un medidor de viento de alto rendimiento.
</p>

Extraído de:<br>
https://www.viaindustrial.com/manuales_pdf/anemometro-digital-portatil-con-sensor-de-temperatura-an200-extech-manual-espanol.pdf

### Producto 3: Medidor de energía solar SP505<br>
**Creador:** EXCTECH instruments<br>

<p align="justify">
El Extech SP505 se destaca como un dispositivo esencial para medir la potencia de la radiación solar y facilitar la determinación de la ubicación ideal para instalaciones solares. Su versatilidad abarca la evaluación de la eficacia de la película solar, la medición precisa de la radiación solar y la comprobación de ventanas con aislamiento solar. En la industria automotriz, este medidor de bolsillo también se emplea para verificar la intensidad de los faros. Su utilidad se extiende incluso a la industria de ventanas, donde los fabricantes y propietarios de viviendas en remodelación confían en él para evaluar la transmisión de radiación solar a través de diferentes espesores de vidrio y niveles de tinte. Además, el SP505 ayuda a encontrar el ángulo óptimo de incidencia para maximizar la eficiencia de paneles solares y calentadores de agua solares. El producto se entrega completamente probado y calibrado.
</p>

<p align="center">
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/E04Imagen06.png" width="550" style="margin: auto;">
</p>

Extraído de:<br>
https://www.finaltest.com.mx/v/vspfiles/assets/datasheet/SP505_UM.pdf<br>
https://www.comerciogc.com/intranet/assets/images/archivos/43-ficha-tecnica.pdf

## Patentes de Invención
### Patente 1
**ES2473640T3** - Dispositivo y método de seguimiento solar para concentración fotovoltaica de alta eficacia<br>
**Fecha de Publicación:** 07/07/2014<br>
**Número de Publicación:** 2473640<br>
**Inventor(es):** Hong Seokhoon, Kang Mun-Sig y Jang Byung-Seok<br>

https://patents.google.com/patent/ES2473640T3/es?q=(dispositivo+medidor+de+radiacion+solar)&oq=dispositivo+medidor+de+radiacion+solar&page=1

<p align="justify">
Este dispositivo innovador es esencialmente un panel solar inteligente que sigue la trayectoria del sol para maximizar la captación de energía solar. Imagina un panel solar especial con la capacidad de enfocar la luz solar en un punto específico utilizando una lente de Fresnel. Este panel cuenta con un "ojo" especial, un sensor de seguimiento solar, que detecta y sigue el punto focal de la luz concentrada. Además, para una eficiencia óptima, el sistema incorpora detectores de luz solar en diferentes lados del panel. Dos unidades de control ajustan la posición del panel: una basada en la luminosidad general medida por los detectores solares y la otra utilizando información detallada del punto focal de la luz concentrada. Para evitar pérdidas de luz solar valiosa, se emplean lentes estratégicamente colocadas. En resumen, este dispositivo asegura que los paneles solares estén constantemente orientados hacia el sol de la manera más eficiente posible, permitiendo una generación de energía solar óptima.
</p>

<p align="center">
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/E04Patente01.png" width="550" style="margin: auto;">
</p>

### Patente 2
**ES2389794B2** - Sistema y método de seguimiento de la radiación solar<br>
**Fecha de Publicación:** 31/10/2012<br>
**Número de Publicación:** 2389794<br>
**Inventor(es):** Paul Stavrou y David W. Catter<br>

https://patents.google.com/patent/ES2389794B2/es?q=(sensor+de+radiacion+solar)&oq=sensor+de+radiacion+solar 

<p align="justify">
Imagina un sistema solar inteligente con un marco diseñado para seguir la trayectoria del sol. Este marco incorpora fotosensores que captan la luz solar a través de una abertura estratégica. Un módulo de cálculo evalúa la diferencia entre los datos recopilados por los fotosensores, indicando así la posición del sol. Esta información es luego utilizada por un controlador para ajustar la orientación del marco, asegurando que los paneles solares estén constantemente optimizados para recibir la máxima cantidad de energía solar. En resumen, este sistema garantiza que los paneles estén siempre alineados de manera eficiente, maximizando la eficiencia en la captación de energía solar.
</p>

<p align="center">
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/E04Patente02.png" width="550" style="margin: auto;">
</p>

### Patente 3
**ES2431829T3** - Sistema sensor eólico que utiliza señales de aspas<br>
**Fecha de Publicación:** 28/11/2013<br>
**Número de Publicación:** 2431829<br>
**Inventor(es):** Fabio Bertolotti y Jens Carpintero<br>

https://patents.google.com/patent/ES2431829T3/es?q=(sensor+eolico)&oq=sensor+eolico&page=4

<p align="justify">
Sistema que utiliza al menos un sensor en una de las aspas de la turbina para medir una cantidad física que refleja una característica del campo de velocidad del viento. Esta información se procesa a través de una tabla que se ha construido previamente, asociando los valores de los componentes cíclicos y constantes de la señal del sensor con los valores correspondientes de la velocidad del viento bajo diversas condiciones.
</p>

<p align="justify">
La tabla resultante se utiliza como referencia para determinar, mediante unos medios de búsqueda, el valor de la característica del campo de velocidad del viento en tiempo real, considerando la condición actual del viento. En resumen, el sistema aprovecha la información recopilada previamente para estimar la velocidad del viento actual y, por ende, optimizar el rendimiento de la turbina eólica.
</p>

<p align="center">
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/E04Patente03.png" width="550" style="margin: auto;">
</p>

### Patente 4
**ES2553980T3** - Un sensor óptico de viento de turbina eólica<br>
**Fecha de Publicación:** 15/12/2015<br>
**Número de Publicación:** 2553980<br>
**Inventor:** Olessen y IB Svend<br>

https://patents.google.com/patent/ES2553980T3/es?q=(sensor+eolico)&oq=sensor+eolico&page=6

<p align="justify">
Se trata de un sensor óptico instalado en el rotor de una turbina eólica, compuesto por varias fuentes de luz colocadas angularmente en el rotor. Estas fuentes emiten haces de luz que atraviesan las palas del rotor con ángulos específicos. Dispositivos receptores de luz, también montados en el rotor, detectan destellos de luz provocados por partículas en el viento. Un controlador procesa estos destellos para calcular tiempos de tránsito de las partículas a través de los haces de luz, proporcionando así información sobre la velocidad y dirección del viento tanto en la dirección axial como en el plano de rotación del rotor. En resumen, el sensor utiliza la interacción de la luz con partículas en el viento para medir la velocidad y dirección del viento en diferentes direcciones.
</p>

<p align="center">
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/E04Patente04.png" width="550" style="margin: auto;">
</p>

## Lista de requerimientos
### Funcionales
<p align="center">
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/E04Imagen07.png" width="650" style="margin: auto;">
</p>

### No funcionales
<p align="center">
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/E04Imagen08.png" width="650" style="margin: auto;">
</p>

### Estrategias de solución
<p align="center">
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/E04Imagen09.png" width="650" style="margin: auto;">
</p>

---
## Bibliografía
Bertolotti, F., et al (2013). ES2431829T3 - Sistema sensor eólico que utiliza señales de aspas - Google Patents. https://patents.google.com/patent/ES2431829T3/es?q=(sensor+eolico)&oq=sensor+eolico&page=4<br>

Dos Santos, T. a. D., De Freitas, F. G., Gonçalves, D. L. C., & Jucá, S. C. S. (2022). Diseño IOT y validación de sistema de medida para generación fotovoltaica, 28, 44–52. http://scielo.senescyt.gob.ec/scielo.php?script=sci_arttext&pid=S1390-860X2022000200044<br>

Hong, S. et al., (2014) . ES2473640T3 - Dispositivo y método de seguimiento solar para concentración fotovoltaica de alta eficacia - Google Patents. https://patents.google.com/patent/ES2473640T3/es?q=(dispositivo+medidor+de+radiacion+solar)&oq=dispositivo+medidor+de+radiacion+solar&page=1<br>

Krulce, D. L., et al  (2020). ES2761579T3 - Sistemas y procedimientos para interacción de dispositivos en base a una mirada detectada - Google Patents. https://patents.google.com/patent/ES2761579T3/es?q=(dispositivo+de+ahorro+de+energ%C3%ADa)&oq=dispositivo+de+ahorro+de+energ%C3%ADa<br>

Olesen, I. S. (2015). ES2553980T3 - Un sensor óptico de viento de turbina eólica - Google Patents. https://patents.google.com/patent/ES2553980T3/es?q=(sensor+eolico)&oq=sensor+eolico&page=6<br>

Quesada-Kimsey, J. et al  (2009). Desarrollo de un sistema de adquisición de datos de campo para variables ambientales y de un sensor de viento, ambos de bajo costo y de arquitectura abierta. https://repositoriotec.tec.ac.cr/handle/2238/5776<br>

Scopus preview -  Scopus (2012)  - A Neural Network Based Intelligent Predictive Sensor for Cloudiness, Solar Radiation and Air Temperature. (n.d.). https://www.scopus.com/home.uri<br>

Stavrou, P., et al (2012). ES2389794B2 - Sistema y método de seguimiento de la radiación solar. - Google Patents. https://patents.google.com/patent/ES2389794B2/es?q=(sensor+de+radiacion+solar)&oq=sensor+de+radiacion+solar
