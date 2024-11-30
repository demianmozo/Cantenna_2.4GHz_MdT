# Proyecto Cantenna_2.4GHz
**Autores**: Facundo Iampietro y Demian N. Mozo  
**Fecha**: Noviembre 2024

------

### Resumen

Este trabajo integra los conocimientos alcanzados por la asignatura "Medios de Transmisión" de 3er año de Ingeniería Electrónica. Se trata de una antena directiva diseñada para funcionar en la banda de frecuencias entre **2.4GHz a 2.462GHz**, la cual abarca los canales de WiFi 1 a 11, utilizados en la República Argentina. 

El diseño se desarrolla alrededor de una **antena de $λ/4$** , utilizando una lata metalica para asignarle directividad. El modelado y las simulaciones se realizaron con el software **CST Studio Suite Learning Edition**.

### Objetivos

- Diseñar e implementar una antena directiva para la frecuencia de 2.4 GHz.
- Verificar su funcionamiento mediante simulaciones y pruebas prácticas.

### Metodología

1. **Diseño Teórico**:

   - Determinación de los parámetros clave de la antena: 
     - Diámetro interno de la lata ($D$).
     - Longitud de la lata ($L$).
     - Longitud del monopolo ($h ≈ λ/4$).
     - Distancia a la que se ubica el monopolo desde el fondo de la lata ($y$).
   - Cálculo de dimensiones óptimas para una frecuencia central de 2.45 GHz.

   Para este caso particular, el diámetro óptimo se estima en $D$ = 9 cm, pues permite el paso de las ondas de interés en un solo modo y elimina el problema de la interferencia intersimbólica. Por otro lado, el largo $L$ no es un parámetro crítico siempre y cuando sea mayor a $3λ/4$ , por lo que siempre es recomendable prolongarlo lo más que se pueda.

2. **Modelado y Simulación**:

   - Modelado paramétrico en **CST Studio Suite**.
   - Análisis del parámetro S11 (reflexión) y del diagrama de radiación para optimizar la directividad y la transferencia de potencia.

3. **Implementación Práctica**:

   - Construcción de la antena usando una lata que se tenia a disposición en el laboratorio, de medidas $D = 9.5$ cm y $L = 33.5$ cm. Esta lata fue seleccionada luego de probar ser la óptima dentro de las disponibles. 
   - Ajustes experimentales en la longitud del monopolo y de la distancia $y$ luego de mediciones con el analizador de espectro.

**A continuación se adjunta el modelo con las respectivas medidas:**  

![3D_con_medidas](/3D_con_medidas.png)

**Diagrama de radiacion de campo lejano:**

![farfield](/farfield.png)

### Resultados

- La simulación inicial mostró una ganancia de **8.26 dBi** en la dirección deseada y un S11 mínimo de **-12 dB** en 2.4 GHz.
- Tras ajustes, el prototipo final alcanzó un S11de **-14.4 dB** a **2.4 GHz**, con una transferencia de potencia óptima en la banda de interés.
- Las mediciones experimentales con el dispositivo nanoVNA mostraron sensibilidad a las irregularidades en el diámetro de la lata, lo cual afectó parcialmente el rendimiento esperado.

### Conclusión

El diseño e implementación de la **Cantenna WiFi** fue exitoso en términos de directividad y ganancia, aunque no se alcanzó una sintonización perfecta para 2.4 GHz debido a limitaciones en los materiales y las condiciones experimentales. Sin embargo, los resultados estuvieron dentro del rango esperado y podrían ser adecuados para aplicaciones que toleren estas desviaciones. 

------

### Referencias

1. Andrade, R. A., et al., "Tecnología Wi-Fi," ENACOM, 2008.
2. "Cantenna: The Poor Mans’ Directional Antenna," Hackaday.io.
3. "PC FAQ’s - Cantenna Calculations."
4. "Waveguide Antenna Calculator."
5. Dassault Systèmes, CST Studio Suite Learning Edition.

------

### Requisitos Técnicos

- **Herramientas**: CST Studio Suite Learning Edition, NanoVNA.
- **Materiales**: Lata metálica, conector coaxial, alambre de cobre.



###### Asignatura Medios de Transmisión - Laboratorio de Comunicaciones - Facultad de Ingeniería - UNMdP

