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
- NOT: invierte el valor de la entrada A  

---

## Ejercicio 2: Conversor Binario a Hexadecimal

### Descripción
Se utiliza un DIP switch de 4 bits para ingresar un número binario, el cual es interpretado por Arduino y mostrado en un display de 7 segmentos en formato hexadecimal (0–F).

### Funcionamiento
- Cada switch representa un bit (b0–b3)  
- Se utiliza configuración pull-down  
- El valor se convierte a decimal y luego a hexadecimal  
- El resultado se muestra en el display mediante activación de segmentos  

---

## Ejercicio 3: Semáforo Vial

### Descripción
Simulación de un sistema de semáforo con tres LEDs y tiempos definidos.

### Secuencia
Verde → Amarillo → Rojo → Amarillo → Verde

### Tiempos
- Verde: 5 segundos  
- Amarillo: 2 segundos  
- Rojo: 5 segundos  

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
