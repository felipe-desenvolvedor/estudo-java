# Lista 01 - Resultados


## EX1 

```java
package exercices.scanner;

import java.util.Scanner;

public class Ex1 {

	public static void main(String[] args) {
		Scanner input = new Scanner(System.in);
				
		String nome = getStringWord("Digite um nome: ", input );
		String sobrenome = getStringWord("Digite um sobrenome: ", input );
		
		System.out.println("Pessoa - " + nome + " " + sobrenome);
				
		input.close();
		

	}
		
	private static String getStringWord(String msg, Scanner input) {
		System.out.print(" " + msg);
		return input.next();
	}

}


```

## EX2
``` java
package exercices.scanner;

import java.util.Scanner;

public class Ex2 {
	public static void main(String[] args) {
		Scanner input = new Scanner(System.in);
		
		String nome = getStringWord("Digite seu nome: ", input);
		String cargo = getStringPhrase("Digite seu cargo: ", input);
		double salario = getDouble("Digite seu salário: ", input); 
				
		System.out.printf("%s ocupa o cargo de %s e ganha um salário de %.2f R$", nome,cargo,salario);
		
	}
	
	private static String getStringWord(String msg, Scanner input) {
		System.out.print(" " + msg);
		return input.next();
	}
	private static String getStringPhrase(String msg, Scanner input) {
		input.nextLine(); // limpando o buffer
		System.out.print(" " + msg);
		return input.nextLine();
	}
	private static double getDouble(String msg, Scanner input) {
		System.out.print(" " + msg);
		return input.nextDouble();
	}
}


```
## EX3
``` java
package exercices.scanner;

import java.util.Scanner;

public class Ex3 {

	public static void main(String[] args) {
		Scanner input = new Scanner(System.in);

		String nome = getStringWord("Digite o nome do comprador: ", input);
		
		String nomeProduto = getStringWord("Digite o produto desejado: ", input);
		
		int qtd = getInt("Digite quantidade do produto desejado: ", input);
		
		double preco = getDouble("Digite o preço do produto desejado: ", input);
		
		double precoTotalPedido = preco * qtd ;
		
		System.out.printf("%n%nRELATORIO DO PEDIDO %n nome do comprador : %s %n"
				+ "produto comprado: %s \n quantidade : %d \n valor: %.2f R$ \n total = %.2f R$"
				,nome,nomeProduto,qtd,preco,precoTotalPedido);

	}
	private static String getStringWord(String msg, Scanner input) {
		System.out.print(" " + msg);
		return input.next();
	}
	
	private static double getDouble(String msg, Scanner input) {
		System.out.print(" " + msg);
		return input.nextDouble();
	}
	private static int getInt(String msg, Scanner input) {
		System.out.print(" " + msg);
		return input.nextInt();
	}
}

```
## EX4
``` java


```
## EX5
``` java


```



