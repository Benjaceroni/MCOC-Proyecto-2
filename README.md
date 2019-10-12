# MCOC-Proyecto-2-Entrega-4
Proyecto 2 Metodos computacionales para Obras Civiles

Se consideran parametros de la simulación con diametro de particulas de 5.6 mm, un dt de 0.001, tiempo máximo de 0.5 segundos, en donde se obtienen los siguientes resultados

## Especificaciones del computador
  
  - Windows 10 Home
  - Procesador AMD Ryzen 5 1600X Six-Core 3.60 GHz
  - RAM 16 GB
  - Sistema operativo de 64 bits, procesador basado en x64

## Método de implementación del codigo

Se utilizaron valores entregados entregados por el profesor con anterioridad, presentados con el nombre de "simulacion-1", "simulacion-2", "simulacion-3" y "simulacion-4", en los cuales se tienen la cantidad de particulas a simular, sus posiciones y velocidades iniciales y los resultados esperados a obtener, con el objetivo de poder comparar estos resultados con los propios obtenidos.
Es necesario agregar que cada simulación se corrio 3 veces para obtener un tiempo de operación promedio.

## Características, tiempo y resultados de cada simulación

**Simulación 1**
- Cantidad de partículas: 10
- Tiempo de modelación por profesor: 251.5 seg.
- Resultado obtenido por profesor:

![particle_trajectories](https://user-images.githubusercontent.com/53712580/66692396-636d9c00-ec74-11e9-8893-82cb07cc696b.png)

**Tiempo y resultados obtenidos por codigo**

Tiempo = 632.81 seg.

Resultado:

![sim1](https://user-images.githubusercontent.com/53712580/66692580-2efadf80-ec76-11e9-837a-0f5ac8bf21db.PNG)


**Simulación 2**
- Cantidad de partículas: 5
- Tiempo de modelación por profesor: 115.1 seg.
- Resultado obtenido por profesor:

![particle_trajectories](https://user-images.githubusercontent.com/53712580/66692387-518bf900-ec74-11e9-8f4c-d8b2ae59a600.png)

**Tiempo y resultados obtenidos por codigo**

Tiempo = 62.4 seg.

Resultado:

![Sim2](https://user-images.githubusercontent.com/53712580/66692417-8f891d00-ec74-11e9-946f-05efd6d9d32e.PNG)

**Simulación 3**
- Cantidad de partículas: 2
- Tiempo de modelación por profesor: 44.1 seg.
- Resultado obtenido por profesor:

![particle_trajectories](https://user-images.githubusercontent.com/53712580/66692384-37eab180-ec74-11e9-816d-df076c8d23e9.png)

**Tiempo y resultados obtenidos por codigo**

Tiempo = 6.7 seg.

Resultado:

![Sim3](https://user-images.githubusercontent.com/53712580/66692428-a465b080-ec74-11e9-8aab-4c2cf3129ce7.PNG)

**Simulación 4**
- Cantidad de partículas: 20
- Tiempo de modelación por profesor: 447.0 seg.
- Resultado obtenido por profesor:

![particle_trajectories](https://user-images.githubusercontent.com/53712580/66692372-273a3b80-ec74-11e9-8f6c-392e1bbd8c73.png)

**Tiempo y resultados obtenidos por codigo**

Tiempo = aproximadamente unos 5400 seg.

Resultado: 

Desafortunadamente, el programa no logro entregar un grafico de este caso, y considerando lo mucho que demoraba en correr, se opto por no mostrar resultados.

## Observaciones

Probablemente, uno de los motivos de porque este codigo logra ser más rapido a menores particulas pero mas lento a mayores particulas (llegando a un punto inutilizable) es por el ciclo for en la definicion particula(z,t), pues cuando son pocas particulas es capaz de realizar las pruebas de choques entre estas de manera rapida, sin embargo, cuando son muchas particulas, el programa no es capaz de realizar este ciclo con gran rapidez y produce la lentitud mostrada. Es necesario realizar mayor testeo en esa parte del codigo, y es posible realizar optimizaciones en este mismo para que demore rangos de tiempos aceptables.
