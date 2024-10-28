# Ответы на вопросы из 3 теста Чабанова

## Вопросы
1) Дан фрагмент кода на С++. Выберите все верные утверждения:
```cpp
int i = 10;
int j = 20;
int* pi = &i;
pi = &j;
*pi = 30;
```
Ответ: <code> j станет равно 30 </code>

2) Язык С++. Дан код:
```cpp
int array[3] = {5, 1, 3};
int* i = &array[1];
++*i;
std::cout << i[0];
```
Что будет выведено в результате?<br>
Ответ: <code> 2 </code>

3) Язык С++. Дан код:
```cpp
int array[3] = {5, 1, 3};
int* i = &array[1];
cout << i[-1];
```
Что будет выведено в результате?<br>
Ответ: <code> 5 </code>

4) Дан фрагмент кода на С++:
```cpp
int* i = new int{10};
```
Выберите все верные утверждения.<br>
Ответ: <code> new выделяет память под переменную в куче </code>

5) Дан фрагмент кода на С++:
```cpp
struct Point{
    short x;
    int y;
} p{0, 0};

Point* ptr = &p;
```
Выберите все варианты позволяющие получить доступ к полю x структуры p.<br>
Ответ: <code> ptr->x; </code><br>
<code> (*ptr).x; </code>

6) Язык С++. Переменная-указатель p хранит адрес некоторой переменной <code>i</code>. Как получить доступ к значению переменной <code>i</code> по её адресу?<br>

Ответ: <code> Применить к p оператор разыменования </code>

7) Язык С++. Выберите все верные утверждения:<br>

Ответ: <code> sizeof(int *) == sizeof(double *) </code><br>
<code> sizeof(int *) == sizeof(vector<int*> *) </code><br>
<code> sizeof(int *) == sizeof(vector<int> *) </code><br>
<code> sizeof(int *) == sizeof(void *) </code>

8) Дан фрагмент кода на языке С++:
```cpp
int b[8][4][2];
```
Выберите все допустимые выражения.<br>
Ответ: <code> int (*i)[4][2] = b; </code>

9) Дана функция на С++:
```cpp
int* foo(){
    int a = 10;
    return &a;
}
```
Выберите все верные утверждения о выражении:<br>
```cpp
int* p = foo();
```
Ответ: <code> p - висячий указатель </code>

10) Дан фрагмент кода на С++:
```cpp
struct A{
};

struct B: A{
};

struct C: B{
};

A objectA;
B objectB;
C objectC;
```
Выберите все выражения, которые не вызовут ошибки.<br>

Ответ: <code> A* ab = &objectB; </code><br>
<code> B* bc = &objectC; </code><br>
<code> A* ac = &objectC; </code>

11) Язык С++. Дан код:
```cpp
int array[3] = {5, 1, 3};
int* i = &array[1];
cout << *(i+1);
```
Что будет выведено в результате?<br>

Ответ: <code> 3 </code>

12) Язык С++. Выберите все верные утверждения.
```cpp
int const i = 1;
```
Что будет выведено в результате?<br>

Ответ: <code> указатель на i может быть объявлен как const int * pi = &i; </code><br>
<code> указатель на i может быть объявлен как int const * const pi = &i; </code><br>
<code> указатель на i может быть объявлен как int const * pi = &i; </code>

13) Язык С++. Известно, что размер типа int в системе равен 4 байта. Дан код:
```cpp
int a = 10;
int* i = &a;
i += 10;
```
На сколько байт сдвинется указатель?<br>

Ответ: <code> 40 </code>

14) Язык С++. Известно, что переменные объявлены следующим образом:
```cpp
int i = 10;
int *p = &i;
```
Выберите все верные утверждения.<br>

Ответ: <code> p - это указатель на int </code>

15) Каким образом можно преобразовать <code>int* i</code> в <code>double* j</code> ?

Ответ: <code> Это невозможно сделать указанными способами </code>

16) Язык С++. Какой тип данных у переменной <code>pj</code>?
```cpp
int i = 10;
int* pi = &i, pj;
```
Ответ: <code> Просто int </code>

17) Дан фрагмент кода на языке С++:
```cpp
int* p = new int{5};
```
Ответ: <code> delete p; </code>

18) Язык С++. Дан код:
```cpp
int array[3] = {5, 1, 3};
int* i = &array[1];
*++i;
std::cout << i[0];
```
Что будет выведено в результате?<br>

Ответ: <code> 3 </code>

19) Дан фрагмент кода на языке С++. Выберите верные утверждения:
```cpp
int const * p;
```

