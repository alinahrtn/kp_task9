# kp_task9  
1. Вы живёте в 2010м. Вас попросили написать метод, приводящий неформальные сообщения из почтового ящика к человекочитаемому виду. Но некоторые фрагменты текста не форматировались с помощью универсальной логики метода. Отформатируйте их при помощи методов форматирования строк. 

**In**: пРиФФкИ 4увиха…твои тя_ги просто   ………… ЖЕСТЬ

**Out**: Приффки чувиха… Твои тяги просто жесть.

**In**: !!! Эй,гошарь !!!!    Иди на кУХНе пошарь, ххыыыы)))))))

**Out**: Эй, гошарь! Иди на кухне пошарь, хы)

**In**: Про100  4елове4ек Атсартировал пять колечегГг

**Out**: Просто человечек атсартировал пять колечек.  
    
2. (*) Отформатируйте эти строки, используя регулярные выражения (regular expressions)
  
3. Реализуйте алгоритмы с помощью циклов и с помощью встроенных методов класса String:
   - замена символов в строке
   - подсчет числа различных символов ,
   - поиск заданного фрагмента строки.
   
   Как может выглядеть основа для второго алгоритма:
   ```
   Dictionary<char, int> entries = new Dictionary<char, int>();

    for(int i = 0; i < src.Length; i++)
    {
        if (entries.ContainsKey(src[i]))
        {
            continue;
        }

        for (int j = i; j < src.Length; j++)
        {

        }
    }
   ```
  3.1. (* Гжесть какое сложное) Во втором алгоритме не получится разумно использоать методы класса String. Вместо этого оставьте внешний цикл, а внутренний замените с использованием метода Count(), внутрь которого подаётся лямбда-выражение (так называется короткая функция, которая пишется в одну строчку. В случае Count() лямбда применяется к каждому элементу коллекции, к которой применяется метод. Выглядит лямбда-функция, например, так: ```x => x == 12 ``` - функция с параметром x, которая возвращает true, если x == 12). Count() относится к выражениям LINQ. LINQ сильно упрощают жизнь и сами по себе они тоже не сложные, поэтому, если научиться ими пользоваться, будете в малине. Можете почитать об этом, например, на Metanit
