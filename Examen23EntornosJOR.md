# Examen Entornos de Desarrollo 
## Tema 3: Git. 05/12/23


Nombre y apellidos: Javier Otero Rodríguez 			Fecha: 05/12/2023

 

LINK DEL REPOSITORIO: https://github.com/javii-oteero/JORExamen23ED

> Vamos a crear una primera versión de una calculadora.  
> Debajo de cada ejercicio deberá aparecer capturas de pantalla pertinentes que justifiquen su realización. Intentad hacer todo lo posible desde la consola si no se indica lo contrario. 
> Se valorará negativamente las malas prácticass de GIT 

 

**1.- (0,75) Crea un repositorio en github “AAAExamen23ED“ e invítame a colaborar: "TomBort8" . AAA serán las primeras letras de tu nombre, 1er apellido y 2º apellido respectivamente.** 

<img src="https://i.ibb.co/bz1FDck/Captura-de-pantalla-2023-12-05-122412.png" alt="Captura-de-pantalla-2023-12-05-122412" border="0">

**2.- (0,75) Inicializa el repostiorio en local y vincúlalo al repostiroio de github** 

<img src="https://i.ibb.co/DGx11S6/Captura-de-pantalla-2023-12-05-122419.png" alt="Captura-de-pantalla-2023-12-05-122419" border="0">

**3.- Crea un main que pida 2 números por teclado.** 

<img src="https://i.ibb.co/kxyxPM0/Captura-de-pantalla-2023-12-05-122902.png" alt="Captura-de-pantalla-2023-12-05-122902" border="0">

```
import java.util.Scanner; 

 

public class MostrarNumeros { 

 

    public static void main(String[] args) { 

        Scanner scanner = new Scanner(System.in); 

 

        System.out.println("Por favor, ingresa el primer número:"); 

        double numero1 = scanner.nextDouble(); 

 

        System.out.println("Ahora, ingresa el segundo número:"); 

        double numero2 = scanner.nextDouble(); 

 

        System.out.println("Los números ingresados son:"); 

        System.out.println("Número 1: " + numero1); 

        System.out.println("Número 2: " + numero2); 

 

        scanner.close(); 

    } 

} 
```
> Sube los cambios al repositorio. 

<img src="https://i.ibb.co/StKTK7P/Captura-de-pantalla-2023-12-05-123013.png" alt="Captura-de-pantalla-2023-12-05-123013" border="0">

**4.- (0,2) Crea  un fichero ExplicaCalculadora.txt : “Este programa es una calculadora que va a poder realizar las operaciones básicas: sumar, restar, multiplicar y dividir”.** 

<img src="https://i.ibb.co/qj7rPYS/Captura-de-pantalla-2023-12-05-123051.png" alt="Captura-de-pantalla-2023-12-05-123051" border="0">

*  **4.1  (0,3)Crea también un fichero de texto que no debes subir a github pero debe estar dentro de la carpeta NoSubir.txt: (Este archivo debes añadirlo y quitarlo, como si te hubieras confundido). “Este archivo debe estar en la carpeta pero no subido a git”.** 

<img src="https://i.ibb.co/b1QBBFQ/Captura-de-pantalla-2023-12-05-123932.png" alt="Captura-de-pantalla-2023-12-05-123932" border="0">

> Muestra por comandos que no lo has subido 

<img src="https://i.ibb.co/n3D2xmH/Captura-de-pantalla-2023-12-05-123944.png" alt="Captura-de-pantalla-2023-12-05-123944" border="0">

> Sube los cambios al repositorio. 

<img src="https://i.ibb.co/nnKWvsy/Captura-de-pantalla-2023-12-05-124102.png" alt="Captura-de-pantalla-2023-12-05-124102" border="0">

**5.- (0,5) Muestra la diferencia entre los 2 últimos commits.** 

<img src="https://i.ibb.co/r2yY7J6/Captura-de-pantalla-2023-12-05-124556.png" alt="Captura-de-pantalla-2023-12-05-124556" border="0">

**6.- (0,5) Crea 2 ramas SUMADORES y RESTADORES** 

<img src="https://i.ibb.co/KzLcTfW/Captura-de-pantalla-2023-12-05-124732.png" alt="Captura-de-pantalla-2023-12-05-124732" border="0">

**7.- Sitúate en SUMADORES y añade al main lo siguiente:**

```
public static double sumar(double a, double b) { 

        return a + b; 

    } 
public static double multiplicar(double a, double b) { 

        return a * b; 

    } 

public static double potencia(double base, double exponente) { 

        return Math.pow(base, exponente); 

    }  
```

