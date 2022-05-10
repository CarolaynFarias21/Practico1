# practico1
package ejer1;
import java.util.Scanner;

public class Programa {
	Scanner teclado=new Scanner(System.in);
	    String apellido;
	    int cedula,edad;
	    double altura;
	    
	public void iniciar() {
		cargar();
		imprimir();
		
	}//fin iniciar 

	private void imprimir() {
		System.out.println("Apellido:" + apellido );
		System.out.println("Cedula:" + cedula );
		System.out.println("Edad:" + edad );
		System.out.println("Altura:" + altura );
		
	}

	private void cargar() {
    System.out.println("Ingrese apellido:");
    apellido=teclado.nextLine();
    System.out.println("Ingrese cedula:");
    cedula=teclado.nextInt();
    System.out.println("Ingrese edad:");
    edad=teclado.nextInt();
    System.out.println("Ingrese altura:");
    altura=teclado.nextDouble();
    
    
		
		
	}

}
Ejer2
package ejer2;
import java.util.Random;
import java.util.Scanner;


public class Programa {

 
	void iniciar(){
		
		int valor=generarAleatorio();
		int num;
		int resul;
		
		do{
			num=pedirNumero();
			resul=compararNumeros(num, valor);
			System.out.println(valor);
			if (resul==1) {
				System.out.println("Demasiado grande");
			}
			else if (resul==-1)
					System.out.println("Demasiado chico");
			
		}while(resul!=0);
		System.out.println("Felicitaciones acertaste!!");
	}
	
	//devuelve un numero aleatorio entre 1 y 100
	private int generarAleatorio(){
		Random azar = new Random();
		int valor = azar.nextInt(1000)+1;
		return valor;
		
	}
	
	//pide un nro por pantalla
	 private int pedirNumero(){
		 Scanner entrada=new Scanner(System.in);
		 System.out.println("Ingrese un numero");
		 int num=entrada.nextInt();
		 return num;
	}
	
	 //compara dos enteros a y b. Devuelve un int indicando si es menor, mayor o igual
	 int compararNumeros(int a, int b){	
	     int resul;
	     if (a>b)
			 resul=1;
		 else if (a<b)
			 resul=-1;
		 else 
		 resul=0;
		 
	     return resul;
		 
		 
					  
	 }
   Ejer3
   
