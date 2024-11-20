# Proyecto Cantenna_2.4GHz
Este trabajo integra los conocimientos alcanzados por la asignatura "Medios de Transmisión" de 3er año de Ingeniería Electrónica. Se trata de una antena directiva diseñada para funcionar en la banda de frecuencias entre **2.4GHz a 2.462GHz**, la cual abarca los canales de WiFi 1 a 11, utilizados en la República Argentina. 

El diseño se desarrolla alrededor de una **antena de $λ/4$** , utilizando una lata metalica para asignarle directividad. El modelado y las simulaciones se realizaron con el software **CST Studio Suite Learning Edition**.

Los paramétros a ajustar para este diseño son los siguientes:

- Diámetro interno de la lata ($D$).
- Longitud de la lata ($L$).
- Longitud del monopolo ($h ≈ λ/4$).
- Distancia a la que se ubica el monopolo desde el fondo de la lata ($y$).

Para este caso particular, el diámetro óptimo se estima en $D$ = 9 cm, pues permite el paso de las ondas de interés en un solo modo y elimina el problema de la interferencia intersimbólica. Por otro lado, el largo $L$ no es un parámetro crítico siempre y cuando sea mayor a $3λ/4$ , por lo que siempre es recomendable prolongarlo lo más que se pueda, 

Sin embargo, esta antena fue implementada con una lata que se tenia a disposición en el laboratorio, de medidas $D = 9.5$ cm y $L = 33.5$ cm. Esta lata fue seleccionada luego de probar ser la óptima dentro de las que teniamos a disposición. 

#### A continuación se adjunta el modelo con las respectivas medidas:  

![3D_con_medidas](/Users/demian/Desktop/Cantenna_2.4GHz_MdT/3D_con_medidas.png)

#### Diagrama de radiacion de campo lejano:

![farfield](/Users/demian/Desktop/Cantenna_2.4GHz_MdT/farfield.png)

###### Asignatura Medios de Transmisión - Laboratorio de Comunicaciones - Facultad de Ingeniería - UNMdP