Ответ: <code> p - это указатель на константный int </code>

20) Язык С++. Дана переменная <code>int i = 10;</code> выберите выражения НЕ вызывающие ошибки:<br>

Ответ: <code> void* a = &i; </code><br>
<code> int* a = &i; </code>

21) Дан фрагмент кода на С++:
```cpp
struct Point{
    short x;
    int y;
} p{0, 0};

Point& ptr = p;
```
Выберите все варианты позволяющие получить доступ к полю x структуры p.<br>

Ответ: <code> ptr.x; </code>

22) Язык С++. Нулевой указатель должен быть инициализирован значением:<br>

Ответ: <code> nullptr </code>

23) Дан фрагмент кода на языке С++:
```cpp
int* p = new int[5] {1, 2, 3, 4, 5};
```
Какой оператор нужно использовать, чтобы освободить выделенную память?<br>

Ответ: <code> delete[] p; </code>

24) Язык С++. Выберите все верные утверждения.
```cpp
int const * const pi = &i;
```
Ответ: <code> i может быть объявлена как int i; </code><br>
<code> Значение pi нельзя менять </code><br>
<code> i может быть объявлена как int const i; </code><br>

25) Язык С++. На какой знак нужно заменить символ # в данном фрагменте кода, чтобы pj стал указателем на int?
```cpp
int i = 10, j = 20;
int* pi, #pj = &j;
```
Ответ: <code> # заменить на * </code>

26) Язык С++. Даны два указателя int* a и int* b. Известно, что в системе тип int занимает 4 байта, а расстояние между указателями 16 байт. Какое число выведется на экран в результате команды:
```cpp
cout << b - a;
```
Ответ: <code> 4 </code>

27) Дан фрагмент кода на С++. Выберите все верные утверждения:
```cpp
int i = 10;
int* pi = &i;
int* pj = &i;
```
Ответ: <code> При помощи указателя pj можно получить доступ к переменной i </code><br>
<code> Выражение pi == pj истинно </code><br>
<code> При помощи указателя pi можно получить доступ к переменной i </code>

28) Дан фрагмент кода на языке С++:
```cpp
int i = 10;
int *p = &i;
std::cout << *p;
```
Ответ: <code> Результат выражения *p в 3й строке - целое число </code><br>
<code> p - хранит адрес переменной i </code><br>
<code> Результат выражения &i во 2й строке - адрес </code><br>
<code> На экране появится 10 </code>

29) Язык С++. Известно, что переменные объявлены следующим образом:
```cpp
int i = 10;
int *p = &i;
```
Ответ: <code> * - часть описания типа переменной </code><br>
<code> & - оператор взятия адреса </code>

30) Язык С++. Указатель объявлен следующим образом:<br>
```cpp
int* i;
```
Какие из следующих утверждений верные?<br>

Ответ:
```cpp
int one;
i = &one;
```
```cpp
int one[10];
i = &one[0];
```
```cpp
int one[10];
i = &one;
```

31) Язык С++. Выберите все выражения НЕ приводящие к ошибке.
```cpp
int i = 10;
double k = 10;
int *a;
double *b;
```
Ответ: <code> a = &i; </code><br>
<code> *b = *a; </code><br>
<code> b = &k; </code>

32) Язык С++. Выберите все допустимые варианты создания ссылок.<br>

Ответ:
```cpp
int& b = /* инициализатор */;
```
```cpp
int (&d)[10] = /* инициализатор */;
```
```cpp
int& *f = /* инициализатор */;
```

33) Язык С++. В функцию foo передаётся переменная a, значение которой НЕ равно 10. Какие функций приведут к изменению значения a ?<br>

Ответ:
```cpp
void foo(int* i){
    *i = 10;
}
```

34) Дан фрагмент кода на С++:
```cpp
int array[7] = {-3, -2, -1, 0, 1, 2, 3};
int* p = array;
while(*p++) std::cout << '+';
```
Сколько символов '+' отобразится на экране.<br>

Ответ: <code> 3 </code>

35) Дан фрагмент кода на С++:
```cpp
int i = 10;
```
Выберите все верные утверждения.

Ответ: <code> Память под переменную выделена в сегменте данных, если она глобальная </code><br>
<code> Память под переменную выделена на стеке, если она локальная </code>

36) Дана функция на С++:
```cpp
int* foo(){
    return new int{10};
}
```
Выберите все верные утверждения о выражении:
```cpp
int* p = foo();
```
Ответ: <code> Нужно освободить память командой delete p </code><br>
 <code> p равно 10 </code><br>
  <code> *p равно 10 </code>
