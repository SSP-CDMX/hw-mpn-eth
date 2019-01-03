# Plataforma Mi Policía en Mi Negocio - Ethernet
Hardware MPN Ethernet

La plataforma  **Mi Policía en Mi Negocio** es un grupo de tecnologías aplicadas para la prevención e inhibición del delito, tecnologías que definen una red de alarmas silenciosas activadas mediante dispositivos móviles o electrónicos comunicadas por Internet.

Esta plataforma consta de una parte pública y una parte controlada y administrada exclusivamente por la Policía de la Ciudad de México, por lo tanto **todos** los servicios que ofrece la plataforma son totalmente **gratuitos**.

La parte controlada es una base de datos georeferenciada de los negocios afiliados y sus sucursales, a fin de brindar una URL que permite disparar una llamada de alerta en la infraestructura privada de la Policía, a fin de poder despachar la patrulla mas cercana.


Si usted desea registrar su negocio le sugerimos llenar el [formulario de pre-registro. ](http://mipolicia.ssp.cdmx.gob.mx/mpn/preafiliacion)


Lo que hay en este repositorio es la parte pública. 

Esta parte pública se libera bajo licencia **Atribución-CompartirIgual 2.5 México  (CC BY-SA 2.5 MX)**, al tratarse de un derivado de la plataforma **Arduino**, por lo tanto, lo que encontrará aquí son las especificaciones para armar su propio circuito **DIY-MiPolicia**, exactamente como el que obtendría al asistir a los talleres que imparte la Policía de la Ciudad de México.

## Cómo se arma
Puedes armar el circuito de Mi Policia muy fácilmente, en tu casa, con componentes fáciles de obtener, ...

## Lista de materiales básica
Esta lista contiene los componentes mínimos necesarios para armar el módulo mínimo de Mi Policía

|  Cantidad      |Descripción                          |Referencia gráfica                         |
|----------------|-------------------------------|-----------------------------|
|1|Shield Ethernet para Arduino            | ![Arduino Ethernet Shield](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/Arduino%20Ethernet%20Shield.png)           |
|1|Tarjeta Micro SD 8Gb           |![Micro SD 8 Gb](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/MicroSD.png) |
|1|Regulador de Voltaje L7805 5v|![Regulador L7805](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/L7805.png)|
|1|Disipador de Calor 8x8x5 mm|![Disipador de Calor](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/DisipadorCalor.png)|
|1|Micro controlador ATMEGA 328 |![ATMega 328](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/ATMega328.png)|
|1|Base para Micro controlador ATMEGA 328 (28 pines) |![Base para Micro controlador](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/BaseATMega.png)|
|1|Cristal oscilador 16 MHz|![Cristal oscilador 16 MHz](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/Oscilador16MHz.png)|
|1|Conector Jack hembra, alimentación debe conicidir con la entrada de la fuente de alimentación|![Conector Jack hembra](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/JackHembraAlimentacion.png)|
|1|Capacitor Electrolítico 0.1  $\mu$Farad a 50 volts|![Capacitor Electrolítico](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/CapacitorElectrolitico.png)|
|1|Capacitor 100 nano Faradios|![Capacitor 100 nano Faradios](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/CapacitorNanoFarads.png)|
|2|Capacitor 22 pico Faradios|![Capacitor 22 pico Faradios](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/CapacitorNanoFarads.png)|
|5|Resistencia de Carbón 220 $\Omega$  1/2 Watt|![Resistencia de Carbón 220 Ohms](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/Resistencia200Ohms.png)|
|5|Resistencia de Carbón 10 K$\Omega$  1/2 Watt|![Resistencia de Carbón 10 KOhms](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/Resistencia10Ohms.png)|
|1|Eliminador 120 - 9 VCD 0.850mA o 1 A con entrada para Jack hembra alimentación |![Eliminador 120V - 9V](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/Eliminador120.png)|
|1|Gabinete de plástico con tapa, de 15x9x6 cm aproximadamente|![Gabinete de plástico](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/Gabinete.png)|
|1| 1 metro de soldadura de estaño|![Soldadura de Estaño](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/Soldadura.png)|
|2| Puntas para cautín Weller de 23 o 25W|![Puntas para cautín](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/PuntasCautin.png)|
|1| Metro de tubo Thermofit de 1 mm de diámetro|![Metro de tubo Thermofit](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/ThermoFit.png)|
|4| Tira de Conector de tres cables|![Tira de Conector de tres cables](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/Conector3Cables.png)|
|1|Metro de Alambre de 1 hilo para conectar circuitos electrónicos |![Alambre de 1 hilo para conectar circuitos electrónicos](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/Alambre1Hilo.png)|
|1|Paquete con 4 tiras de Headers apilables para nuevos modelos Arduino |![Paquete con 4 tiras de Headers apilables para nuevos modelos Arduino](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/HeadersApilables.png)|
|1|Tira sencilla de 36 Header macho |![Tira sencilla de 36 Header macho](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/HeaderMacho.png)|
|2|Tira de header y conector apilable|![Tira de header y conector apilable](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/HeaderConectorApilable.png)|
|1|Tubo de Silicón Frío|![Tubo de Silicón Frío](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/TuboSilicon.png)|
|1|Diodo Led Rojo |![Diodo Led Rojo](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/LedRojo.png) |
|1|Diodo Led Verde|![Diodo Led Verde](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/Led.png)|
|1|Diodo Led Azul|![Diodo Led Azul](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/Led.png)|
|1|Bornera de Audio con 9 terminales |![Bornera de Audio con 9 terminales](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/Bornera.png)|
|1|Fusible F500L 500 miliAmperes (5x20mm)|![Fusible F500L 500 miliAmperes (5x20mm)](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/Fusible.png)|
|2|Porta fusible F500L (5x20mm)|![Porta fusible F500L (5x20mm)](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/PortaFusible.png)|

## Lista de materiales extendida
Esta lista contiene los accesorios necesarios para los diferentes modos electrónicos de activación.

 - Botón físico
 - Botón inalámbrico
 - Alarma propia (cuando ya se invirtió en una alarma propia)
 - Sensor magnético
 - Sensor de movimiento

|  Cantidad      |Descripción                          |Referencia gráfica                         |
|----------------|-------------------------------|-----------------------------|
|1|Botón físico| ![Botón físico](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/BotonFisico.png)
|1|Receptor simple de RF M4-315 MHz|![Receptor simple de RF](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/ReceptorRF315MHz.png) |
|1|Control remoto RF Tipo llavero 305 MHz|![Control remoto RF Tipo llavero 305 MHz](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/ControlRemoto350Mhz.png) |
|1|Relevador 12v CD (Para un funcionamiento óptimo, deberá ser tal cual se muestra en la imagen)| 
|1|Sensor magnético|![Relevador 12v CD](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/Reelevador12V.png)|
|1|Sensor PIR HC-SR501|![PIR HC-SR501](https://raw.githubusercontent.com/SSP-CDMX/hw-mpn-eth/master/Imagenes/PIR.png)|
