# Simulación de Compuertas Lógicas, Conversor Binario-Hexadecimal y Semáforo con Arduino

## Descripcion
Este repositorio contiene la implementacion de tres practicas fundamentales utilizando Arduino, enfocadas en el aprendizaje de electronica digital y programacion basica.

Los ejercicios fueron desarrollados y probados mediante simulacion en Tinkercad.

Incluye:

- Simulacion de compuertas logicas (AND, OR, NOT)  
- Conversor de binario a hexadecimal con DIP switch y display de 7 segmentos  
- Sistema de semaforo vial con control de tiempos  

El objetivo es comprender el comportamiento de sistemas digitales mediante entradas simuladas y salidas visuales.

---

## Objetivos

- Implementar compuertas lógicas básicas en Arduino  
- Interpretar números binarios usando entradas digitales  
- Mostrar resultados en un display de 7 segmentos  
- Simular un sistema de control secuencial (semáforo)

---

## Materiales (en caso de realizar el ejercico fisicamente)

- Arduino UNO  
- Protoboard  
- Cables jumper  
- Slidesitch  
- DIP switch de 4 posiciones  
- Display de 7 segmentos (cátodo común)  
- LEDs (rojo, amarillo, verde, azul, naranja, verde)  
- Resistencias:
  - 220Ω (para LEDs y display)  
  - 10kΩ (para configuración pull-down)  

---

## Ejercicio 1: Compuertas Lógicas

### Descripción
Se simulan las compuertas AND, OR y NOT mediante dos entradas (A y B) y tres LEDs como salidas.

### Funcionamiento
- AND: se activa únicamente cuando A y B están en estado HIGH
- OR: se activa cuando al menos una entrada está en estado HIGH
<img width="1528" height="635" alt="AND, OR y NOT (and)" src="https://github.com/user-attachments/assets/bcd68eca-2d00-493f-92e8-5355446bd894" />
- NOT: invierte el valor de la entrada A
<img width="1528" height="635" alt="AND, OR y NOT (not)" src="https://github.com/user-attachments/assets/73b826f0-e79d-4fdf-9b52-97cfc1b07376" />
Link: https://www.tinkercad.com/things/0aGrGsCVwd1-and-or-y-not?sharecode=JwMrtHPNC28uOwOgErkmYXutu81OBwd8Icf339_dtA4

---

## Ejercicio 2: Conversor Binario a Hexadecimal

### Descripción
Se utiliza un DIP switch de 4 bits para ingresar un número binario, el cual es interpretado por Arduino y mostrado en un display de 7 segmentos en formato hexadecimal (0–F).
<img width="1528" height="635" alt="Conversor Binario a Hexadecimal (A)" src="https://github.com/user-attachments/assets/bade98f4-7ef7-40f7-9309-b79c4ac2a698" />

### Funcionamiento
- Cada switch representa un bit (b0–b3)  
- Se utiliza configuración pull-down  
- El valor se convierte a decimal y luego a hexadecimal  
- El resultado se muestra en el display mediante activación de segmentos
Link: https://www.tinkercad.com/things/2MQg0y2xCoO-conversor-binario-a-hexadecimal?sharecode=62n05DCqeGau_1AwcDduFM_6MCXRIYSMc1Dm8obiorw 
<img width="1528" height="635" alt="Conversor Binario a Hexadecimal (F)" src="https://github.com/user-attachments/assets/bde95067-6747-41a5-9e87-7596a326de9b" />

---

## Ejercicio 3: Semáforo Vial

### Descripción
Simulación de un sistema de semáforo con tres LEDs y tiempos definidos.

### Secuencia
Verde → Amarillo → Rojo → Amarillo → Verde
<img width="1528" height="635" alt="Semaforo (1)" src="https://github.com/user-attachments/assets/16291a50-a40a-4485-a64d-f7d73d34b23f" />

### Tiempos
- Verde: 5 segundos  
- Amarillo: 2 segundos  
- Rojo: 5 segundos

Link: https://www.tinkercad.com/things/93x5paBOZNU-semaforo?sharecode=W-hDnMCTzTY6zWAXv8GzKIaL5_TZIV7WGRHkC6D4erc
<img width="1528" height="635" alt="Semaforo (2)" src="https://github.com/user-attachments/assets/46cf6b7e-728d-4cf7-9590-fcc73bf33694" />

---

## Consideraciones Técnicas

- Uso de resistencias pull-down para evitar estados flotantes  
- Uso de resistencias limitadoras de corriente en LEDs y display  
- Control de salidas mediante funciones digitales (`digitalWrite`)  
- Lectura de entradas mediante `digitalRead`  
- Implementación de lógica con operadores (`&&`, `||`, `!`)
- Uso de estructuras de control `switch-case` para la selección de valores en el display de 7 segmentos, permitiendo una representación clara y organizada de los valores hexadecimales (0–F).
- Separación de lógica mediante funciones (por ejemplo, funciones de limpieza o de visualización), mejorando la organización y reutilización del código.


---

## Recomendaciones

- Verificar la conexión del display (cátodo común)  
- No exceder la corriente máxima del Arduino  
- Utilizar una resistencia por cada LED o segmento  
- Revisar la polaridad de los componentes  

---

## Conclusión

Este proyecto permite integrar conceptos clave de electrónica digital y programación, facilitando la comprensión de cómo los sistemas lógicos pueden implementarse en hardware real mediante microcontroladores.

---

## Autor

Sergio Alarcón
