# My-Java-training-projects
//Temperature Converter project
import java.util.Scanner;

public class Temp_converter 
{
	public void cel_far()
	{
		Scanner sc=new Scanner(System.in); 
		System.out.println("Enter the temperature in celsius:");
		double c=sc.nextInt();
		double f= c*9/5 + 32;
		System.out.println("The temperature in Fahrenheit:"+f);
	}
	public void far_cel()
	{
		Scanner sc=new Scanner(System.in); 
		System.out.println("Enter the temperature in Fahrenheit:");
		double f=sc.nextInt();
		double c = f-32*5/9;
		System.out.println("The temperature in Celcius:"+c);
	}
	public void cel_kel()
	{
		Scanner sc=new Scanner(System.in); 
		System.out.println("Enter the temperature in Celcius:");
		double c=sc.nextInt();
	    double k=c+273.15;
		System.out.println("The temperature in kelvin:"+k);
	}
	public void kel_cel()
	{
		Scanner sc=new Scanner(System.in); 
		System.out.println("Enter the temperature in Kelvin:");
		double k=sc.nextInt();
		double c=k-273.15;
		System.out.println("The temperature in Celsius:"+c);
	}
	public void far_kel()
	{
		Scanner sc=new Scanner(System.in); 
		System.out.println("Enter the temperature in Fahrenheit:");
		double f=sc.nextInt();
		double k = f-32* (5/9) + 273.15;
		System.out.println("The temperature in Kelvin:"+k);
	}
	public void kel_far()
	{
		Scanner sc=new Scanner(System.in); 
		System.out.println("Enter the temperature in Kelvin:");
		double k=sc.nextInt();
		double  f = k-273.1* (9/5) + 32;
		System.out.println("The temperature in Celsius:"+k);
	}

	public static void main(String[] args) {
		Temp_converter a=new Temp_converter();
		Scanner sc=new Scanner(System.in);
		System.out.println("Convertions:\n1. Celcius to Fahrenheit\n2. Fahrenheit to Celcius\n3. Celsius to Kelvin\n4. Kelvin to Celsius\n5. Fahrenheit to Kelvin\n6. Kelvin to Fahrenheit\nEnter your choice:");
		int ch=sc.nextInt();
		switch(ch)
		{
		case 1:
			a.cel_far();
			break;
		case 2:
			a.far_cel();
			break;
		case 3:
			a.cel_kel();
			break;
		case 4:
			a.kel_cel();
			break;
		case 5:
			a.far_kel();
			break;
		case 6:
			a.kel_far();
			break;
		}

	}

}
