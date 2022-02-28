package calculadoraConversionUnidades;

import java.util.Scanner;

/**
 * Calculadora de conversion de unidades de medida.
 * 
 * Inicialmente implementa conversion de unidades de temperatura.
 * 
 * @author CamiloM
 * 
 */
public class main {

	public static void main(String[] args) {
		Scanner teclado = new Scanner(System.in);
		int opcion = 0;
		double tempInicial, resultado;
	
		while(opcion !=7) {
			opcion = mostrarMenu(teclado);
			switch(opcion) {
			case 1:
				System.out.println("digite la temperatura en Kelvin");
				tempInicial = teclado.nextDouble();
				resultado = convertirKelvinCelsius(tempInicial);
				System.out.println("La temperatura en Celsius es: "+ resultado + "\n");
				break;
			case 2:
				System.out.println("Digite la temperatura en Kelvin");
				tempInicial = teclado.nextDouble();
				resultado = convertirKelvinFahrenheit(tempInicial);
				System.out.println("La temperatura en Fahrenheit es: " + resultado);
				break;
			case 3:
				System.out.println("Digite la temperatura en Celsius");
				tempInicial = teclado.nextDouble();
				resultado = convertirCelsiusKelvin(tempInicial);
				System.out.println("La temperatura en kelvin es: " + resultado);
				break;
			case 4:
				System.out.println("Digite la temperatura en faherenheit");
				tempInicial = teclado.nextDouble();
				resultado = convertirFaherenheitKelvin(tempInicial);
				System.out.println("La temperatura en kelvin es: " + resultado);
				break;
			case 5:
				System.out.println("Digite la temperatura en faherenheit");
				tempInicial = teclado.nextDouble();
				resultado = convertirFaherenheitCelsius(tempInicial);
				System.out.println("La temperatura en celsius es: " + resultado);
				break;
			case 6:
				System.out.println("digite la temperatura en faherenheit");
				tempInicial = teclado.nextDouble();
				resultado = convertirCelsiusFaherenheit(tempInicial);
				System.out.println("La temperatura en kelvin es: " + resultado);
				break;
			case 7:
				System.out.println("--- Programa Terminado ---");
				break;
			}//fin switch
		}//fin while
	}

	/**
	 * Muestra el menu de seleccion de tipo de conversion
	 * 
	 * @param teclado es un objeto {@code Scanner} para lectura a traves del teclado 
	 * @return Opcion int seleccionada por el usuario
	 */
	public static int mostrarMenu(Scanner teclado) {
		int opcion;
		System.out.println("\n --- MENU --- ");
		System.out.println("1. convertir kelvin a Celsius");
		System.out.println("2. convertir kelvin a Fahrenheit");
		System.out.println("3. convertir Celsius a Kelvin");
		System.out.println("4. convertir Fahrenheit a Kelvin");
		System.out.println("5. convertir Fahrenheit a Celsius");
		System.out.println("6. convertir Celsius a Fahereneit");
		System.out.println("7. Salir");
		opcion = teclado.nextInt();
		return opcion;
	}

	/**
	 * funcion que recibe una temperatura en kelvin y la convierte a celsius
	 * 
	 * @param kelvin: temperatura en grados kelvin
	 * @return Resultado de la operacion c=k-273,15
	 */
	public static double convertirKelvinCelsius(double kelvin) {
		double celsius;
		celsius = kelvin - 273.15;
		return celsius;
	}
	/**
	 * funcion que recibe una temperatura en kelvin y la convierte en faherenheit
	 * @param kelvin: temperatura en grados kelvin
	 * @return resultado de la operacion faherenheit= 9 * (kelvin-273.15)/5+32
	 */
	public static double convertirKelvinFahrenheit(double kelvin) {
		double fahrenheit;		
		fahrenheit = 9 * (kelvin-273.15)/5+32;
		return fahrenheit;
	}
	/**
	 * funcion que recibe una temperatura en celsius y la  convierte a kelvin
	 * @param celsius: temperatura en grados celsius
	 * @return Resultado de la operacion  k=c+2.73.15
	 */
	public static double convertirCelsiusKelvin(double celsius) {
		double kelvin;		
		kelvin = celsius + 273.15;
		return kelvin;
	}
	/**
	 * funcion que recibe una temperatura en Fahereneit y la convierte a kelvin
	 * @param Fahereneit: temperatura en grados fahereneit
	 * @return Resultado de la operacion k= 5*(F-32)/(9) + 273.15
	 */
	public static double convertirFaherenheitKelvin(double faherenheit) {
		double kelvin;		
		kelvin= 5*(faherenheit-32)/(9) + 273.15;
		return kelvin;
	}
	/**
	 * funcion que recibe una temperatura en faherenheit y la convierte a celsius
	 * @param Faherenheit: temperatura en grados faherenheit
	 * @return Resultado de la operacion c=(5*(F-32))/(9)
	 */
	public static double convertirFaherenheitCelsius(double faherenheit) {
		double celsius;		
		celsius = (5*(faherenheit-32))/(9);
		return celsius;
	}
	/**
	 * funcion que recibe una temperatura en celsius y la  convierte a Faherenheit
	 * @param celsius: temperatura en grados celsius
	 * @return Resultado de la operacion  F=(9*C)/(5)+32
	 */
	public static double convertirCelsiusFaherenheit(double celsius) {
		double faherenheit;		
		faherenheit = (9*celsius)/(5)+32;
		return faherenheit;
	}
}
