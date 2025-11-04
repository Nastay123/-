using System;

using 4ntvf;

namespace NetStandardConsoleApp
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Тестирование  библиотеки ");
            Console.WriteLine();
            Console.WriteLine("Тестируем void методы:");

            4ntvf.MathOperations.DisplayMessage("Это тестовое сообщение из консольной программы.");

            4ntvf.MathOperations.AddAndDisplay(30, 40);
            Console.WriteLine();
            Console.WriteLine("Тестируем методы с возвращаемыми значениями:");

            int sumResult = 4ntvf.MathOperations.Add(100, 25);
            Console.WriteLine($"Результат сложения: {sumResult}");

            double productResult = 4ntvf.MathOperations.Multiply(7.5, 3.0);
            Console.WriteLine($"Результат умножения: {productResult}");

            int numberToCheck = 23;
            bool isPrimeResult = 4ntvf.MathOperations.IsPrime(numberToCheck);
            Console.WriteLine($"Число {numberToCheck} простое? {isPrimeResult}");

            numberToCheck = 24;
            isPrimeResult = 4ntvf.MathOperations.IsPrime(numberToCheck);
            Console.WriteLine($"Число {numberToCheck} простое? {isPrimeResult}");
            Console.WriteLine();

            Console.WriteLine("Тестирование библиотеки завершено. Нажмите любую клавишу для выхода");
            Console.ReadKey();
        }
    }
}
