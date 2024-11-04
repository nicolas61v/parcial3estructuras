# Guía de Ejecución - Métodos de Simpson con OpenMP
link Google Colab https://colab.research.google.com/drive/1pKqpEzO0nlCRp-Kj0VvdBNlnCWea2QPa?usp=sharing

## Estudiantes
- Adyuer
- Nicolás

## Instrucciones para ejecutar el código en mycompiler.io

1. **Acceder a mycompiler.io**
   - Ir a [https://www.mycompiler.io/](https://www.mycompiler.io/)
   - Click en "New Project"

2. **Configurar el entorno**
   - En el menú desplegable de lenguajes, seleccionar "C"
   - Importante: NO seleccionar C++

3. **Copiar el código**
   - Copiar todo el contenido del archivo del ultimo bloque de codigo en google coolab ya que en github no se alcanza a apreciar la diferencia entre ellos 
   - Pegarlo en el editor de mycompiler.io
   - Asegurarse de que todo el código se copió correctamente, incluyendo los includes del principio

4. **Ejecutar el código**
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

2. Si los tiempos de ejecución son 0:
   - Esto es normal para los métodos simples debido a su rapidez
   - Los métodos compuestos deberían mostrar diferencias más notables

3. Si aparece error de "undefined reference to main":
   - Verificar que todo el código se copió completamente
   - Asegurarse de que la función main() está incluida

