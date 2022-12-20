//Задача 64: Задайте значение N. Напишите программу, которая выведет все натуральные числа в промежутке от N до 1. Выполнить с помощью рекурсии.

//N = 5 -> "5, 4, 3, 2, 1"
//N = 8 -> "8, 7, 6, 5, 4, 3, 2, 1"
/*
void ShowNumbers (int n)
{
    Console.Write(n+" ");
    if(n>1)ShowNumbers(n-1);
   
}

ShowNumbers(8);
*/
//Задача 66: Задайте значения M и N. Напишите программу, которая найдёт сумму натуральных элементов в промежутке от M до N.

//M = 1; N = 15 -> 120
//M = 4; N = 8. -> 30
/*
int ShowNumbers(int m, int n)
{
   if(m==0) return n;
   else if(n==0) return m;
   else if(m>n) return n + ShowNumbers(m,n+1);
   else if (m<n) return n + ShowNumbers(m, n-1);
   return m;

}

Console.WriteLine(" Input a first number: ");
int a1 = Convert.ToInt32(Console.ReadLine());
Console.WriteLine(" Input a second number: ");
int b1 = Convert.ToInt32(Console.ReadLine());
int sum = ShowNumbers(a1,b1);
Console.WriteLine($"Sum of digits = {sum}");
*/

//Задача 68: Напишите программу вычисления функции Аккермана с помощью рекурсии. 
//Даны два неотрицательных числа m и n.
//m = 2, n = 3 -> A(m,n) = 9
//m = 3, n = 2 -> A(m,n) = 29
/*
int Accerman(int m, int n)
{    
    if (m<0 || n<0) return -1;
    else if(m==0) return n+1;
    else if(n==0) return Accerman(m-1,1);
    else if(n>0 && m>0) return Accerman(m-1, Accerman(m,n-1));
    return 0;
}
Console.WriteLine(" Input a first number: ");
int a1 = Convert.ToInt32(Console.ReadLine());
Console.WriteLine(" Input a second number: ");
int b1 = Convert.ToInt32(Console.ReadLine());

Console.WriteLine(Accerman(a1,b1));
*/