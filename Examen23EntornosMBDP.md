# Examen Entornos de Desarrollo 
## Tema 3: Git. 05/12/23


Nombre y apellidos: Miguel Bayona De Pablo<br> 			Fecha:05/12/2023

 

LINK DEL REPOSITORIO: <a href="">repositorio</a> 

> Vamos a crear una primera versión de una calculadora.  
> Debajo de cada ejercicio deberá aparecer capturas de pantalla pertinentes que justifiquen su realización. Intentad hacer todo lo posible desde la consola si no se indica lo contrario. 
> Se valorará negativamente las malas prácticass de GIT 

 

**1.- (0,75) Crea un repositorio en github “AAAExamen23ED“ e invítame a colaborar: "TomBort8" . AAA serán las primeras letras de tu nombre, 1er apellido y 2º apellido respectivamente.** 

<img src="https://i.ibb.co/jDfRc5r/Captura-de-pantalla-2023-12-05-122513.png">
<img src="https://i.ibb.co/TqvLq7z/Captura-de-pantalla-2023-12-05-122356.png">

**2.- (0,75) Inicializa el repostiorio en local y vincúlalo al repostiroio de github** 

<img src="https://i.ibb.co/wJzsLGV/Captura-de-pantalla-2023-12-05-122758.png">
<img src="https://i.ibb.co/wLncFjx/Captura-de-pantalla-2023-12-05-123011.png">
<img src="https://i.ibb.co/WGVC0HZ/Captura-de-pantalla-2023-12-05-123058.png">

**3.- Crea un main que pida 2 números por teclado.** 

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

<img src="https://i.ibb.co/YDFTVyW/Captura-de-pantalla-2023-12-05-123639.png">
<img src="https://i.ibb.co/7g376RP/Captura-de-pantalla-2023-12-05-123729.png">
<img src="https://i.ibb.co/6JzTmLj/Captura-de-pantalla-2023-12-05-123822.png">

**4.- (0,2) Crea  un fichero ExplicaCalculadora.txt : “Este programa es una calculadora que va a poder realizar las operaciones básicas: sumar, restar, multiplicar y dividir”.** 

<img src="https://i.ibb.co/31Zf0Tw/Captura-de-pantalla-2023-12-05-124005.png">
<img src="https://i.ibb.co/rd4RCng/Captura-de-pantalla-2023-12-05-124048.png">

*  **4.1  (0,3)Crea también un fichero de texto que no debes subir a github pero debe estar dentro de la carpeta NoSubir.txt: (Este archivo debes añadirlo y quitarlo, como si te hubieras confundido). “Este archivo debe estar en la carpeta pero no subido a git”.** 

<img src="https://i.ibb.co/RcTtS74/Captura-de-pantalla-2023-12-05-124532.png">
<img src="https://i.ibb.co/xC1nzKN/Captura-de-pantalla-2023-12-05-124617.png">

> Muestra por comandos que no lo has subido 

> Sube los cambios al repositorio. 

<img src="https://i.ibb.co/j3m8pgb/Captura-de-pantalla-2023-12-05-124955.png">
<img src="https://i.ibb.co/8DXf5Kp/Captura-de-pantalla-2023-12-05-125034.png">

**5.- (0,5) Muestra la diferencia entre los 2 últimos commits.** 

<img src="https://i.ibb.co/nnjrv05/Captura-de-pantalla-2023-12-05-125326.png">

**6.- (0,5) Crea 2 ramas SUMADORES y RESTADORES** 

<img src="https://i.ibb.co/brwyLpd/Captura-de-pantalla-2023-12-05-125718.png">
<img src="https://i.ibb.co/pXWb7SD/Captura-de-pantalla-2023-12-05-125805.png">
<img src="https://i.ibb.co/3BXjthR/Captura-de-pantalla-2023-12-05-125634.png">

**7.- Sitúate en SUMADORES y añade al main lo siguiente:**

<img src="https://i.ibb.co/QdL55G8/Captura-de-pantalla-2023-12-05-130054.png">

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

<img src="https://i.ibb.co/fDhVWVs/Captura-de-pantalla-2023-12-05-130623.png">
<img src="https://i.ibb.co/J2Q0vYJ/Captura-de-pantalla-2023-12-05-130659.png">
<img src="https://i.ibb.co/wYJV2HZ/Captura-de-pantalla-2023-12-05-130733.png">

> Sube los cambios al repositorio.

**8.- Sitúate en RESTADORES y añade al main lo siguiente:**

<img src="https://i.ibb.co/M1c3YdF/Captura-de-pantalla-2023-12-05-130824.png">

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

<img src="https://i.ibb.co/9qp5XFW/Captura-de-pantalla-2023-12-05-131205.png">
<img src="https://i.ibb.co/Y7DFfC7/Captura-de-pantalla-2023-12-05-131252.png">
<img src="https://i.ibb.co/y6fykZP/Captura-de-pantalla-2023-12-05-131330.png">

> Sube los cambios al repositorio. 

**9.- (1) Muestra la diferencia entre las ramas sumadores y restadores y guárdalo en un fichero llamado DIFERENCIA _RAMAS (desde consola). Este ficehro debe subirse al repositorio.** 

 <img src="https://i.ibb.co/1n4h5D6/Captura-de-pantalla-2023-12-05-131929.png">

**10.- (1,5) Fusiónalo en main (consola) y resuelve el conflicto (en gitHUB).** 

<img src="https://i.ibb.co/hsLQWVz/Captura-de-pantalla-2023-12-05-132302.png">
<img src="https://i.ibb.co/HgYTyy6/Captura-de-pantalla-2023-12-05-132659.png">

> Sube los cambios al repositorio. 

<img src="https://i.ibb.co/bJr3GPK/Captura-de-pantalla-2023-12-05-132736.png">

**11.-(0,5) Borra las ramas SUMADORES Y RESTADORES.**

 <img src="https://i.ibb.co/VSWPPRC/Captura-de-pantalla-2023-12-05-132902.png">
 <img src="https://i.ibb.co/s1JcRcw/Captura-de-pantalla-2023-12-05-132935.png">

**12.- (0,5) entra a SOURCETREE y haz una captura del eje temporal del repositorio. Haz una breve explicación de lo que observas.** 

 <img src="https://i.ibb.co/KxXZMxW/Captura-de-pantalla-2023-12-05-133139.png">

**13.- (1) ¿ Cuál es la diferencia entre “git pull” y “git clone” ?** 
> git pull descarga el historial del marcador e incorpora cambios mientras que git clone descarga un proyecto y toda su historia de versión.

**14.- (1) Abre el main y déjalo inservible. Sube los cambios. Deshaz el último commit.**
 
 <img src="https://i.ibb.co/ccJ8X9b/Captura-de-pantalla-2023-12-05-133511.png">
 <img src="https://i.ibb.co/s1Hb5KC/Captura-de-pantalla-2023-12-05-133545.png">
 <img src="https://i.ibb.co/DQjG7Vy/Captura-de-pantalla-2023-12-05-133621.png">

**15.- (1) Vuelve al estado en el que estaba el proyecto al acabar el ejercicio 3 en local.**
 
 
 **16.-(0,5) Añade este documento al repoitorio, con todas las imágenes para que se pueda ver desde git.**


**17.- Por último, ejecutad el siguiente comando:** 

> *history > historial.txt* 

**sube el resultado a aules junto al PDF de este documento.** 