using System;

class Program
{
    // 1. Función suma
    static int Sumar(int a, int b)
    {
        return a + b;
    }

    // 2. Función edad
    static string EvaluarEdad(int edad)
    {
        if (edad >= 18)
            return "Es mayor de edad";
        else
            return "Es menor de edad";
    }

    // 3. Área de un círculo
    static double AreaCirculo(double radio)
    {
        return Math.PI * radio * radio;
    }

    // 4. Área de un triángulo
    static double AreaTriangulo(double baseT, double altura)
    {
        return (baseT * altura) / 2;
    }

    static void Main()
    {
        // Suma
        Console.Write("Ingrese el primer número: ");
        int num1 = int.Parse(Console.ReadLine());

        Console.Write("Ingrese el segundo número: ");
        int num2 = int.Parse(Console.ReadLine());

        int resultadoSuma = Sumar(num1, num2);
        Console.WriteLine("La suma es: " + resultadoSuma);

        // Edad
        Console.Write("\nIngrese su edad: ");
        int edad = int.Parse(Console.ReadLine());

        string mensajeEdad = EvaluarEdad(edad);
        Console.WriteLine(mensajeEdad);

        // Área del círculo
        Console.Write("\nIngrese el radio del círculo: ");
        double radio = double.Parse(Console.ReadLine());

        double areaC = AreaCirculo(radio);
        Console.WriteLine("El área del círculo es: " + areaC);

        // Área del triángulo
        Console.Write("\nIngrese la base del triángulo: ");
        double baseT = double.Parse(Console.ReadLine());

        Console.Write("Ingrese la altura del triángulo: ");
        double altura = double.Parse(Console.ReadLine());

        double areaT = AreaTriangulo(baseT, altura);
        Console.WriteLine("El área del triángulo es: " + areaT);
    }
}
