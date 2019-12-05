# promedio_altura_personas
Lee x alturas de personas por teclado y muestra la altura promedio de las personas.

import java.util.Scanner;

public class alturas_personas {

	public static void main (String[] args) {
		Scanner teclado=new Scanner(System.in);
		int n,x;
		float altura, suma, promedio;
		System.out.println ("Cuantas personas hay?: ");
		n=teclado.nextInt();
		x=1;
		suma=0;
		while (x<=n) {
			System.out.println("Introduce una altura: ");
			altura=teclado.nextFloat();
			suma=suma+altura;
			x=x+1;
		}
		promedio=suma/n;
		System.out.println("Altura promedio: "+promedio);
	}
}
