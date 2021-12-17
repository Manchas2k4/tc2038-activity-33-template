![Tec de Monterrey](images/logotecmty.png)
# Actividad 3.3 Implementación de "Knapsack problem"

## <span style="color: rgb(26, 99, 169);">¿Qué tengo que hacer?</span>
En este repositorio encontrarás el archivo "main.cpp". En este archivo deberás desarrollar la implementación del problema presentado en esta actividad.  En la parte superior del archivo coloca, en comentarios, tus datos. Por ejemplo:
```
// =========================================================
// File: main.cpp
// Authors:
//  Edward Elric - A00123456
//  Alphonse Elric - A00124598
// Date: 01/01/2021
// =========================================================
```
Implementa, <span style="text-decoration-line: underline;">en equipos de 2 personas (máximo)</span>, una solución para el problema que se describe a continuación. El problema fue tomado del siguiente sitio: [10664 Luggage](https://onlinejudge.org/external/106/10664.pdf).

## <span style="color: rgb(26, 99, 169);">**Descripción**</span>
Peter y sus amigos están de vacaciones, por lo que han decidido hacer un viaje en coche para conocer el norte de España. Son siete personas y piensan que dos coches son suficientes para su equipaje.

Es hora de irse ... y un montón de maletas esperan fuera de los autos. Los conductores no se ponen de acuerdo sobre qué maleta se debe meter en cada maletero, porque nadie quiere que un maletero cargue más peso que el otro. ¿Es posible que las dos botas carguen con el mismo peso? (¡Obviamente sin desempacar las maletas!)

Considere m conjuntos de números que representan el peso de las maletas, debe decidir para cada uno, si es posible distribuir las maletas en los maleteros, y los dos maleteros pesan lo mismo.

## <span style="color: rgb(26, 99, 169);">**Entrada**</span>
La primera línea de la entrada contiene un número entero, *m*, que indica el número de casos de prueba. Para cada caso de prueba, hay una línea que contiene *n* números enteros (1 <= *n* <= 20) separados por espacios simples. Estos números enteros son los pesos de cada maleta. La suma total de los pesos de todas las maletas es menor o igual a 200 kilogramos.

## <span style="color: rgb(26, 99, 169);">**Salida**</span>
La salida consta de m líneas. La *i*-ésima línea corresponde al *i*-ésimo conjunto de peso de maletas y contiene la cadena "YES" o "NO", dependiendo de la posibilidad de que los dos maleteros carguen con el mismo peso para el caso de prueba respectivo.

## <span style="color: rgb(26, 99, 169);">**Ejemplo de entrada**</span>
```
3
1 2 1 2 1
2 3 4 1 2 5 10 50 3 50
3 5 2 7 1 7 5 2 8 9 1 25 15 8 3 1 38 45 8 1
```

## <span style="color: rgb(26, 99, 169);">**Ejemplo de salida**</span>
```
NO
YES
YES

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
