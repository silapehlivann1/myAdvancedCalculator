// ADVANCED MULTİ OPERATİON CALCULATOR

Console.WriteLine("Enter the first number:");
double number1=Convert.ToDouble(Console.ReadLine());
Console.WriteLine("Enter the second number:");
double number2=Convert.ToDouble(Console.ReadLine());
Console.WriteLine("choose the operation: +,-,*,/");
string operation=Console.ReadLine();
double result;

if (operation=="+")
{
    result = number1 + number2;
    Console.WriteLine($"Answer is: {result}");
}
else if (operation=="-")
{
    result = number1 - number2;
    Console.WriteLine($"Answer is: {result}");
}
else if (operation=="*")
{
    result = number1 * number2;
    Console.WriteLine($"Answer is: {result}");
}
else if (operation=="/")
{
    if (number2 != 0)
    {
        result = number1 / number2;
        Console.WriteLine($"Answer is: {result}");

    }
    else
    {
        Console.WriteLine("Error: Division by zero is not allowed.");
    }
}
else
{ 
    Console.WriteLine("Invalid operation. Please choose +, -, *, or /.");
}
    
Console.ReadKey();
