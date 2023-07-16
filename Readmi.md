<!--  Задача 10: Напишите программу, которая принимает на вход 
трёхзначное число и на выходе показывает вторую цифру 
этого числа.
456 -> 5
782 -> 8
918 -> 1 

Console.WriteLine("Введите трехзначное число.\nВыход из программы команда Exit.");
    while(true)
    {
        string input = Console.ReadLine();
        if(!input.Equals("exit"))
            Console.WriteLine("{0}->{1}",input, input[1]);
        else
            break;
    } 
 


Задача 15: Напишите программу, которая принимает на вход цифру,
обозначающую день недели, и проверяет, является ли этот день
выходным.
6 -> да
7 -> да
1 -> нет 

int Prompt(string msg)
{

System.Console.WriteLine($"{msg}");
return Convert.ToInt32(Console.ReadLine());
}
int number = Prompt("Введите число: ");
string ss = ("Упс! Такого дня недели нет!");
string check(int number)
{
if (number >= 5 && number < 7) ss = ("Ехуу! выходной!");
if (number >= 1 && number < 6) ss = ("Увы, это рабочий день");
return ss;
}
System.Console.WriteLine(check(number)); 


Задача 13: Напишите программу, которая выводит третью цифру заданного числа или сообщает, что третьей цифры нет.
645 -> 5
78 -> третьей цифры нет
32679 -> 6 


int Prompt(string msg)
{

System.Console.WriteLine($"{msg}");
return Convert.ToInt32(Console.ReadLine());
}
int number = Prompt("Введите число: ");

int fnumber(int number)
{
while (number > 999)
{
number /= 10;
}
return number % 10;
}

bool check(int number)
{
if (number < 100)
return false;
else return true;
}

if (check(number) != true)
System.Console.WriteLine("Третьей цифры нет.");
else
System.Console.WriteLine($"Третья цифра числа {number} является {fnumber(number)}"); 


  -->