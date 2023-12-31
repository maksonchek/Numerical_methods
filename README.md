# Численные методы
**Привалов Максим БПМ-21-3**

### Инструкции:
1. Открыть папку в репозитории с нужным названием лабораторной.
2. Скачать .ipynb файл или перейти по ссылке в колаб ниже (Ссылки находятся напротив заголовков к лабораторным)
3. Открыть у себя на устройстве
4. Последовательно выполнить все ячейки
5. Проверить результат

## Проект: (https://github.com/zhuzzzhha/interpolation)

## Лабораторная работа 1 (https://colab.research.google.com/drive/1O-xwsTMUF_t3zbZKGp9HDddwA32UmYG5?usp=sharing):
### 1. Метод половинного деления:

**Метод бисекции или метод половинного деления** — простейший численный метод для решения нелинейных уравнений вида *f(x)=0*. Предполагается только непрерывность функции *f(x)*. Поиск основывается на теореме о промежуточных значениях.

**Теорема о промежуточном значении (или Теоре́ма Больца́но — Коши́)** утверждает, что если непрерывная функция, определённая на вещественном промежутке, принимает два значения, то она принимает и любое значение между ними.

**Математическая постановка задачи:** Дана монотонная, непрерывная функция *f(x)*, которая содержит корень/ни на отрезке *[a,b]*, где *b>a* и. 
Определить корень/ни *f(x) = 0* с точностью *?*, если известно, что *f(a)f(b)<0*

**Алгоритм**

1. Найдем середину отрезка *[a; b]*: *c=(a+b)/2*;

2. Вычислим значения функции в точках *a* и *c* и найдем произведение полученных значений: *d=f(c)?f(a)*;

3. Если *d>0*, то теперь точкой a станет *c: a=c*; Если *d<0*, то точкой *b* станет *c: b=c*;

4. Вычислим разность *a* и *b*, сравним ее с точностью *?*: если *|a-b|> ?*, то идем в пункт *1*. если нет, то корень с нужной нам точностью найден, и он равен: *x=(a+b)/2*;

### 2. Метод простой итерации:=

Пусть дано уравнение *f(x) = 0*. Мы можем преобразовать его к виду *x = g(x)*, где *g(x)* подходит для решения по методу итераций. Если мы выберем начальное приближение *x0*, общее решение может быть найдено путем последовательного применения уравнения *x = g(x)* к *x0* до тех пор, пока последующие значения x не станут достаточно близки к точному решению.

**Математическая постановка задачи**: 

Дано:

Функция f(x), для которой мы хотим найти решение уравнения f(x) = 0.
Начальное приближение x₀.
Задача:

Найти такое значение x, которое делает функцию f(x) равной нулю, то есть решить уравнение f(x) = 0.
Метод простых итераций решает эту задачу, используя итеративную формулу:

x(n+1) = g(x_n),

где x(n+1) - новое приближение, x_n - предыдущее приближение, и g(x) - выбранная функция, которая приводит к сходимости к решению уравнения f(x) = 0.

Завершение процесса:
Процесс итераций продолжается до тех пор, пока не выполнится условие сходимости. Обычно это может быть определено, например, как |x(n+1) - x_n| < ε, где ε - некоторая заданная точность, определяющая, насколько близко мы хотим приблизиться к решению.

По формуле Лагранжа: x_истин - x_(n+1) = g(x_истин) - g(x_n) = g'(x_*)(x_истин - x_n), x_* принадлежит отрезку от x_истин - x_n, тогда чтобы решение сходилось, нужно, чтобы |g'(x_*)| < 1. 
А g'(x_*) = 0, если x_* = x_истин

**Подбор функции для операции взятия корня**:
1. x = a^(1/2)
2. x^2 = a
3. 2x^2 = a + x^2
4. x = 0.5*(x+a/x) => x_(n+1) = 0.5*(x_n+a/x_n)

## Лабораторная работа 2 (https://drive.google.com/file/d/1kF8nQKY5KPRwhGmF2bg-OqO6gkq0VRUa/view?usp=sharing):
1. Метод Ньютона
2. Упрощённый метод Ньютона
3. Метод Ньютона-Бройдена
4. Метод секущих

## Лабораторная работа № 3 (https://drive.google.com/file/d/1e51IyDV-1EIR44-7JfrMpmTJ-oZn9kly/view?usp=sharing)
1. Метод Гаусса
2. Метод прямоугольников
3. Метод ведущего элемента
4. Метод простых итераций
5. Метод Зейделя

## Лабораторная работа № 4 (https://colab.research.google.com/drive/1vynfaJ5rnrC2A9fqLpK91ON-QIShyJ_5?usp=sharing)
1. Метод итераций
2. Метод вращений

## Лабораторная работа № 5 (https://colab.research.google.com/drive/1GbWb23CK7NWGSl1XNxwmUU7UqFuL5crf?usp=sharing)
1. Интерполяция многочленом Лагранжа
2. Линейная интерполяция
3. Параболическая интерполяция

## Лабораторная работа № 6
1. Многочлен Ньютона для неравномерной сетки
2. Многочлен Ньютона для равномерной сетки
3. Многочлен Ньютона 1 для равномерной сетки
4. Многочлен Ньютона 2 для равномерной сетки
 
## Лабораторная работа № 7
1. МНК
