![Tec de Monterrey](images/logotecmty.png)
# Actividad 3.2 Implementación de "Dijkstra and Floyd"

## <span style="color: rgb(26, 99, 169);">¿Qué tengo que hacer?</span>
Accede a la siguiente liga: [Actividad Integradora 1](https://classroom.github.com/a/n5fs_Sy0) y acepta la tarea. Esto creará tu repositorio de trabajo. En él, encontrarás el archivo "main.cpp". En este archivo deberás desarrollar la implementación del problema presentado en esta actividad.  En la parte superior del archivo coloca, en comentarios, tus datos. Por
```
// =========================================================
// File: main.cpp
// Authors:
//  Edward Elric - A00123456
//  Alphonse Elric - A00124598
// Date: 01/01/2021
// =========================================================
```
Implementa, <span style="text-decoration-line: underline;">en equipos de 2 personas (máximo)</span>, una solución para el problema que se describe a continuación.

## <span style="color: rgb(26, 99, 169);">**Descripción**</span>
Desarrolla un programa en C++ que implementa los algoritmos de Dijkstra y Floyd para encontrar la distancia más corta entre un par de vértices en un grado dirigido.

## <span style="color: rgb(26, 99, 169);">**Entrada**</span>
El programa recibe un número entero, *N*, seguido de *N* x *N* valores enteros que representan una matriz de adyacencia de un grafo dirigido. El primer número, *N*, representa el número de nodos. Los siguientes valores representan los valores en la matriz. El valor en la posición ()*i*, *j*) representa el peso del arco del nodo *i* al nodo *j*. Si no hay un arco entre el nodo *i* y el nodo *j*¨, el valor en la matriz será -1.

## <span style="color: rgb(26, 99, 169);">**Salida**</span>
La salida del programa es, primerocon el resultado del algoritmo de Dijkstra, la distancia del nodo *i* al nodo *j* para todos los nodos. A continuación, se debe mostrar la matriz resultado del algoritmo de Flyod.

## <span style="color: rgb(26, 99, 169);">**Ejemplo de entrada**</span>
```
4
0 2 -1 3
-1 0 1 5
2 3 0 -1
3 -1 4 0
```

## <span style="color: rgb(26, 99, 169);">**Ejemplo de salida**</span>
```
Dijkstra :
node 1 to node 2 : 2
node 1 to node 3 : 3
node 1 to node 4 : 3
node 2 to node 1 : 3
node 2 to node 3 : 1
node 2 to node 4 : 5
node 3 to node 1 : 2
node 3 to node 2 : 3
node 3 to node 4 : 5
node 4 to node 1 : 3
node 4 to node 2 : 5
node 4 to node 3 : 4

Floyd :
0 2 3 3
3 0 1 5
2 3 0 5
3 5 4 0

```

Para probar tu implementación, compila tu programa con el comando:
```
g++ -std=c++11 main.cpp -o app
```
Posteriormente, ejecuta tu programa. Para realizar las pruebas, puedes usar las siguientes líneas de código.
```
./app < inputX.txt > mysolutionX.txt
diff mysolutionX.txt outputX.txt
```
Si el segundo comando no tiene ninguna salida, los resultados que obtuviste son los esperados.

## <span style="color: rgb(26, 99, 169);">**¿Bajo qué criterios se evalúa mi evidencia?**</span>

- **80%** - Para cada una de las funcionalidades se evaluará:

    - **Excelente (80%)** - pasa correctamente todos los casos de prueba.
    - **Muy Bien (60%)** - pasa correctamente el 75% de los casos de prueba.
    - **Bien (40%)** - pasa correctamente el 50% de los casos de prueba.
    - **Insuficiente (20%)** - pasa correctamente menos del 50% de los casos de prueba.

- **10%** - El código deberá seguir los lineamientos estipulados en el estándar de codificación: <span class="instructure_file_holder link_holder">[liga_estándar_codificación](estandar.pdf)</span>
- **10%** - Se especifica (en comentarios) la complejidad computacional de cada uno de las funciones desarrolladas.

## <span style="color: rgb(26, 99, 169);">**¿Dónde la entrego?**</span>
Cuando hayas pasado todas las pruebas, recuerda publicar el código en tu repositorio (*git push*).

## <span style="color: rgb(26, 99, 169);">**Importante**</span>
Recuerda colocar el nombre y las matrículas de ambos integrantes en en los comentarios iniciales. En caso de que se incumpla este punto, se penalizará con 20 puntos sobre la calificación obtenida.
