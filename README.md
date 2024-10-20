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

## Ejercicio 4.5.2

Este ejercicio aborda la formulación del vector de estado para un sistema de partículas con spin, comenzando con dos partículas y generalizándolo a \( n \) partículas.

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

### 2. Generalización a \( n \) Partículas

Para un sistema de \( n \) partículas, el número total de estados básicos es \( 2^n \). El vector de estado genérico se escribe como:

$$
|\psi\rangle = \sum_{i=1}^{2^n} a_i |s_i\rangle
$$

donde |sᵢ⟩ representa el i-ésimo estado básico del sistema de n partículas, y aᵢ son coeficientes complejos.



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
Para ejecutar Observables.ipynb, asegúrate de tener instaladas las siguientes librerias:

- **NumPy**: para realizar cálculos matemáticos.

Puedes instalar las dependencias necesarias utilizando pip:

```
pip install numpy
```

### Construido con
Este proyecto fue construido con [Python 3.12](https://www.python.org/)

### Colaboradores
Laura Natalia Perilla Quintero [Lanapequin](https://github.com/Lanapequin)