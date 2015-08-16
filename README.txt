# ESPAI-Hoja5


Ejercicios capítulo 5

1. ¿Qué es una función?
2. ¿En qué 2 partes podemos dividir una función?
Explica también que objetivo cumple cada una de ellas.
3. ¿Qué diferencia hay entre variables globales y locales? ¿Qué ventajas e inconvenientes tiene cada
una de ellas?
4. Dado el siguiente código
#include <iostream>
using namespace std;
int sumar (int a, int b);
int z = 0;
int main() {
int x = 7;
int y = 8;
z = sumar(x, y);
cout << "z=" << z << endl;
return 0;
}
int sumar (int a, int b)
{
int c = 0;
c = a + b;
return c;
}

a. Localiza las variables globales, locales y parámetros que estamos utilizando.
b. ¿Cuál es el retorno de esta función?
c. En caso de definir una funcion restar, ¿qué variables de las definidas hasta ahora podríamos ver
desde la nueva función?
d. Cómo podríamos hacer que el valor por defecto de a y b fuera 0?


5. Revisa el siguiente programa

#include <iostream>
using namespace std;
int sumar (int a, int b);
int sumar (int c, int d);
float sumar (int c, float d);
int sumar (int a, int b, int c);
int z = 0;
int main() {
int x = 7;
int y = 8;
int z2 = 0;
z = sumar(x, y);
cout << "z=" << z << endl;
z2 = sumar(15, 12.7f);
cout << "z2=" << z2 << endl;
return 0;
}
int sumar (int a, int b)
{
int c = 0;
c = a + b;
return c;
}
float sumar (int a, float b)
{
float c = 0;
c = a + b;
return c;
}
int sumar (int a, int b, int c)
{
int d = 0;
d = a + b + c;
return d;
}

a. ¿Falta o sobra alguna definición de funcion en la cabecera? ¿Qué opinas de las 2 primeras?
b. Cómo sabe el programa qué funcion de todas ellas utilizar, si se llaman igual?
c. Cuál será la salida de esta aplicación?
d. ¿Cómo harías otra funcion de sobrecarga que recibiera 3 parámetros float, y retornara un int?;

6. Encuentra el error en el siguiente código, y expica cómo lo solucionarías.

#include <iostream>
using namespace std;
void sumar (int a, int b);
int z = 0;
int main() {
int x = 7;
int y = 8;
int z2 = 0;
z = sumar(x, y);
cout << "z=" << z << endl;
return 0;
}
void sumar (int a, int b)
{
int c = 0;
c = a + b;
return c;
}

7. ¿Para qué sirve la palabra clave inline?

8. Práctica final del capítulo
Haz un programa que nos permita calcular la suma, resta, multiplicación y división de 2 números
que nos proporcionará el usuario. Utiliza para ello funciones.
Crea un menú donde el usuario pueda escoger la operación, de esta manera:
1. Suma
2. Resta
3. Multiplicación
4. División
