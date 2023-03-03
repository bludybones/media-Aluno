# media-Aluno



package exemplo;

import java.util.Scanner;

public class ex01 {
	
	public static void main(String a[]) {
		Scanner teclado;
		teclado = new Scanner(System.in);
		
		String aluno;
		float nota01, nota02, media, soma, mediaturma;
		
		soma = 0;
		for (int i = 0; i < 3; i++) {
			System.out.println("Nome do aluno: ");
			aluno = teclado.nextLine();
			System.out.println("Nota 01: ");
			nota01 = teclado.nextFloat();
			System.out.println("Nota 02: ");
			nota02 = teclado.nextFloat();
			teclado.nextLine();
			
			
			media = (nota01 + nota02)/2;
			soma = soma + media;
			
			if(media >= 6)
				System.out.println("Aluno aprovado, parabens");
			else {
				System.out.println("Aluno reprovadoi");
			}
			
			mediaturma = soma/3;
			System.out.println(mediaturma);
			
			
			
			
		}
	}
	
