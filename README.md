# Kansiris CSHARP Interview Questions Answers
> Bu [linkdədəki inteveiw sualların](https://github.com/DrMadWill/KansirisCSHARP-InterviewQuestions-Answers)ı cavablandırmağa çalışdım.
### What is Computer programming?
***
> **My Answer** : Hər hansı Developing Probleminin Probelmi anlama, Problemin həlliniə uyğun Kod Structurun qurulası, Kodun yazılması, Bu koda yaranan prablemlərin həlli, Testləmə və Nəticə döngüsünə girməsi .

### How programming work?
***
> **My Answer** : Programlaşdırma dilinin _keyword_-ləri vastəsi ilə komputerə görüləcək işlər barəsində əmir vermək.

### What is debugging?
***
> **My Answer** : Xətaları tapma sonra onların Səbəblərni tapıb xətaları və ya səbəbləri arada qaldırma.

### Name different types errors which can occur during the execution of a program?
***
> **My Answer** : 3 tip proramlaşdırma _error_-u ala bilirik:
1. Syntax Error və ya Compiler Time Error : kodun sintaksisi düzgün yazılmadıqda ortaya çıxar.
2. Runtime Errors : Yazılan pragramın məqsədə uyğun işləməməsi. Məsələn: Əmir => Get qapını aç. Error => Orda qapı yoxdur. 
3. Logical errors : Yazılan proqramda mətiqi xətlar oluğunu göstərir. Məsələn : Komputerə verilən əmir qapını açmaqdır o qapnı örtür.

### When a syntax error occurs?
***
> **My Answer** : proramlaşdırma dilinin Syntax qaydalarina riayət etmədkidə Syntax Error alıq. Yazılan kodların compiler tapıb göstərdiyi errorlar Compiler Time Errordur və ya Syntax Error.

### When a runtime error occurs?
***
> **My Answer** : Komputer databasesdən məlumatı gətirməsini istəyərsiz ancaq belə bir databases yoxdur bu zaman _Runtime Error_ alıqırıq. Program işlədiyi vaxt bu errorları alırıq və tapılması nisbətən asandır.

### What is flowchart?
***
> **My Answer** : Problemin həlli yolunun riyazi qrafiki.

### What is an algorithm?
***
> **My Answer** : Prorblemin daxilindəki Problemlərin ardıcıl həlləri toplusudur. _Algorithm_ anaqlı, icra edilə bilən və mümkün qədər qısa olmalıdır.

### What do you understand by the term 'Maintain and update the Program'?
***
> **My Answer** : Bir programin yazıldıqdan(publish edildikdən) sonrakı dövürlərdə gəliştirilərək yeni gəlişən platformalara uyğunlaşdırmaq , prorgrama yeni funksiyalarin ələvə edəlməsi və _bug_-ların aradan qaldırılması.

### What are variables?
***
> **My Answer** : Hər hansı bir əşyanı tutmaq,saxlamaq və daşımaq  üçün əşyanı saxlayabiləcək qablar ehtiyac var. Birdə bu qablar kifayyət qədər açıqlaycı olamalıdır ki biz onlara baxdıqda daxilində nə olduğunu bilək. Burada əşya value dur,Qab isə variable-dir.

### What are reserved words?
***
> **My Answer** : Programlaşdırma dilində daxilində bir və bir neçə hadisəni gerçəkləşdirmək üçün Programlaşdırma dilinə qabcadan yazılmış _key_-lər və mətin pracacıqlarıdır. 

###  What are Loop?
***
> **My Answer** : Bir kod pracasını öncədən müəyyən edilmiş sayda(bu bir şərtdə ola bilər) təkrarıdır.
- Code
```markdown

for (int i = 0; i < 3; i++)
    {
        Console.WriteLine("Hello World!");
    }

```
- We see
```
Hello World!
Hello World!
Hello World!

C:\Users\nofel\OneDrive\Desktop\CDev\Task\Task\bin\Debug\netcoreapp3.1\Task.exe (process 11464) exited with code 0.
Press any key to close this window . . .
```
### What is the use of FOR…NEXT Loop?
***
> **My Answer** : `for` dövrünün müəyyən bir şərti ödəyənədə həmin təkrarı buraxib növbəti döngüyə keçir.
- Code

```
    for (int i = 0; i < 5; i++)
        {
            if (i == 3)// condition
                continue;


            Console.WriteLine(i);
        }

```
- We see
```
0
1
2
4
```

### What is the use of WHILE…WEND Loop?
***
> **My Answer** : Döngü müəyyən şərti ödəyənə qədər davam edəcəksə `while` döngüsündən isfadə edirik. Döngünün sayı bilinmədikdə isfadə edilir.
- Code

```
    int i = 0; // initialization

    while (i < 10) // condition
    {
        Console.WriteLine($"i = {i}") ;
        i++; // increment
    }

```
- We see
```
i = 0
i = 1
i = 2
i = 3
i = 4
i = 5
i = 6
i = 7
i = 8
i = 9
```
### What is the use of Nested Loop?
***
> **My Answer** : Döngü daxilində döngüdən söhbət gedir. Xaricdəki döngü ilə daxildəki döngü arsında hər hası bir şərti ödəyən informasiyaların axtarilması döngünü misal göstərmək olar.
- Code

```
    int[] numbers = { 1,4,5, 6, 78 };

        for (int i = 0; i < 5; i++)
        {
            foreach (var item in numbers)
            {
                if (item == i)
                {
                    Console.WriteLine($"Success : {i}");
                }
            }

        }

```
- We see
```
Success : 1
Success : 4

```

### What is Documentation?
***
> **My Answer** : Programin yazılmasi zaman istfadə edoilən kod strukturu, qarşıya çıxan _error_-lar, onlarin həlli yolları , _update_-lər, istfadəsi və s. kimi program haqda önəli məlumatatlar açıqlamsıdır. Programçıların can damarı və bəlasıdır.

###  What is the working of a compiler?
***
> **My Answer** : Proglamlaşdırma dilində uyğun keywordləri işləyərək başqa bir dilə çevirən onu komputerdə işlək vəziyətə çevirən kod parçası. Compiler yazılan kod çevrilir `IL` dilinə.

### What do we call the binary form of a target language?
***
> **My Answer** : Binar kod və ya ikiklik say sistemində yazılmış kod.

### What are constants?
***
> **My Answer** : `const` `Class` daxilidə təyin edlilərək program icrasi vaxt və ya yazılmasi müddətində dəişdirilmir.`const` variable ancaq `const` variable bərəbərləşdirlə bilər. `static` təyin etmək mükün deyildir.
- Code
```
    public const int a = 25;
    public const int b = a;
    public const int c = a + b;
```

### Define Numeric constants.
***
> **My Answer** : Tam və kəsir olaraq ədəd `constant` iki hissədən ibarətdir.
- Code
```
    public const int a = 25;
    public const double val_dob = 25;
```
### Define String constants
***
> **My Answer** : `Length` maksumum 255 olan `char` _array_-ı dır.

- Code

```
    foreach (var item in str)
        {
            Console.WriteLine($"Char : {item}");
        }

public const string str = "string value";    

```
- We see
```
Char : s
Char : t
Char : r
Char : i
Char : n
Char : g
Char :
Char : v
Char : a
Char : l
Char : u
Char : e

```

### Define Operators.
***
> **My Answer** : Riayazi, Mətiqi və s. əməliyyatları həyata keçirən _keyword_-lər toplusudur.

- Code

```
    foreach (var item in str)
        {
            Console.WriteLine($"Char : {item}");
        }

    if (1 < 5)
        {
            Console.WriteLine($">> Success");
        } 

```
### What is an Array?
***
> **My Answer** : Bir neçə informasiyanı toplu şəkildə yaddaşda ardıcıl yer tutaraq bir _variable_ altında toplayan informaisia toplusudur.

- Code

```
    int[] numbers = { 1, 4, 5, 6, 78 }; 

```
