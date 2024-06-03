#include <stdio.h> // Librería de funciones

int main() {
    // SUMA DE LOS DIGITOS DE UN NUMERO
    int num1 = 123; // Inicializa el número
    int sum1 = 0; // Inicializa la suma
    int n = num1; // Copia el número

        while (n > 0) {
            sum1 += n % 10; // Suma el último dígito
            n /= 10; // Elimina el último dígito
        }
        printf("La suma de los digitos es: %d\n", sum1);

    // INVERSO DE UN NUMERO
    int num2 = 123456; // Inicializa el número
    int inver = 0; // Inicializa el inverso

        while (num2 != 0) {
            inver = inver * 10 + num2 % 10; // Añade el último dígito al inverso
            num2 /= 10; // Elimina el último dígito
        }
        printf("El inverso del numero es: %d\n", inver);

    // POTENCIA DE UN NUMERO
    int base = 3; // Base
    int exp = 3; // Exponente
    int rs = 1; // Resultado
    int i = 0; // Contador

        while (i < exp) {
            int sum2 = 0; // Suma temporal
            int j = 0; // Contador interno

            while (j < base) {
                sum2 += rs; // Suma acumulada
                j++;
            }
            rs = sum2; // Actualiza el resultado
            i++;
        }
        printf("El resultado de %d^%d es: %d\n", base, exp, rs);

    // RADICACION MEDIANTE RESTAS SUCESIVAS
    int nu6 = 27; // Número fijo
    int x = 3; // Índice de la raíz
    int res = 0; // Resultado
    int x1 = 1; // Contador

        while (nu6 > 0) {
            res++; // Incrementa el resultado
            nu6 -= res; // Resta el resultado del número
            x1++;
        }
        printf("La raiz %d es: %d\n", x, res - 1);

    // SERIE FIBONACCI
    int num3 = 10; // Número de términos
    int a = 0, b = 1; // Primeros dos términos
    printf("Serie de Fibonacci: %d %d", a, b);
    int k = 2; // Contador

        while (k < num3) {
            int next = a + b; // Siguiente término
            printf(" %d", next);
            a = b; // Actualiza a
            b = next; // Actualiza b
            k++;
        }
        printf("\n");

    // FACTORIAL DE UN NUMERO
    int fac = 1; // Inicializa el factorial
    int num4 = 5; // Número
    int l = 1; // Contador

        while (l <= num4) {
            fac *= l; // Multiplica el contador
            l++;
        }
        printf("El factorial de %d es: %d\n", num4, fac);

    // SUMA DE UNA SERIE ARITMÉTICA
    int num5 = 10; // Número fijo
    int sum5 = 0; // Inicializa la suma
    int o = 1; // Contador

        while (o <= num5) {
            sum5 += o; // Suma el contador
            o++;
        }
        printf("La suma de la serie aritmetica es: %d\n", sum5);

    // PRODUCTO DE UNA SERIE GEOMÉTRICA
    int num6 = 5; // Número fijo
    int a1 = 2; // Primer término
    int r = 2; // Razón común
    int prod = 1; // Producto
    int p = 0; // Contador

        while (p < num6) {
            prod *= a1; // Multiplica el término actual
            a1 *= r; // Actualiza el término
            p++;
        }
        printf("El producto de la serie geometrica es: %d\n", prod);

    // NÚMERO DE DÍGITOS DE UN NÚMERO
    int num7 = 123; // Número fijo
    int con = 0; // Contador

        while (num7 != 0) {
            num7 /= 10; // Elimina el último dígito
            con++; // Incrementa el contador
        }
        printf("El numero tiene %d digitos\n", con);

    // VERIFICAR SI UN NÚMERO ES PRIMO
    int num = 29; // Número fijo
    int iprimo = 1; // Inicializa como primo
    int ip = 2; // Contador

        while (ip <= num / 2) {
            if (num % ip == 0) {
                iprimo = 0; // No es primo
                break;
            }
            ip++;
        }

        if (iprimo) {
            printf("%d es primo\n", num);
        } else {
            printf("%d no es primo\n", num);
        }

    // ENCONTRAR EL MCD (Máximo Común Divisor)
    int a2 = 54; // Número fijo
    int b2 = 24; // Número fijo

        while (a2 != b2) {
            if (a2 > b2) {
                a2 -= b2; // Resta el menor del mayor
            } else {
                b2 -= a2; // Resta el menor del mayor
            }
        }
        printf("El MCD es: %d\n", a2);

    // SUMAR LOS NÚMEROS IMPARES HASTA N
    int num8 = 10; // Número fijo
    int sum8 = 0; // Suma
    int q = 1; // Contador

        while (q <= num8) {
            sum8 += q; // Suma el contador
            q += 2; // Incrementa por 2
        }
        printf("La suma de los numeros impares hasta %d es: %d\n", num8, sum8);

    // SUMAR LOS NÚMEROS PARES HASTA N
    int num9 = 10; // Número fijo
    int sum9 = 0; // Suma
    int w = 0; // Contador

        while (w <= num9) {
            sum9 += w; // Suma el contador
            w += 2; // Incrementa por 2
        }
        printf("La suma de los numeros pares hasta %d es: %d\n", num9, sum9);

    // SUMA DE LOS CUADRADOS DE LOS PRIMEROS N NÚMEROS
    int nu1 = 5; // Número fijo
    int su1 = 0; // Suma
    int e = 1; // Contador
        while (e <= nu1) {
            su1 += e * e; // Suma el cuadrado
            e++;
        }
        printf("La suma de los cuadrados de los primeros %d numeros es: %d\n", nu1, su1);

    // SUMA DE LOS CUBOS DE LOS PRIMEROS N NÚMEROS
    int nu2 = 4; // Número fijo
    int su2 = 0; // Suma
    int t = 1; // Contador

        while (t <= nu2) {
            su2 += t * t * t; // Suma el cubo
            t++;
        }
        printf("La suma de los cubos de los primeros %d numeros es: %d\n", nu2, su2);

    // SUMA DE UNA SERIE DE NÚMEROS FRACCIONARIOS
    int nu3 = 5; // Número fijo
    float su3 = 0.0; // Suma
    int u = 1; // Contador

        while (u <= nu3) {
            su3 += 1.0 / u; // Suma el recíproco
            u++;
        }
        printf("La suma de la serie fraccionaria es: %.2f\n", su3);

    // PRODUCTO DE UNA SERIE DE NÚMEROS FRACCIONARIOS
    int nu4 = 5; // Número fijo
    float prod4 = 1.0; // Producto
    int d = 1; // Contador

        while (d <= nu4) {
            prod4 *= 1.0 / d; // Multiplica el recíproco
            d++;
        }
        printf("El producto de la serie fraccionaria es: %.6f\n", prod4);

    // CONTAR LOS NÚMEROS PRIMOS HASTA N
    int nx = 20; // Número fijo
    int cont2 = 0; // Contador de primos
    int px = 2; // Contador

        while (px <= nx) {
            int ipri = 1; // Inicializa como primo
            int j = 2; // Contador interno

            while (j <= px / 2) {
                if (px % j == 0) {
                    ipri = 0; // No es primo
                    break;
                }
                j++;
            }
            if (ipri) {
                cont2++; // Incrementa el contador de primos
            }
            px++;
        }
        printf("Hay %d numeros primos hasta %d\n", cont2, nx);

    // CALCULAR EL N-ÉSIMO NÚMERO TRIANGULAR
    int nu5 = 7; // Número fijo
    int tri = 0; // Suma
    int f = 1; // Contador

        while (f <= nu5) {
            tri += f; // Suma el contador
            f++;
        }
        printf("El %d-esimo numero triangular es: %d\n", nu5, tri);

    // CALCULAR LA SUMA DE LOS FACTORIALES DE LOS PRIMEROS N NÚMEROS
    int nx1 = 5; // Número fijo
    int sx = 0; // Suma
    int fx = 1; // Contador

        while (fx <= nx1) {
            int facx = 1; // Factorial temporal
            int j = 1; // Contador interno

            while (j <= fx) {
                facx *= j; // Calcula el factorial
                j++;
            }
            sx += facx; // Suma el factorial
            fx++;
        }
        printf("La suma de los factoriales de los primeros %d numeros es: %d\n", nx1, sx);

    return 0;
}
