# Guía de Ejecución - Métodos de Simpson con OpenMP

## Estudiantes
- Adyuer
- Nicolás

## Instrucciones para ejecutar el código en mycompiler.io

1. **Acceder a mycompiler.io**
   - Ir a [https://www.mycompiler.io/](https://www.mycompiler.io/)
   - Click en "New Project"

2. **Configurar el entorno**
   - En el menú desplegable de lenguajes, seleccionar "C"
   - Importante: ¡NO seleccionar C++!

3. **Copiar el código**
   - Copiar todo el contenido del archivo `simpson_methods.c` 
   - Pegarlo en el editor de mycompiler.io
   - Asegurarse de que todo el código se copió correctamente, incluyendo los includes del principio

4. **Configurar la compilación**
   - Click en el botón de configuración (icono de engranaje ⚙️)
   - En "Compiler flags", pegar exactamente:
     ```
     gcc -fopenmp $fileName -o $fileNameWithoutExt -lm
     ```
   - Esta configuración es crucial para que OpenMP funcione correctamente

5. **Ejecutar el código**
   - Click en el botón "Run" (o usar F9)
   - Los resultados aparecerán en la consola de salida

## Resultados esperados

El programa mostrará los tiempos de ejecución y resultados para:
- Simpson 1/3 Simple (Secuencial y Paralelo)
- Simpson 3/8 Simple (Secuencial y Paralelo)
- Simpson 1/3 Compuesto (Secuencial y Paralelo)
- Simpson 3/8 Compuesto (Secuencial y Paralelo)

## Solución de problemas comunes

1. Si aparece error de "undefined reference to omp_get_wtime":
   - Verificar que seleccionó C y no C++
   - Verificar que las flags de compilación están exactamente como se indicó

2. Si los tiempos de ejecución son 0:
   - Esto es normal para los métodos simples debido a su rapidez
   - Los métodos compuestos deberían mostrar diferencias más notables

3. Si aparece error de "undefined reference to main":
   - Verificar que todo el código se copió completamente
   - Asegurarse de que la función main() está incluida

## Notas adicionales

- El código utiliza n = 1000000 subintervalos para los métodos compuestos
- La función a integrar es f(x) = e^(-x^2)
- El intervalo de integración es [-1, 1]

Si tiene alguna duda o problema con la ejecución, no dude en contactarnos.
