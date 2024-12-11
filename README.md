# Beam Search

## Introducción
**Beam Search** es un algoritmo de búsqueda heurística diseñado para encontrar la solución más probable en un conjunto de nodos. Este algoritmo expande únicamente los nodos con mayor probabilidad, siendo especialmente útil en modelos secuenciales donde el orden de las decisiones importa.

El algoritmo comienza en un nodo inicial y genera todos sus hijos posibles. A cada hijo se le asigna un valor heurístico y se seleccionan los *N* mejores, definidos por el parámetro llamado *beam width*. Este proceso se repite iterativamente hasta encontrar el camino con la mayor puntuación global.

## Diferencias con Naive Search
A diferencia del algoritmo **Naive Search**, que expande todos los nodos posibles, **Beam Search** se enfoca solo en aquellos nodos que tienen el mejor valor heurístico dentro del ancho de búsqueda (*beam width*). Aunque esto reduce drásticamente el espacio de búsqueda, no garantiza encontrar la solución óptima en todos los casos.

### Ejemplo conceptual
Si programamos un traductor con **Naive Search**, cada palabra de un idioma como el español (con miles de palabras en su vocabulario) podría expandir todos los nodos posibles. Esto resultaría en un tiempo de computación elevado y generaría combinaciones innecesarias. En contraste, **Beam Search** limita la expansión a los nodos más prometedores según el modelo heurístico, optimizando el proceso.

---

## Ejemplos Gráficos
### Representación visual del algoritmo
Un diagrama que representa el funcionamiento de **Beam Search** comparado con **Naive Search**:

- **Beam Search**: Solo expande nodos seleccionados según el valor heurístico.
- **Naive Search**: Expande todos los nodos sin restricciones.

*(Diagrama en preparación: incluir una gráfica de árbol que ilustre el proceso.)*

---
