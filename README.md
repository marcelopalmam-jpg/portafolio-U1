# Ensayo de compresion de una probeta de hormigon 

# Proposito
Este proyecto toma los datos de un ensayo de compresion  hecho a una probeta de hormigon y calcula el esfuerzo que resistio, para despues graficar contra el desplzamiento medido.

# Datos de entrada
Se uso el un archivo llamado `ensayo hormigon final v2.xlsx` principalment, ya que es la version mas reciente de los datos. Por otro lado el archivo `ensayo hormigon.xlsx` se dejo guardado solo como resplado, pero no se uso para los calculos finales.
Existen dos columnas en el archivo:
-`P` : Es la carga aplicada durante el ensayo (kN)
-`u` : Es el desplazamiento registrado (mm)
-`sigma` : Es la resistencia que se obtuvo (MPa)
Las dimensiones de la probeta son D= 150 mm y H= 300 mm. Estos valores no venian confirmados en el proyeto original, por lo que deberian verificarse en el laboratorio.

# Procedimiento 
En primer lugar se calcula el area de la seccion circular de la probeta, que seria de la siguiente manera:

Area = pi * D^2 / 4 = pi * 150^2 / 4 = 17671,46 mm^2
Luego para cada punto del ensayo, se calcula el esfuerzo:

sigma = (P * 1000) / Area   
Se multiplica por 1000 para transformar la carga de kN a N 

Obteniendo estos valores de sigma se genera el grafico de esfuerzo (eje y) contra desplzamiento (eje x).

# Unidades y supuestos
-La carga en kN, el desplzamiento en mm y el esfuerzo en MPa.
- Las medidas de la probeta estan en mm, ya que asi calza perfecto con la formula utilizada.

# Limitaciones
-No se tuvo acceso a la ficha de laboratorio original, asi que no se pudo confirmar con certeza las unidades ni las condiciones del ensayo.
-El grafico que venia en el proyecto heredado era solo una imagen, sin mostrar nada de como se genero, por lo que aca se hizo el procediemiento de eso.

# Herramientas utilizadas
-Se utilizo microsoft excel para calcular los esfuerzos y generar el grafico.