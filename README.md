# Depto de Sistemas y Computación
# Ing. En Sistemas Computacionales
# SISTEMAS PROGRAMABLES 23a


# OBJETIVO:


# CÓDIGO
```python
## Depto de Sistemas y Computación
## Ing. En Sistemas Computacionales
## SISTEMAS PROGRAMABLES 23a
## Autor (es): ___________
## Repositorio:  
## Fecha de revisión:   99/99/2023
## Objetivo:
##   

# Sensor RP2040

Codigo:
import machine

# Configura el pin del botón
button_pin = machine.Pin(14, machine.Pin.IN, machine.Pin.PULL_DOWN)

# Función para manejar la interrupción del botón
def button_interrupt(pin):
    if pin.value() == 1:
        print("¡Botón presionado!")

# Configura la interrupción del botón
button_pin.irq(trigger=machine.Pin.IRQ_RISING, handler=button_interrupt)

# Bucle principal
while True:
    pass

# PRUEBAS

```
![Texto alternativo](https://scontent.ftij1-2.fna.fbcdn.net/v/t1.15752-9/344301652_100384643068951_3791336422858187356_n.png?_nc_cat=106&ccb=1-7&_nc_sid=ae9488&_nc_ohc=6-69AexMVbkAX8Mqudk&_nc_ht=scontent.ftij1-2.fna&oh=03_AdSZt4PXZIdRq495ywLauZXxLxLr5DLUxK5q-e1aV6vqJA&oe=64890BF7)






#Sensor RP2040
```python
import machine

# Configura el pin del potenciómetro
potentiometer_pin = machine.ADC(26)

# Bucle principal
while True:
    # Lee el valor analógico del potenciómetro
    potentiometer_value = potentiometer_pin.read_u16()

    # Imprime el valor leído
    print("Valor del potenciómetro:", potentiometer_value)


```
![Texto alternativo](https://scontent.ftij1-1.fna.fbcdn.net/v/t1.15752-9/344301214_1264726620834552_3319900546932863438_n.png?_nc_cat=110&ccb=1-7&_nc_sid=ae9488&_nc_ohc=_06ySVvvLJ4AX-l0-vd&_nc_ht=scontent.ftij1-1.fna&oh=03_AdSGw1HjAWfefChq4z0SGgbPURZDRsS6QRqTgzXbcJms6Q&oe=648918F5)

Led laser

```python
import machine
import time

# Configuración del pin GPIO
led_pin = machine.Pin(7, machine.Pin.OUT)

# Enciende el LED
led_pin.value(0)
print('Led prendido')
# Espera 1 segundo
time.sleep(10)

# Apaga el LED
led_pin.value(1)
print('Led apagado')

```

![](https://scontent.ftij1-2.fna.fbcdn.net/v/t1.15752-9/344300433_256959086837359_952338236435345702_n.png?_nc_cat=103&ccb=1-7&_nc_sid=ae9488&_nc_ohc=bBfD9If0DjYAX8lo8CL&_nc_ht=scontent.ftij1-2.fna&oh=03_AdREC2fYyh8bN-zrEjFjlTBdyQ0eZrONQfkC-qv5NfWijg&oe=648946F0)

![](https://scontent.ftij1-2.fna.fbcdn.net/v/t1.15752-9/349058431_574392501404259_3150481255012632406_n.jpg?_nc_cat=100&ccb=1-7&_nc_sid=ae9488&_nc_ohc=PBhjY3E078AAX9A2uN1&_nc_ht=scontent.ftij1-2.fna&oh=03_AdSjhtd2jgymXjBagP_4ngjNNcczPugfKsJf6OB2FLfBhQ&oe=6496487D)

# CONCLUSIONES
_esta es conclusión_