> Sube los cambios al repositorio.

<img src="https://i.ibb.co/THjZ17h/Captura-de-pantalla-2023-12-05-125051.png" alt="Captura-de-pantalla-2023-12-05-125051" border="0">

**8.- Sitúate en RESTADORES y añade al main lo siguiente:**

```
public static double restar(double a, double b) { 

        return a - b; 

    } 

public static double dividir(double a, double b) { 

        if (b != 0) { 

            return a / b; 

        } else { 

            throw new IllegalArgumentException("No se puede dividir por cero"); 

        } 

    } 

public static double raizCuadrada(double a) { 

        if (a >= 0) { 

            return Math.sqrt(a); 

        } else { 

            throw new IllegalArgumentException("No se puede calcular la raíz cuadrada de un número negativo"); 

        } 

    } 
```

> Sube los cambios al repositorio. 

<img src="https://i.ibb.co/CKxLzJh/Captura-de-pantalla-2023-12-05-125315.png" alt="Captura-de-pantalla-2023-12-05-125315" border="0">

**9.- (1) Muestra la diferencia entre las ramas sumadores y restadores y guárdalo en un fichero llamado DIFERENCIA _RAMAS (desde consola). Este ficehro debe subirse al repositorio.** 

<img src="https://i.ibb.co/vHYJPqQ/Captura-de-pantalla-2023-12-05-125455.png" alt="Captura-de-pantalla-2023-12-05-125455" border="0">
<img src="https://i.ibb.co/zstGT2S/Captura-de-pantalla-2023-12-05-125502.png" alt="Captura-de-pantalla-2023-12-05-125502" border="0">

<hr>

<img src="https://i.ibb.co/SRzcKmb/Captura-de-pantalla-2023-12-05-130210.png" alt="Captura-de-pantalla-2023-12-05-130210" border="0">
<img src="https://i.ibb.co/1Lx14Cb/Captura-de-pantalla-2023-12-05-130541.png" alt="Captura-de-pantalla-2023-12-05-130541" border="0">

**10.- (1,5) Fusiónalo en main (consola) y resuelve el conflicto (en gitHUB).** 

<img src="https://i.ibb.co/6Ftc2NR/Captura-de-pantalla-2023-12-05-131112.png" alt="Captura-de-pantalla-2023-12-05-131112" border="0">

<img src="https://i.ibb.co/2S1bWPT/Captura-de-pantalla-2023-12-05-131517.png" alt="Captura-de-pantalla-2023-12-05-131517" border="0">

> Sube los cambios al repositorio. 


 

**11.-(0,5) Borra las ramas SUMADORES Y RESTADORES.**

 <img src="https://i.ibb.co/0yzhMk4/Captura-de-pantalla-2023-12-05-132850.png" alt="Captura-de-pantalla-2023-12-05-132850" border="0">

**12.- (0,5) entra a SOURCETREE y haz una captura del eje temporal del repositorio. Haz una breve explicación de lo que observas.** 

 <img src="https://i.ibb.co/ftGvwTG/Captura-de-pantalla-2023-12-05-133349.png" alt="Captura-de-pantalla-2023-12-05-133349" border="0">

**13.- (1) ¿ Cuál es la diferencia entre “git pull” y “git clone” ?** 
> Git pull actualiza el repositorio online con el local, mientras que git clone "descarga" todos los archivos online en el repositorio local

**14.- (1) Abre el main y déjalo inservible. Sube los cambios. Deshaz el último commit.**
 
 <img src="https://i.ibb.co/b3hLZ8K/Captura-de-pantalla-2023-12-05-133855.png" alt="Captura-de-pantalla-2023-12-05-133855" border="0">
 <img src="https://i.ibb.co/PgXLL7G/Captura-de-pantalla-2023-12-05-134122.png" alt="Captura-de-pantalla-2023-12-05-134122" border="0">

**15.- (1) Vuelve al estado en el que estaba el proyecto al acabar el ejercicio 3 en local.**

<img src="https://i.ibb.co/W58sKMT/Captura-de-pantalla-2023-12-05-134338.png" alt="Captura-de-pantalla-2023-12-05-134338" border="0">


 
 
 **16.-(0,5) Añade este documento al repoitorio, con todas las imágenes para que se pueda ver desde git.**
 
 <img src="https://i.ibb.co/1v3hTCx/Captura-de-pantalla-2023-12-05-134543.png" alt="Captura-de-pantalla-2023-12-05-134543" border="0">


**17.- Por último, ejecutad el siguiente comando:** 

> *history > historial.txt* 

**sube el resultado a aules junto al PDF de este documento.** 