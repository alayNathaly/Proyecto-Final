Definir res, n1, n2, A, B, C, matriz Como real;
    Definir opcion como entero;
    Definir impar Como Logico;
    Escribir "1. Calcular una suma: ";
    Escribir "2. Calcular una resta: ";
    Escribir "3. Calcular una multiplicacion: ";
    Escribir "4. Calcular una division: ";
    Escribir "5. Calcular la suma de todos los valores de la matriz: ";
    Escribir "6. Calcular la resta de todos los valores de la matriz: ";
    Escribir "7. Calcular la suma de matrices: ";
    Escribir "8. Calcular la resta de matrices: ";
    Escribir "9. Realizar un triangulo con números impares: ";
    Escribir "10. Realizar un rectangulo con asteriscos: ";
    Escribir "11. Realizar un cuadrado con asteriscos: ";

    Escribir "Escriba su opcion: ";
    leer opcion;
    
    Segun opcion hacer
        1: Escribir "Ingrese numero 1: ";
            leer n1;
            Escribir "Ingrese numero 2: ";
            leer n2;
            res= n1+n2;
            Escribir "El total de la suma es: " res;
            
        2: Escribir "Ingrese numero 1: ";
            leer n1;
            Escribir "Ingrese numero 2: ";
            leer n2;
            res= n1-n2;
            Escribir "El total de la resta es: " res;
            
        3: Escribir "Ingrese numero 1: ";
            leer n1;
            Escribir "Ingrese numero 2: ";
            leer n2;
            res= n1*n2;
            Escribir "El total de la multiplicacion es: " res;
            
        4: Escribir "Ingrese numero 1: ";
            leer n1;
            Escribir "Ingrese numero 2: ";
            leer n2;
            res= n1/n2;
            Escribir "El total de la division es: " res;
            
        5: // Calcular la suma de todos los valores de la matriz
            Dimension matriz[100, 100];
            Definir filas, columnas, i, j como Entero;
            Definir suma como real;
            suma = 0;
            
            Escribir "Ingrese el número de filas de la matriz: ";
            Leer filas;
            Escribir "Ingrese el número de columnas de la matriz: ";
            Leer columnas;
            
            Escribir "Ingrese los elementos de la matriz:";
            Para i <- 1 Hasta filas Hacer;
                Para j <- 1 Hasta columnas Hacer;
                    Escribir "Ingrese el elemento [", i, ",", j, "]: ";
                    Leer matriz[i, j];
                    suma = suma + matriz[i, j];
                FinPara
            FinPara
            
            Escribir "La suma de todos los valores de la matriz es: ", suma;
			
        6: // Calcular la resta de todos los valores de la matriz
            Dimension matriz[100, 100];
            Definir filas, columnas, i, j como Entero;
            Definir resta como real;
            resta = 0;
            
            Escribir "Ingrese el número de filas de la matriz: ";
            Leer filas;
            Escribir "Ingrese el número de columnas de la matriz: ";
            Leer columnas;
            
            Escribir "Ingrese los elementos de la matriz:";
            Para i <- 1 Hasta filas Hacer;
                Para j <- 1 Hasta columnas Hacer;
                    Escribir "Ingrese el elemento [", i, ",", j, "]: ";
                    Leer matriz[i, j];
                    resta = resta-matriz[i, j];
                FinPara
            FinPara
            
            Escribir "La resta de todos los valores de la matriz es: ", resta;
			
        7: // Calcular la suma de matrices
            Dimension A[100, 100];  // Matriz A
            Dimension B[100, 100];  // Matriz B
            Dimension C[100, 100];  // Matriz resultado
            Definir filas, columnas, i, j como Entero;  
            
            Escribir "Ingrese el número de filas de las matrices: ";
            Leer filas;
            Escribir "Ingrese el número de columnas de las matrices: ";
            Leer columnas;
            
            Escribir "Ingrese los elementos de la matriz A:";
            Para i <- 1 Hasta filas Hacer;
                Para j <- 1 Hasta columnas Hacer;
                    Escribir "Ingrese el elemento A[", i, ",", j, "]: ";
                    Leer A[i, j];
                FinPara
            FinPara
            
            Escribir "Ingrese los elementos de la matriz B:";
            Para i <- 1 Hasta filas Hacer;
                Para j <- 1 Hasta columnas Hacer;
                    Escribir "Ingrese el elemento B[", i, ",", j, "]: ";
                    Leer B[i, j];
                FinPara
            FinPara
            
            // Sumar las matrices A y B
            Para i <- 1 Hasta filas Hacer;
                Para j <- 1 Hasta columnas Hacer;
                    C[i, j] = A[i, j] + B[i, j];
                FinPara
            FinPara
            
            Escribir "El resultadao de la suma de matrices es: ";
            Para i <-1 Hasta filas Hacer;
                Para j <- 1 Hasta columnas Hacer;
                    Escribir sin saltar C[i , j ];
                FinPara
                Escribir "  ";
            FinPara
			
        8: // Calcular la resta de matrices
            Dimension A[100, 100];  // Matriz A
            Dimension B[100, 100];  // Matriz B
            Dimension C[100, 100];  // Matriz resultado
            Definir filas, columnas, i, j como Entero;  
            
            Escribir "Ingrese el número de filas de las matrices: ";
            Leer filas;
            Escribir "Ingrese el número de columnas de las matrices: ";
            Leer columnas;
            
            Escribir "Ingrese los elementos de la matriz A:";
            Para i <- 1 Hasta filas Hacer;
                Para j <-1 Hasta columnas Hacer;
                    Escribir "Ingrese el elemento A[", i, ",", j, "]: ";
                    Leer A[i, j];
                FinPara
            FinPara
            
            Escribir "Ingrese los elementos de la matriz B:";
            Para i <- 1 Hasta filas Hacer;
                Para j <- 1 Hasta columnas Hacer;
                    Escribir "Ingrese el elemento B[", i, ",", j, "]: ";
                    Leer B[i, j];
                FinPara
            FinPara
            
            // Restar las matrices A y B
            Para i <-1 Hasta filas Hacer;
                Para j <- 1 Hasta columnas Hacer;
                    C[i, j] = A[i, j] - B[i, j];
                FinPara
            FinPara
            
            Escribir "El resultado de la resta de matrices es:";
            Para i<-1 Hasta filas Hacer;
                Para j<- 1 Hasta columnas Hacer;
                    Escribir sin saltar C[i, j];
                FinPara
                Escribir " ";
            FinPara
            
        9: Definir num, i, j como entero;
            Escribir "Ingrese un numero entero: ";
            leer num;
            Para i<-0 Hasta num - 1 con paso 1 Hacer;
                Para j <-0 Hasta i con paso 1 Hacer;
                    Escribir sin saltar (2 * j + 1); 
                FinPara
                Escribir "";
            FinPara
			
        10: Definir i, j, alto, ancho como entero;
			Escribir "Ingrese el alto del rectangulo: ";
		    leer alto;
			Escribir "Ingrese el ancho del rectangulo: ";
			leer ancho;
			Para i<-1 hasta alto con paso 1 hacer;
				para j<-1 hasta alto con paso 1 hacer;
					escribir sin saltar "*";
					para j<-2 hasta ancho con paso 1 hacer;
						escribir sin saltar " *";
						
					FinPara
					Escribir "";
				FinPara
				
			FinPara
			
		11: Definir num, i, j como entero;
			Escribir "Ingrese un numero para el cuadrado: ";
			Leer num;
			para i<-1 hasta num con paso 1 hacer;
				para j<-1 hasta  num con paso 1 hacer;
					si i>1 y i<num y j>1 y j<num entonces;
						escribir Sin Saltar "  ";
					sino escribir sin saltar"* ";
					FinSi
				FinPara
				Escribir "";
			FinPara
    FinSegun