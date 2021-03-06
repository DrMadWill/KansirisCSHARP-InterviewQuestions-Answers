# Kansiris CSHARP Interview Questions Answers  <img src="https://i.postimg.cc/kXnJkdQX/kansir.jpg" align="right" height="300" width="250" >
> Bu günlərdə **Interview**-da `C#`-dan ən çox soruşulan suallari cavablandlandlirmağa çalışdım.
- [My Answer in Medium](https://medium.com/@DrMadWill/i-answered-to-interview-question-1d73a19695f8)
- [My Answer in GitHub](https://github.com/DrMadWill/KansirisCSHARP-InterviewQuestions-Answers)
- [Questions source](https://github.com/kansiris/C-Sharp-c-interview-question)

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
```c

for (int i = 0; i < 3; i++)
    {
        Console.WriteLine("Hello World!");
    }

```
- We see
```c
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

```c
    for (int i = 0; i < 5; i++)
        {
            if (i == 3)// condition
                continue;


            Console.WriteLine(i);
        }

```
- We see
```c
0
1
2
4
```

### What is the use of WHILE…WEND Loop?
***
> **My Answer** : Döngü müəyyən şərti ödəyənə qədər davam edəcəksə `while` döngüsündən isfadə edirik. Döngünün sayı bilinmədikdə isfadə edilir.
- Code

```c
    int i = 0; // initialization

    while (i < 10) // condition
    {
        Console.WriteLine($"i = {i}") ;
        i++; // increment
    }

```
- We see
```c
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

```c
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
```c
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
```c
    public const int a = 25;// initialization
    public const int b = a;// initialization
    public const int c = a + b;
```

### Define Numeric constants.
***
> **My Answer** : Tam və kəsir olaraq ədəd `constant` iki hissədən ibarətdir.
- Code
```c
    public const int a = 25;// initialization
    public const double val_dob = 25;// initialization
```
### Define String constants
***
> **My Answer** : `Length` maksumum 255 olan `char` _array_-ı dır.

- Code

```c
    foreach (var item in str)
        {
            Console.WriteLine($"Char : {item}");
        }

public const string str = "string value";// initialization    

```
- We see
```c
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

```c
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

```c
    int[] numbers = { 1, 4, 5, 6, 78 }; // initialization

```
### What is subroutine?
***
> **My Answer** : _method_ bir alt programdır çağrıldığı yerdə daxildəki funksiyanı yerinə yetirir və _method_ olduğu üçün biz onun access olduğu yerlərdə çağrıb həmin funksiyanı icrasını tələb edə bilərik.

### What is the purpose of arithmetic operators?
***
> **My Answer** : Müəyyən edilmiş bir riyazı əməliyyatları yerinə yetirən _keyword_-lər toplusudur.

- Code

```c
    int c = 5 + 5; 
```

### What is the purpose of relational operators?
***
> **My Answer** : `value`-lər arsindakı riyazı münasibətləri təyin etmək üçün isfadə edilir.`ture` və `false` dəyərlər döndürür. 
- Code
```c
    bool d = 5 >= 4; 
```


### Define Low-level programming language.
***
> **My Answer** : İnsan dilinə uzaq maşın dilinə yaxın bir porglamlaşdırma dili deməkdir. Burada İnsasn dili Obyekt yönümlü programlaşdırmaya yünəlikdir.


### Define High-Level programming language.
***
> **My Answer** : İnsan dilinə daha yazın və anlşılır olur. Bu programlaşdırma dilini öyənmək _Low-level programming language_ öyrənməkdən daha asan və anlaşılırdı.

### What is Machine code?
***
> **My Answer** : Hər hansı bir komputer yazılan maşın kodundakı informasiya doğrudan icra olnur. Amma fərqli komputerlərin fərliq maşın dilləri olduğu üçün programçılar kodları maşın dilində yazmırlar. 

### What is the working on an algorithm?
***
> **My Answer** :  Verilən _İnput_-la problemlemi həll edərək _Output_-a çatırmaq alqoritimdir.

### How is the division by zero defined?
***
> **My Answer** : Division by zero is not defined.


### What is the meaning of implementation of a program?
***
> **My Answer** : Böyük programlar kiçik program hissələrindən ibarət olur. Kiçik program hissləri ona verlən input düzügün şəkildə işləyib outputa ötürə bilirsə həmin program hissələri böyük(əsas) programda yerinə(implementation) yazılır.

###  What are numeric variables?
***
> **My Answer** : Daxilində kəsir və tam ədədləri tutan dəyişkən tipidir.

### What are string variables?
***
> **My Answer** : Daxilində mətinləri Char array-ı şəkilində saxlayan  dəyişkən tipidir.

### Differentiate between the while and for loop in C#.
***
> **My Answer** : While döngüsü biz döngünün sayni bilmədikdə işlənir və bool dəyərindən bir dəyər qəbul edir.Həmin şərt false dəyəri döndürənə qədər davam edir. For dövrü biz dövrün saynı bildikdə işlədilir.

###  What is the syntax to declare a namespace in .NET?  
***
> **My Answer** : Eyni məqsədə xidmət edən Class-ları,Methodları və s. bir başlıq altinda tutmaq üçün istfadə edilir.Kodun oxuna bilirliyni artirmaq üçün və ən önəmlisi qarışıqlığı aradan qaldırmaq üçün lazımdır. Bir çox programlama dilində olduğu kimi C#-da da bir dəyişəni bir dəfə təyin etmək mümkündür. Bu böyük programlarda bir dəyişəni istfadə etməyimizə gətrib çıxarırdı.`namespace` isfadə edərək bunun qarşına keçə bilirik və həmin programların oxunurluğu və anlaşırlığı artır..

###  What is an identifier? 
***
> **My Answer** : Bir programda developer tərfindən clas-a,method-a və s. ad verilməsi tələb edilir.Bu adlar `identifier` dir. `identifier`-lər rəqəmlə başlaya bilməz və case sensitive deyilən Böyük və kiçik həriflərə həssasdır .Yəni myReader ilə MyReader fərqli elemetlərdir.

###  What does a break statement do in the switch statement?
***
> **My Answer** : Switch ifadəsidə göndərilən dəyişkənin bir neçə şərtə uyğunluğunu yoxlamaq məqsədi ilə isfdə edilir və burda case həmin şərtlərdir. case sonladırmaq üçün break keyindən isfadə edilir. 

- Code
```c
     switch (number)
        {
            case 5:
                Console.WriteLine("This number is 5");
                break;
            case 15:
                Console.WriteLine("This number is 15");
                break;
            case 30:
            case 35:
                Console.WriteLine("This number is 35 or 30 ");
                break;

            default:
                Console.WriteLine("No conditions were met.");
                break;
        }
```

###   Explain keywords with example.
***
> **My Answer** : Keyword programlaşdırma dililərində xususi yeri var və identifier ola bilməz.Yəni program daxilində yenidən təyin edilə bilməz.Pogramlaşdırma dilində öncədən təyin edilmiş bir hadisəni və ya xususiyyəti göstərir. Məsələn `break` keyword-ü loop-ların sonlandırmaq üçün isfadə edilir.


- Code
```c
    for (int i = 0; i < 7; i++)
        {
            Console.WriteLine($"i = {i}");
            if (i == 3)
            {
                break;
            }
        }

     
```

- We see
```c
i = 0
i = 1
i = 2
i = 3
```

###  What is the difference between “continue” and “break” statements in C#?
***
> **My Answer** : `break` ifadəsi yuxarıda da bəlirtiyim kimi hər hansı döngünü solnadırır.`continue` ifadəsi isə döngü həmin ifadənəni gördüyü anda növbəti döngüyə keçir.


- Code
```c
    for (int i = 0; i < 7; i++)
        {
            if (i == 1)
            {
                continue;
            }
            Console.WriteLine($"i = {i}");
            if (i == 3)
            {
                break;
            }
            

        }

     
```

- We see
```c
i = 0
i = 2
i = 3
```

###  What is the difference between constant and readonly in c#?
***
> **My Answer** : `constant` və `readonly` ikisidə programin başlanğıcında təyin edilməlidir,`constant` anacq value type isftadə edilə bilir, `readonly` referance type və ya value type işlədilə bilər.`constant` təyin edildikdə bu dəyərin sonra dəişiriməyəcək deməkdir və ancaq təyin edildiyi yerdə dəyər yazmaq olar.`readonly`-də isə həm təyin edildir həm də constructor da təyin edilə bilir və bu fildi boş saxlayib yarılan anda dəyər tələb edə bilərik. 


###   What is the difference between ref and out keywords?
***
> **My Answer** : ref və out bu keyword-lərin köməyi ilə biz methoda göndərdiyimiz value dəyərin koyası deyil həmin dəyərin adresi gedir yəni bu method daxilidə göndərilən dəyər dəişsə həm dəyər method xaricində də dəyişəcək. ref keyword ilə təyin edilən method-a gonderilən dəyər boş ola bilməz. out keyword ilə təyin edilən method-a göndərilən dəyər boş ola bilər ancaq methoda mütləq override olmalıdır.

###   Differentiate between Boxing and Unboxing.
***
> **My Answer** : **Boxing** _value type_ dəyərin _referance type_ çevirməkdən söhbət gedir.**Unboxing** _referance type_-ın _value type_-a çevirilməsindən söhbət gedir.
- Code
```c
    int value_number = 5;
    object obuekt_number = value_number;//Boxsing

    object obyeckt_number_2 = 5;
    int value_number_2=(int)obyeckt_number_2//UnBoxing

```

###   What is the difference between a struct and a class in C#?
***
> **My Answer** : `struct` `class`-in daha yüngül versiyasıdır. `struct` _value type_-dır. `class` _referance type_-dır. `struct` `class`-a nisbətən daha tez icra olunur.`struct` _constroctor_-u mütləq parametir qəbul etməlidir və yaradılarkən `new` keyword-ünə ehtiyac duymur ancaq  `class`-da belə deyil.

###   What is the difference between Interface and Abstract Class?
***
> **My Answer** : **Interface =>** Ən önəmli fərqləri `interface` `class`-lara yol göstərmək üçündür və `interface` daxilində yalnız _property_ və _method_ təyin edə bilərik. Bir `class` bir neçə `interface` `implement` edə bilərik və `interface`-lər öz daxilində bir-birilərini `implement` edə bilir.`interface` təyin edərkən `interface` _keyword_-dən istadə edilir.**Abstract Class =>** `abstract class` `class`-lar daxilində iyerarxiya yaratmaq üçün istifadə edilir. `abstract class` sadəcə sinifin sahib olduğu xususiyətləri göstərir.Məsələn bir Animals `abstract class`-ı yaradırıqsa bu `class` heyvanaların bütün xüsusiyyətlərni özünüdə toplayır.

###  What is enum in C#?
***
> **My Answer** : Programlarda sabit dəyərlərdən təkrar təkrar isfadə edildikdə bu təkrarın qaşısını almaq üçün və dəyərlərin düzgün yazılması üçün istfadə edilir.Developer istfadəsi üçündür._Value type_-dır.

- Code
```c
    enum Rənglər { yellow, yellowgreen, green };

```

###  Define Property in C# .net?
***
> **My Answer** : Bir `class`-ın daxilindəki məlumatları qorumaq üçün _Property_ istfadə edirik. _Property_ daxilində təyin edilən **get** methodu ilə uyğun(qorunan) fildi oxunur **set** methodu ilə həmin fildə informasiya yazmaq istədiyimizdə hansi hasilər baş verəcək onları yazırıq._Property_ yalnız **get** methodu ilə təyin edilə bilər o zaman bu _Property_dəki məlumat yalnız oxuna bilir.

- Code
```c

   public class User  
{  
    private string _First_Name;  
    private string _Last_Name;  
    private int _Age;  
  
    public string First_Name  
    {  
        get { return _First_Name; }  
        set { _First_Name = value; }  
    }  
  
    public string Last_Name  
    {  
        get { return _Last_Name; }  
        set { _Last_Name = value; }  
    }  
  
    public int Age  
    {  
        get { return _Age; }  
    }  

    public User(int age)
    {
        this._Age = age;
    }

}  

```

### What is sealed class in c#?
***
> **My Answer** : `sealed` keywordü işlənmiş `class` _inheritence_-da iştirak edə bilmir. Bu sayədə sabit fildlərə və methodlara sahib bir `class` əldə edirik.Məsələn `string` `obyect`
- Code
```c
namespace Sealed
{
    public sealed class User
    {
        
        public int id { get; set; }
        public string Name { get; set; }
        public string Surname { get; set; }
    }
}


public class SuperUser : User
{ }

### error
‘Project.SuperUser’:  cannot derive from sealed type ‘Project.User’
```
### What is extension method in c# and how to use them?
***
> **My Answer** : C#3.0 ilə gələn yenilikərdən biridir.Qısa izah versək `class` və `struct` daxilindəki methodlardan isfadə etmək üçün modify etməyə ehticını ardan qaldır. Və Nəticə etibarı ilə daha az kod yazmağa gətirib çıxarır.

### How to use extension methods?
***
> **My Answer** : Bu methodlar `static` `class`-ın içərisində təyin edilir və methodun ilk parametirinə `this` keywordü yazılır və yanlız bir parametrə `this`keywordü yaza bilərik.
- Code
```c
public static class MyExtensions
   {
       public static bool IsPrime(this int integer)
       {
           // some amazing code
           return true;
       }
   }
```