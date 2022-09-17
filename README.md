# Контрольная работа

## Перечень задач:
1. [Создать репозиторий на GitHub](#task1)
2. [Нарисовать блок схему алгоритма](#task2)
3. [Снабдить репозиторий оформленным текстовым описанием (файл Readмe.md)](#task3)
4. [Написать программу, решающую поставленную задачу](#task4)
5. [Использовать контроль версий в работе над этим небольшим проектом (не должно быть так что все залито одним коммитом, как минимум этап 2, 3 и 4 должны быть расположены в разных коммитах)](#task5)

Решение 
- операторы по преобразованию текста в массив и обратно:

//оператор .Split
//строка преобразуеться в массив где разделителем между элементами является ,
//например
string strLine = "шорох,порох,высота";
string[] inArr = strLine.Split(",");
//результатом выполнения будет
//inArr[0]="шорох" : inArr[1]="порох" : inArr[2]="высота"

//оператор .Join
//преобразует массив в текстовую строку разделяя элементы , 
string resultJoin = string.Join(",", inArr);
//результатом выполнения будет
//resultJoin="шорох,порох,высота"
```
- оператор для увеличения размера массива
```C#
//оператор Array.Resize
//увеличивает размер массива с сохранением данных находящихся в нем
string[] outArr = new string[1];
outArr[0]="Hello";
Array.Resize(ref outArr, outArr.Length + 1);
outArr[1]="World";
//результатом выполнения будет
// outArr[0]="Hello" : outArr[1]="World"
