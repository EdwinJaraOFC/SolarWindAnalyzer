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
**Producto 1:** Medidor de radiación solar Fluke IRR1-SOL
**Creador:** Fluke corporation

<p align="center">
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/E04Imagen04.png" width="350" style="margin: auto;">
</p>

<p align="justify">
El Fluke IRR1-SOL es un medidor de radiación, ha sido desarrollado con el propósito de simplificar el proceso de instalación, puesta en marcha y mantenimiento de sistemas fotovoltaicos a través de un único dispositivo fácil de manejar. Este instrumento portátil posibilita la medición de radiación solar, temperatura, inclinación y dirección de los paneles, cumpliendo con los estándares de la normativa IEC 62446-1. Gracias a su diseño compacto y robusto, acompañado de una pantalla LCD de alto contraste, su utilización se facilita en diversos entornos. Equipado con funciones como brújula integrada y sensor de inclinación, el IRR1-SOL permite medir y documentar de manera eficiente la orientación del techo, la instalación, así como el ángulo e inclinación de los paneles. Asimismo, puede emplearse para el diseño, supervisión y comparación del rendimiento de sistemas fotovoltaicos, asegurando que estos generen la potencia eléctrica prevista en relación con la radiación solar recibida.
</p>

Extraído de:
https://www.fluke.com/es-pe/producto/comprobacion-electrica/herramientas-de-energia-solar/flk-irr1-sol#
https://dam-assets.fluke.com/s3fs-public/flk-220224-200400-es-naam-RR1-Soi-irradiance-meter-ds-w_0.pdf?isQmPxDLBawuwtd21Lok8Xi0DWvXM9Dd

**Producto 2:** Anemómetro digital portátil con sensor de temperatura AN200 EXTECH
<p align="center">
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/E04Imagen05.png" width="350" style="margin: auto;">
</p>

<p align="justify">
El AN200 de EXTECH destaca como un minitermoanemómetro excepcional con un enfoque especial en la medición del viento. Este dispositivo versátil no solo cuenta con un termómetro infrarrojo para medir la temperatura de superficies remotas hasta 500 °F (260 °C) con puntero láser, sino que también tiene la capacidad de mostrar simultáneamente el flujo de aire o la velocidad del viento junto con la temperatura ambiente. Sus características avanzadas incluyen la memorización de dimensiones de área configurables (ft² o m²) para mayor comodidad. Con una rueda de paleta de baja fricción y una precisión de velocidad del 3%, el AN200 proporciona mediciones precisas y fiables del viento. Viene completo con una batería de 9 voltios, funda protectora de goma y estuche, siendo una herramienta integral y práctica para profesionales que buscan un medidor de viento de alto rendimiento.
</p>

Extraído de:
https://www.viaindustrial.com/manuales_pdf/anemometro-digital-portatil-con-sensor-de-temperatura-an200-extech-manual-espanol.pdf

**Producto 3:** Medidor de energía solar SP505
**Creador:** EXCTECH instruments

<p align="justify">
El Extech SP505 se destaca como un dispositivo esencial para medir la potencia de la radiación solar y facilitar la determinación de la ubicación ideal para instalaciones solares. Su versatilidad abarca la evaluación de la eficacia de la película solar, la medición precisa de la radiación solar y la comprobación de ventanas con aislamiento solar. En la industria automotriz, este medidor de bolsillo también se emplea para verificar la intensidad de los faros. Su utilidad se extiende incluso a la industria de ventanas, donde los fabricantes y propietarios de viviendas en remodelación confían en él para evaluar la transmisión de radiación solar a través de diferentes espesores de vidrio y niveles de tinte. Además, el SP505 ayuda a encontrar el ángulo óptimo de incidencia para maximizar la eficiencia de paneles solares y calentadores de agua solares. El producto se entrega completamente probado y calibrado.
</p>

<p align="center">
  <img src="https://github.com/Paradoxeado/prototypeProject/blob/main/Im%C3%A1genes/E04Imagen06.png" width="350" style="margin: auto;">
</p>

Extraído de:
https://www.finaltest.com.mx/v/vspfiles/assets/datasheet/SP505_UM.pdf
https://www.comerciogc.com/intranet/assets/images/archivos/43-ficha-tecnica.pdf

## Patentes de Invención
