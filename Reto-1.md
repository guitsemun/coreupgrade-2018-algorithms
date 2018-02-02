## 1. ¿Cual es la complejidad de tiempo de la función example()?

```c++
int example(int n)
{
  int count = 0;
  for (int i = n; i > 0; i /= 2)
     for (int j = 0; j < i; j++)
        count += 1;
  return count;
}
```
La complejidad de este algoritmo es O(n) debido a que en el bucle interno se tiene que "j<i esto quiere decir que j<n" . Se observa que en el bucle externo se tiene una complejidad de O(logn); pero para definir la complejidad manda el bucle interno. Tanto el bucle interno y externo logran el mismo numero de interacciones.

## 2. ¿Cual es la complejidad de tiempo de la función example2()?

```c++
void example2(int n, int arr[])
{
    int i = 0, j = 0;
    for(; i < n; ++i)
        while(j < n && arr[i] < arr[j])
            j++;
}
```
La complejidad de este algoritmo es O(n) debido a que j solo se diferencia i por 1; esto quiere decir que cada vez que incremente j, incrementa i. Por lo tanto se nota que el numero de ejecuciones del ciclo while es igual al del ciclo for.

## 3. ¿Cuál es la mejor complejidad de tiempo de bubbleSort?

Es la ordenación de un vector ya ordenado. En este caso el número de comparaciones será el mismo que en cualquier otro caso n^2

