# Proyecto Final - Equipo: Tilines

## Introduccion
 En un mundo cada vez más interconectado y digitalizado, la integración de la inteligencia artificial (IA) ha emergido como un componente fundamental para potenciar y optimizar numerosos proyectos. En esta era de avances tecnológicos acelerados, la capacidad de aprovechar el poder de la IA se convierte en un diferenciador clave para el éxito y la evolución continua de cualquier iniciativa.

 El presente proyecto se gesta como una extensión y enriquecimiento de una base sólida previamente establecida. Partiendo de la premisa de este trabajo final busca expandir sus capacidades y funcionalidades mediante la integración estratégica de técnicas y algoritmos de IA. La incorporación de estos elementos proporcionará un impulso significativo al proyecto, mejorando su eficiencia, precisión y adaptabilidad en un entorno cambiante.




# Sistema Gestor De Temperatura De Hospitales
## Creación de Servidor
## La visualización de una de las instancias del equipo, se presenta a continuación:
![image](https://github.com/tectijuana/sp5-iot-ai-los-tiliners-1/assets/80359457/59bca619-5037-43bc-85cb-22d20edb0625)
Las características de la instancia mostrada son las siguientes:
![image](https://github.com/tectijuana/sp5-iot-ai-los-tiliners-1/assets/80359457/f4e50383-2604-4832-bec5-6f09c80bdad5)
## Se considero la siguiente configuración para los puertos del servidor:

![image](https://github.com/tectijuana/sp5-iot-ai-los-tiliners-1/assets/80359457/3426da4c-b47a-4af0-b625-c3c372079eae)

# Conexión de Servidor
## Para realizar la conexión con el servidor desde un ordenadro, se ejecutaron los siguientes comandos desde la Terminal:

![image](https://github.com/tectijuana/sp5-iot-ai-los-tiliners-1/assets/80359457/62d33610-484b-4aec-87dc-f82540492d01)

# Instalación y uso de Mosquitto en servidor
## Se realizó la instalación de Mosquitto y Mosquitto Clients

![image](https://github.com/tectijuana/sp5-iot-ai-los-tiliners-1/assets/80359457/c73706de-e5cf-4304-94d5-bc01ffc8cffa)

Instalación de Mosquitto en Linux (Ubuntu)
Paso 1: Actualización del sistema

sudo apt update 

sudo apt upgrade

Paso 2: Instalación de Mosquitto

sudo apt install mosquitto

Paso 3: Verificación del estado de Mosquitto

sudo systemctl status mosquitto

Uso básico de Mosquitto

Paso 1: Iniciar el servicio de Mosquitto

sudo systemctl start mosquitto

Paso 2: Verificar el estado del servicio

sudo systemctl status mosquitto

Paso 3: Prueba de conexión

Puedes utilizar el comando mosquitto_pub para publicar un mensaje y mosquitto_sub para suscribirte y recibir mensajes en un tópico MQTT.

Ejemplo de publicación:


mosquitto_pub -h localhost -t "mi/topico" -m "Hola, Mosquitto!"

Ejemplo de suscripción:

mosquitto_sub -h localhost -t "mi/topico"

Estos comandos son básicos para probar la funcionalidad de Mosquitto. Para aplicaciones más avanzadas, como configurar autenticación, encriptación SSL/TLS u otras opciones de configuración, se requerirán pasos adicionales.

![image](https://github.com/tectijuana/sp5-iot-ai-los-tiliners-1/assets/80359457/2d24fec8-b7f8-4f0d-9241-e3bf5c4bf4f2)

## Se puede comprobar que la instalación fue exitosa revisando el servicio en ejecución del siguinte modo:

![image](https://github.com/tectijuana/sp5-iot-ai-los-tiliners-1/assets/80359457/1e9769dd-702d-40b9-998e-2293f25349b0)

## Instalación de Prometheus

![image](https://github.com/Mayra1207/Proyecto-Final---Tilines/assets/89611745/87abd6e0-d2b3-4082-9c07-8cb144d99137)

Instalación de Prometheus:

Paso 1: Descargar Prometheus

Visita el sitio web de Prometheus para obtener la última versión: Prometheus Downloads.

Elige la versión adecuada para tu sistema operativo (Linux, Windows, MacOS, etc.).

Descarga el archivo comprimido.

Paso 2: Descomprimir el archivo

Utiliza un software para descomprimir el archivo descargado.

Ubica el directorio donde desees instalar Prometheus.

Paso 3: Configurar Prometheus

En el directorio de instalación, busca el archivo prometheus.yml. Este es el archivo de configuración principal de Prometheus.

Edita este archivo para configurar los objetivos de scraping (puntos de datos a los que Prometheus se conectará para recopilar métricas). Por ejemplo:

global:

  scrape_interval: 15s

scrape_configs:

  - job_name: 'mi_aplicacion'
    
    static_configs:
    
      - targets: ['localhost:9090'] # Ejemplo de un servicio en localhost
        
Puedes agregar más configuraciones según sea necesario para tus objetivos específicos.

Paso 4: Ejecutar Prometheus

Abre una terminal o línea de comandos.

Navega al directorio donde se encuentra el ejecutable de Prometheus.

Ejecuta el comando para iniciar Prometheus:

./prometheus --config.file=prometheus.yml

Paso 5: Acceder a la interfaz de Prometheus

Abre un navegador web.
Ingresa la dirección http://localhost:9090 (si estás utilizando la configuración por defecto) para acceder a la interfaz web de Prometheus.


 La instalación de Prometheus en sistemas programables es un proceso fundamental para habilitar el monitoreo y la recolección de métricas en tiempo real. Prometheus, una herramienta de código abierto, permite recopilar datos de sistemas diversos y esencialmente programables, ofreciendo así información crucial para el análisis, la toma de decisiones y el mantenimiento proactivo de dichos sistemas.

# Acceso al servidor

![image](https://github.com/Mayra1207/Proyecto-Final---Tilines/assets/89611745/10e6973d-0427-45c0-aad7-ab42fc06d7b3)

### Actualizar ubuntu, enlistado, las aplicaciones 

![image](https://github.com/Mayra1207/Proyecto-Final---Tilines/assets/89611745/b324e1e4-9059-4c98-bf5b-24b1e637e71a)

![image](https://github.com/Mayra1207/Proyecto-Final---Tilines/assets/89611745/0de35201-91fd-4ebb-9468-00a3b441e051)

![image](https://github.com/Mayra1207/Proyecto-Final---Tilines/assets/89611745/16a661f0-6754-44b4-b404-3f074f4b8c95)

![image](https://github.com/Mayra1207/Proyecto-Final---Tilines/assets/89611745/837446de-fef3-4c4b-a835-cd3de04a3189)

![image](https://github.com/Mayra1207/Proyecto-Final---Tilines/assets/89611745/9a01b963-12f0-41b7-a82c-45d5f19a33b1)

![image](https://github.com/Mayra1207/Proyecto-Final---Tilines/assets/89611745/777fbf2c-5422-4335-b1a7-744a0ba32918)


## Instalación de Grafana
![image](https://github.com/Mayra1207/Proyecto-Final---Tilines/assets/89611745/14e82dd9-fb06-4ee7-8f88-3cbe862cf594)

Su instalación en esta materia ofrece a los estudiantes la capacidad de crear paneles interactivos y gráficos dinámicos para analizar datos provenientes de sistemas programables como Arduino, Raspberry Pi o dispositivos similares. Esta instalación permite explorar y entender el rendimiento y comportamiento de estos sistemas a través de representaciones visuales intuitivas y personalizables.

# Programa pico
## Para comenzar con el proyecto se tiene como referencia la actividad 3.2.1 de la asignatura de sistemas programables. Consiste en el siguiente código:
```python
################################################################################
# Nombre del Archivo: main.py
# Autores:           
# Luis Mardueno 19211677 
# Mayra Itzel Bamaca Hernandez 2021185
# Cesar Andree Morales Castillo 20211816
# Sencion Salas Jose Oscar 20212430
# Alan Fernando diaz Garduño 18210990
# Gutierrez Mora Karime Isabel 19211653
# Dennies victor Sanchez Rompelotto C19212433
# Alvarez Lopez Alex Omar 20211753
#
#
# Correo:            l20212430@tectijuana.edu.mx
# Fecha:             01/12/23
# Institución:       Tecnológico Nacional de México (TECNM) - Campus ITT
# Curso:             Sistemas Programables 
#
# Objetivo:
# La propuesta de este programa es brindar una solución flexible para la infraestructura de un hospital. Se propone un
# sistema que brinde la capacidad de monitorear un hospital, con el objetivo de mantener la instalación dentro de
# un rango determinado de valores ambientales, de modo que se mantenga el control de un sector desterminado del edificio.



# Historial de Revisiones:
# 01/12/23        Sención Salas José Oscar - Creado
# 01/12/23        Sención Salas José Oscar - Actualizado para añadir funcionamiento base
#
# Enlace a GitHub Repository ó GIST:
# https://github.com/tectijuana/sp5-iot-ai-los-tiliners-1/new/main?readme=1
#
# Enlace a Wokwi :
# https://wokwi.com/projects/381617378640964609
#
# Licencia:
# Este programa es software libre y puede ser redistribuido y/o modificado bajo los términos de la Licencia Pública General GNU
# como está publicado por la Free Software Foundation, ya sea la versión 3 de la Licencia, o (a tu elección) cualquier versión posterior.
#
# Este programa se distribuye con la esperanza de que sea útil, pero SIN GARANTÍA ALGUNA; incluso sin la garantía implícita de
# COMERCIALIZACIÓN o APTITUD PARA UN PROPÓSITO PARTICULAR. Consulte la Licencia Pública General GNU para obtener más detalles.
#
# Deberías haber recibido una copia de la Licencia Pública General GNU junto con este programa. Si no es así, consulte <http://www.gnu.org/licenses/>.
#
################################################################################
# Importación de módulos necesarios
import network
import time
from machine import Pin
import dht
import ujson
from umqtt import MQTTClient


# Código principal
# Parametros MQTT Server
MQTT_CLIENT_ID = "micropython-weather-demo"
MQTT_BROKER    = "broker.mqttdashboard.com"
MQTT_USER      = ""
MQTT_PASSWORD  = ""
MQTT_TOPIC     = "wokwi-weather"

#Asignacion del pin del sensor
DHT22 = dht.DHT22(Pin(15))

#Modulo de conexion a internet
print("Connecting to WiFi", end="")
wlan = network.WLAN(network.STA_IF)
wlan.active(True)
wlan.connect("Wokwi-GUEST", "")
while not wlan.isconnected():
  print(".", end="")
  time.sleep(0.1)
print(" Connected!")
print(wlan.ifconfig())

#Modulo de conexion al servidor MQTT
print("Connecting to MQTT server... ", end="")
client = MQTTClient(MQTT_CLIENT_ID, MQTT_BROKER, user=MQTT_USER, password=MQTT_PASSWORD)
client.connect()

print("Connected!")

#Lectura continua del sensor
prev_weather = ""
while True:
  print("Measuring weather conditions... ", end="")
  DHT22.measure() 
  message = ujson.dumps({
    "temp": DHT22.temperature(),
    "humidity": DHT22.humidity(),
  })
  if message != prev_weather:
    print("Updated!")
    print("Reporting to MQTT topic {}: {}".format(MQTT_TOPIC, message))
    client.publish(MQTT_TOPIC, message)
    prev_weather = message

  else:
    print("No change")
  time.sleep(1)
```


Material Visual Utilizado:

![image](https://github.com/Mayra1207/Proyecto-Final---Tilines/assets/89611745/67fb54d3-7ddb-40ba-9e47-ef487d595753)

https://gist.github.com/IoTeacher/bf51fae05191256c2d83b3a14723cf89

![image](https://github.com/Mayra1207/Proyecto-Final---Tilines/assets/89611745/b30e7a91-dab4-4a9d-b398-31c25242f971)

https://electrocredible.com/raspberry-pi-pico-w-data-logger-temperature-micropython/


