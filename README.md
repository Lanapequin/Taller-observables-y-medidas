# Taller Observables y Medidas

## Descripción
En mecánica cuántica, un sistema cuántico discreto puede estar en un estado descrito por un vector de estado o ket que contiene amplitudes complejas. Estas amplitudes representan la probabilidad de que una partícula sea encontrada en una posición particular. El cuadrado del valor absoluto de una amplitud nos da la probabilidad de encontrar la partícula en dicha posición.

Este simulador cuántico ofrece las siguientes funcionalidades:

1. **Probabilidad de posición**: Dado un vector de estado, calcula la probabilidad de encontrar la partícula en una posición específica.

2. **Amplitud de Transición**: Representa un valor complejo que describe la probabilidad de transitar de un estado inicial a uno final. Se utiliza para calcular la probabilidad de transición.

3. **Probabilidad de Transición**:Indica la posibilidad de que un sistema cuántico pase de un estado inicial a un estado final. Se calcula a partir del cuadrado del valor absoluto de la amplitud de transición.

4. **Observable Hermitiano**: Dada una matriz que describe un observable y un vector ket, el sistema verifica que la matriz sea hermitiana. Si lo es, calcula la media y la varianza del observable en el estado dado.

5. **Valores Propios y Probabilidades**: Calcula los valores propios del observable y la probabilidad de que el sistema transite a alguno de los vectores propios después de la observación.

6. **Dinámica del Sistema**: Considera la dinámica del sistema mediante una serie de matrices unitarias $$U_n$$ y calcula el estado final a partir de un estado inicial.

En conjunto, este simulador ofrece una herramienta poderosa para explorar y comprender los principios fundamentales de la mecánica cuántica.

## Ejercicio 4.5.2

Este ejercicio aborda la formulación del vector de estado para un sistema de partículas con spin, comenzando con dos partículas y luego me piden generalizarlo a (n) partículas.

### 1. Sistema de Dos Partículas con Spin

Para un sistema de dos partículas, cada una puede estar en uno de dos estados de spin: "arriba" |↑⟩ o "abajo" |↓⟩. Los estados básicos son:

1. |↑↑⟩
2. |↑↓⟩
3. |↓↑⟩
4. |↓↓⟩

El vector de estado genérico para dos partículas se expresa como:

$$
|\psi\rangle = a_{1} |\uparrow \uparrow\rangle + a_{2} |\uparrow \downarrow\rangle + a_{3} |\downarrow \uparrow\rangle + a_{4} |\downarrow \downarrow\rangle
$$

donde $$a_{1}, a_{2}, a_{3}, a_{4}$$ son coeficientes complejos que representan las amplitudes de probabilidad de cada estado.

### 2. Generalización a (n) Partículas

Para un sistema de (n) partículas, el número total de estados básicos es $$2^n$$ El vector de estado genérico se escribe como:

$$
|\psi\rangle = \sum_{i=1}^{2^n} a_i |s_i\rangle
$$

donde |sᵢ⟩ representa el i-ésimo estado básico del sistema de n partículas, y aᵢ son coeficientes complejos.

## Ejercicio 4.5.3

Un **estado separable** en mecánica cuántica significa que se puede escribir como el producto tensorial de estados independientes de los subsistemas que lo componen. 
Un estado $$|\psi\rangle$$ es separable si puede escribirse de la forma:

$$
|\psi\rangle = |\psi_1\rangle \otimes |\psi_2\rangle
$$

donde $$|\psi_1\rangle$$ es el estado del primer subsistema y $$|\psi_2\rangle$$ es el estado del segundo subsistema.

Por otro lado, si el estado no puede escribirse de esta forma, se considera un **estado entrelazado**.


- En este caso, para poder determinar si el estado del ejercicio 4.5.3 es separable o no, se realiza el siguiente procedimiento:
### Paso 1: Reescribir el estado

El estado del ejercicio es:

$$
|\phi\rangle = |x_0\rangle \otimes |y_1\rangle + |x_1\rangle \otimes |y_1\rangle.
$$

Tanto el primer término $$|x_0\rangle \otimes |y_1\rangle$$ como el segundo término $$|x_1\rangle \otimes |y_1\rangle$$ tienen en común el estado $$|y_1\rangle$$  

Esto significa que se puede factorizar $$|y_1\rangle$$ fuera de la expresión:

$$
|\phi\rangle = (|x_0\rangle + |x_1\rangle) \otimes |y_1\rangle.
$$

### Paso 2: Interpretación de la factorización

Al escribir $$|\phi\rangle$$ de esta manera, se observan dos partes:

1. |x₀⟩ + |x₁⟩ describe un estado del **primer subsistema**.

2. |y₁⟩ describe un estado del **segundo subsistema**.


### Paso 3: Significado de separabilidad

En este caso, logré escribir el estado completo como:

$$
|\phi\rangle = (|x_0\rangle + |x_1\rangle) \otimes |y_1\rangle
$$

lo cual **sí** es un producto tensorial entre un estado del primer subsistema 

$$
|x_0\rangle + |x_1\rangle
$$

y un estado del segundo subsistema 

$$
|y_1\rangle
$$

### Conclusión

Esto significa que el estado es **separable** porque se descompuso el estado total en dos partes que corresponden a estados de los subsistemas individuales.


## Instrucciones
Configuración del Entorno:

Activa el entorno virtual:
- En Windows:
```
.venv\Scripts\activate
```
- En macOS y Linux:
```
source .venv/bin/activate
```

## Prerrequisitos
Para ejecutar **Observables.ipynb**, asegúrate de tener instaladas las siguientes librerías:

- **NumPy**: para realizar cálculos matemáticos.
- **Matplotlib**: para generar gráficos.

Puedes instalar las dependencias necesarias utilizando pip:

```
pip install numpy matplotlib
```

### Construido con
Este proyecto fue construido con [Python 3.12](https://www.python.org/)

### Colaboradores
Laura Natalia Perilla Quintero [Lanapequin](https://github.com/Lanapequin)