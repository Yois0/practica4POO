
Objetivo de la practica 
se implementaron una red de sensores conectados a una ESP32, programada en MicroPython, se utilizaron 
* clases y objetos
* clases base y clases especificas 
* encapsulamiento 
* polimorfismo 
* lectura de sensores 
clases
son la estructura principal. Cada bloque classNombre: define cada sensor 

objetos
se crean llamando a la clase. Esto quiere decir que un objeto es un sensor representado en el software

Herencia:
la jerarquia se muestra en una herencia

BaseSensor
* DigitalSensor
* -HallSensor
AnalogSensor
* TemperaturaSensor
* LDRSensor 
* PotenciometroSensor 

Encapsulamiento 
Evita modificar los valores internos desde fuera

Polimorfismo 
Todos los sensores comparten los métodos de read() y as_text() y cada uno se comporta distinto 

Codigo modular

class SensorNetworkApp:
    def _setup_sensors(self):
    def run(self):

Se puede:
* Agregar más se sensores
* Quitar sensores 
* Cambiar pines 
* Modificar la lógica

todo esto se puede hacer, sin romper el resto del código 

Muestreo en la terminal 
La terminal muestra un monitoreo en tiempo real 

No hay variables globales
* Todas las variables se encuentran dentro de las clases 
* Nada está declarado fuera de las funciones y clases, excepto el main()