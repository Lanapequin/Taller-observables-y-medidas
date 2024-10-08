# Taller Observables y Medidas

## Descripción
En mecánica cuántica, un sistema cuántico discreto puede estar en un estado descrito por un vector de estado (o ket) que contiene amplitudes complejas. Estas amplitudes representan la probabilidad de que una partícula sea encontrada en una posición particular. El cuadrado del valor absoluto de una amplitud nos da la probabilidad de encontrar la partícula en dicha posición.

Este simulador cuántico ofrece las siguientes funcionalidades:

1. **Probabilidad de posición**: Dado un vector de estado, calcula la probabilidad de encontrar la partícula en una posición específica.

2. **Amplitud de Transición**: Representa un valor complejo que describe la probabilidad de transitar de un estado inicial a uno final. Se utiliza para calcular la probabilidad de transición.

3. **Probabilidad de Transición**:Indica la posibilidad de que un sistema cuántico pase de un estado inicial a un estado final. Se calcula a partir del cuadrado del valor absoluto de la amplitud de transición.

4. **Observable Hermitiano**: Dada una matriz que describe un observable y un vector ket, el sistema verifica que la matriz sea hermitiana. Si lo es, calcula la media y la varianza del observable en el estado dado.

5. **Valores Propios y Probabilidades**: Calcula los valores propios del observable y la probabilidad de que el sistema transite a alguno de los vectores propios después de la observación.

6. **Dinámica del Sistema**: Considera la dinámica del sistema mediante una serie de matrices unitarias \(U_n\) y calcula el estado final a partir de un estado inicial.

En conjunto, este simulador ofrece una herramienta poderosa para explorar y comprender los principios fundamentales de la mecánica cuántica.

## Prerrequisitos
Para ejecutar el código, asegúrate de tener instalados los siguientes paquetes:

- **NumPy**: para realizar cálculos matemáticos.

Puedes instalar las dependencias necesarias utilizando pip:

```bash
pip install numpy
```
