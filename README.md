![Tec de Monterrey](images/logotecmty.png)
# Act 1.3 - Actividad Integral de Conceptos Básicos y Algoritmos Fundamentales (Evidencia Competencia)

## <span style="color: rgb(26, 99, 169);">¿Qué tengo que hacer?</span>
En este repositorio encontrarás los archivos de entrada, así como las salidas esperadas que podrás usar para probar tu implementación. También encontrarás un archivo "main.cpp". Ahí deberás implementar tu solución. En el archivo deberás colocar en la parte superior, en comentarios, tus datos. Por ejemplo:
```
// =========================================================
// File: main.cpp
// Author: Edward Elric - A00123456
// Date: 01/01/2021
// =========================================================
```
<span style="text-decoration: underline;">De manera individual</span>, desarrolla la solución del siguiente problema:

El canal de Suez es un canal navegable que conecta el mar Mediterráneo con el mar Rojo a través de alrededor de 190 km, uniendo por un el lado del mar Mediterráneo desde el puerto Said hasta el golfo de Suez en el mar Rojo. Este canal es navegado entre 49 y 97 barcos diariamente. Se tiene un registro de los barcos que navegan por el canal con el siguiente formato:
```
<fecha> <hora> <punto-entrada> <UBI-Identificador único del buque>
```
Ejemplo:
```
03-01-20 13:45 M 8PAK7
```
Donde:
* El punto de entrada puede ser **M – Mar Mediterráneo** y **R – Mar Rojo**.
* La fecha estará entre **01-ENE-2020** y **31-DIC-2020**.
* El tiempo estará en formato de 24 Hrs.

## <span style="color: rgb(26, 99, 169);">**Entrada**</span>
La primera línea de entrada contiene dos elementos: un entero *n*, el número de barcos que ha entrado al canal, y una cadena de 3 tres caracteres *prefix*, el prefijo del UBI a búscar. Las siguientes *n* líneas; contiene el registro de los barcos que han entrado al canal con el formato descrito anteriormente.

## <span style="color: rgb(26, 99, 169);">**Salida**</span>
Deberás desplegar sólo los registros cuyo UBI empiece con *prefix*, ordenados por fecha.

## <span style="color: rgb(26, 99, 169);">**Ejemplo de entrada**</span>
```
16 2HU
01-01-20 00:17 R 2HUN5
01-01-20 00:37 R 2AET2
01-01-20 00:57 M 2HUQ5
01-01-20 01:17 M 2FRW0
01-01-20 01:37 M 4MXV8
01-01-20 01:57 R 2HUG7
01-01-20 02:17 R 1KIH9
01-01-20 02:37 R 2HUX2
01-01-20 02:57 M 3CFE2
01-01-20 03:17 R 1TLD0
01-01-20 03:37 R 3FRF4
01-01-20 03:57 R 2HUK8
01-01-20 04:17 M 0CFR7
01-01-20 04:37 R 0TQL9
01-01-20 04:57 R 2HUS4
01-01-20 05:17 R 0FRX0
```

## <span style="color: rgb(26, 99, 169);">**Ejemplo de salida**</span>
```
01-01-20 00:17 R 2HUN5
01-01-20 00:57 M 2HUQ5
01-01-20 01:57 R 2HUG7
01-01-20 02:37 R 2HUX2
01-01-20 03:57 R 2HUK8
01-01-20 04:57 R 2HUS4
```

Para probar tu implementación, compila tu programa con el comando:
```
g++ -std=c++11 main.cpp -o app
```
Posteriormente, prueba con cada uno de los archivos de entrada de prueba que encontrarás en este repositorio (input1.txt, input2.txt, input3.txt, input4.txt). Los resultados que debes obtener se encuentran en los archivos llamados output1.txt, output1.txt, output1.txt y output1.txt. Para realizar las pruebas, puedes usar las siguientes líneas de código. Por ejemplo, si queremos probar con el archivo de prueba "input1.txt".
```
./app < input1.txt > mysolution1.txt
diff mysolution1.txt output1.txt
```
Si el segundo comando no tenga ninguna salida, sabrás que los resultados que obtuviste son los esperados. Recuerda actualizar tu repositorio (*git push*) cuando hayas terminado tu implementación.

Por último, realiza una investigación y reflexión en forma individual de la importancia y eficiencia del uso de los diferentes algoritmos de ordenamiento y búsqueda en una situación problema de esta naturaleza, generando un documento llamado **"ReflexAct1.3.pdf"**

## <span style="color: rgb(26, 99, 169);">**¿Bajo qué criterios se evalúa mi evidencia?**</span>

- **80%** - Para cada una de las funcionalidades se evaluará:

    - **Excelente (80%)** - pasa correctamente todos los casos de prueba.
    - **Muy Bien (60%)** - pasa correctamente el 75% de los casos de prueba.
    - **Bien (40%)** - pasa correctamente el 50% de los casos de prueba.
    - **Insuficiente (20%)** - pasa correctamente menos del 50% de los casos de prueba.


- **10%** - El código deberá seguir los lineamientos estipulados en el estándar de codificación: <span class="instructure_file_holder link_holder">[liga_estándar_codificación](estandar.pdf)</span>
- **10%** - Se respetenan los nombres de las funciones en la aplicación.

## <span style="color: rgb(26, 99, 169);">**¿Dónde la entrego?**</span>
Esta actividad forma parte tanto de tu calificación final del curso, así como del portafolio de evidencias de las competencias a desarrollar del curso, por lo que se te pide que en forma individual:
* Realices una entrega de  los archivos correspondientes de los algoritmos de ordenamiento y búsqueda, en la sección correspondiente dentro de esta plataforma, así como el documento de reflexión individual (**ReflexAct1.3.pdf**).
* Generes una carpeta en forma personal llamada **TC1031(Portafolio_Final)** que servirá como preparación para la entrega del portafolio de competencias que se realizará al final del curso, esta carpeta debe contener 5 carpetas:
    * **Act1.3** - coloca aquí tus archivos que solucionaron la <span style="text-decoration: underline;">actividad 1.3</span> así como el documento de reflexión individual (**ReflexAct1.3.pdf**).
    * Act2.3
    * Act3.4
    * Act4.3
    * Act5.2
