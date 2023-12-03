---
---

# Oscilación

Es el movimiento de ida y vuelta de un objeto alrededor de un punto central o posicion.
Para entender la oscilación necesitamos un poco de trigonometría, la matemática de los triángulos. 
Mediante trigonometría podemos resolver la velocidad angular o la aceleración de giro de un objeto
mientras se mueve. Con senos y cosenos se pueden modelar patrones de aceleracion-deceleración, como
el balance de un pendulo.

## Ángulos

P5 mide los ángulos en radianes 

```radians = 2PI x degrees / 360```

En P5 se puede cambiar a grados con `angleMode(DEGREES)` o `radians(degrees)`.

Pero es mas standard usar radianes.

## Movimiento angular

La rotación también es el movimiento angular, es lo mismo. La tasa de cambio de la posición en el tiempo es la velocidad angular. Y la aceleración angular es la descripción de los cambios de velocidad angular.

```
velocidad angular = velocidad angular + aceleración angular
angulo = angulo + velocidad angular
```

En este caso, el angulo, la velocidad angular y la aceleracion angular tienen una única dimension, son escalares, en lugar de vectores. En un espacio 2D solo hay un ángulo de rotación, en un espacio 3D serían 2 angulos y necesitaríamos de un vector. 

Para estas fórmulas asumimos un delta time de 1, que multiplica por el cambio temporal.

