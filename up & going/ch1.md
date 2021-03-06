# You Don't Know JS: Up & Going
# Часть 1: В программирование

Добро пожаловать в серию книг You Don’t Know JS (YDKJS).

«Вперед и вверх» — представляет собой введение в некоторые базовые концепции в программировании. Конечно, далее мы будем изучать JavaScript (или сокращенно JS) прицельно, а также все необходимое для того чтобы подойти к пониманию следующих книг данной серии. Особенно, если вы только начитаете свой путь в программировании на JavaScript, эта книга коротко покажет вам все необходимое, чтобы встать и идти дальше.

Книга начинается с объяснения базовых принципов программирования на верхнем уровне. Она прежде всего предназначена людям с маленьким или же вообще без опыта программирования, которые обратились к данной серии книг за помощью на старте своего пути в понимании программирования через призму JavaScript.

Часть первая должна восприниматься как краткий обзор вещей, о которых вы бы хотели узнать подробнее, а так-же получение начальной практики в программировании. Существует множество других отличных ресурсов для новичков в JavaScript,  и я советую вам изучать и их, в дополнение к первой части нашего учебника.

Как только вы почувствуете себя комфортно с основами, часть номер два поможет вам познакомиться с  программированием под соусом JavaScript. Вторая часть расскажет вам — что такое JavaScript, но напомню, это не подробное руководство — для этих вещей есть следующие книги нашей серии!

Если вы уже чувствуете себя достаточно комфортно с JavaScript, сперва загляните в часть три данной книги, там вы найдете намек на то, что вообще ожидать от серии книг «You Dont Know JavaScript», а потом ныряйте с головой!

## КОД

Начнем с самого начала.

Программа, часто называемая как исходный код (исходник) или просто код — набор специальных инструкций которыми мы можем объяснить компьютеру, какую задачу мы хотим, чтобы он выполнил. Обычно, код сохраняется в текстовом файле, хотя в случае JavaScript вы также можете вводить его в консоли разработчика в вашем веб-браузере, о чем мы расскажем далее.

Набор правил форматирования и комбинаций таких инструкций называется языком программирования, так-же известным как синтаксис языка. Это очень близко к тому, как правила английского языка говорят вам о том как правильно писать слова и составлять из них предложения с помощью этих слов и знаков препинания.

### ИНСТРУКЦИИ

В компьютерном языке, группа слов, числа и операторы, выполняющие определенную задачу — это инструкции. В JavaScript, инструкция может выглядеть например так:

```js
a = b * 2;
```

Буквы a и b называются переменными (см. «Переменные»), это что-то вроде простых коробок, куда вы можете положить любые нужные вам вещи. В программах, в переменные кладут значения (например число 42), чтобы потом можно было достать его и использовать в программе. Думайте о них как о символически подписанных коробках.

Для контраста, число 2 это просто значение само по себе, называемое буквальным (литеральным) значением, так как оно существует само по себе и не содержится в переменной(коробке).

Знаки = и * являются операторами (см. «Операторы») — они производят действия со значениями и переменными, например действие присвоения(=) и математического умножения(*).

Большинство инструкций в JavaScript заканчиваются точкой с запятой(;) в конце.

Инструкция a = b * 2; говорит компьютеру, упрощенно — взять текущее значение, содержащееся в переменной b, умножить его на 2, затем сохранить получившийся результат в другую переменную, которая называется a.

Программа — это просто коллекция множества таких предложений, описывающая шаги, которые необходимо выполнить для достижения определенного результата.

### ВЫРАЖЕНИЯ

Предложения состоят из одного или более выражений. Выражение — это какое-либо упоминание переменной или значения, или же набора переменных или значений, соединенных операторами.

Например:
```js
a = b * 2;
```

В этом предложении четыре выражения:

* `2` выражение литерального (буквального) значения
* `b` выражение переменной, означающее — получить ее текущее значение
* `b * 2` арифметическое выражение, означающее — выполнить умножение
* `a = b * 2` выражение присвоения, означающее — присвоить результат выражения b * 2 переменной a (подробнее о присвоении чуть позже)

Выражение, стоящее отдельно называется обычно выражением-инструкцией, например:

```js
b * 2;
```

встречается не часто, т.к. оно не особо практично и в большинстве случаем не произведет никакого эффекта на работающую программу. Оно получит значение переменной b и умножит его на 2, но потом не сделает ничего с получившимся результатом.

Более частое применение выражений-инструкций — их вызов (см. «Функции»):

```js
alert( a );
```

### ВЫПОЛНЕНИЕ ПРОГРАММЫ

Как этот набор инструкций говорит компьютеру что необходимо сделать? Программа необходимо выполниться, или по-другому, ее необходимо запустить.

Инструкции вроде a = b * 2 удобны для разработчиков, когда им необходимо написать или прочитать код, но это не совсем та форма, которую может прямо понимать сам компьютер. Итак, специальная программа в компьютере (интерпретатор или компилятор) используется для перевода кода, который вы написали в команды, которые может понять ваш компьютер.

В некоторых языках программирования этот перевод обычно осуществляется сверху вниз, строка за строкой, при каждом запуске программы. Такую операцию обычно называют интерпретированием кода.

В других языках, перевод осуществляется один раз заранее, такая операция называется компилированием кода. Таким образом когда программу запустят позднее, компьютер получит заранее приготовленный и понятный ему набор команд, сразу готовый к запуску.

Часто утверждают что JavaScript — интерпретируемый язык, т.к.  исходный код на JavaScript обрабатывается каждый раз при запуске. Но это не совсем верное утверждение. Движок JavaScript на самом деле компилирует программу на лету и затем немедленно исполняет полученные команды.

**Примечание:** более подробная информация о процессе компиляции JavaScript доступна в первых двух частях книги «Scope & Closures» данной серии.

## ПОПРОБУЙ САМ

В этом разделе мы познакомимся с каждой концепцией наглядно, используя небольшие кусочки кода, написанными на JavaScript (очевидно!).

Думаю, не нужно лишний раз говорить о том, что по мере чтения данного текста, вам необходимо практиковаться в каждом из данных ниже примеров, самим набирая данный код и наблюдая за его работой. Самый простой способ сделать это — открыть консоль разработчика (developer tools console) в вашем браузере (Firefox, Chrome, IE…).

Совет: обычно вы можете запустить консоль разработчика сочетанием горячих клавиш (в Chrome Ctrl+Shift+i), или из меню браузера. Для более детальной информации о том как запустить и использовать данный инструмент можно прочитать в интернете, например «Mastering The Developer Tools Console» (http://blog.teamtreehouse.com/mastering-developer-tools-console). Чтобы набрать несколько команд за раз,  используйте <shift> + <enter> для перехода на новую строку. Если же нажать просто <enter>, консоль выполнит все, что вы до этого набрали.

Давайте познакомимся с процессом запуска кода в консоли. Сначала, я предлагаю вам открыть пустую вкладку в вашем браузере. Затем, убедитесь что консоль разработчика открыта, как было сказано ранее.

Теперь, введите этот код и посмотрите как он выполнится:

```js
a = 21;

b = a * 2;

console.log( b );
```

Консоль выведет примерно следующее:

<img src="fig1.png" width="500">

Вперед, попробуйте сами. Лучший способ научиться программированию — начать кодить!

### Вывод

В прошлом примере, мы использовали console.log(..). Коротко, давайте посмотрим что означает эта строчка кода.

Наверное, вы уже догадались, с помощью нее мы вывели текст в консоль. Есть два момента в данной инструкции, которые мы должны объяснить.

Первый — часть строки log( b ) — является вызовом функции (см. «Функции»). Что происходит? Мы передаем переменную b в данную функцию, которая берет значение, содержащееся в переменной b и выводит ее в консоль.

Второй — часть console. это ссылка на объект, в котором расположена функция log(..). Мы расскажем об объектах и их содержимом более детально во второй части.

Другой способ вывести информацию — использование инструкции alert(..). Например:

```js
alert( b );
```

Если вы запустите этот код, вы заметите, что вместо вывода в консоль, появится всплывающее окно с содержимым переменной b. Однако, использование console.log(..) в основном предпочтительнее, т.к. вы можете вывести множество значений за раз, не прерывая работы браузера.

В этой книге, мы будем использовать console.log(..) для вывода информации.

### Ввод

До сих пор мы говорили о выводе информации, давайте теперь поговорим о ее вводе (получении информации от пользователя).

Обычно для этого размещают элементы формы, с возможностью ввода текста в самом html коде страницы (такие элементы как textarea, input), а затем, используя JS, достают содержимое этих элементов и сохраняют их в переменных.

Но есть способ гораздо легче, который отлично подходит для нашей миссии — обучения и демонстрации работы программ.  Я говорю о функции prompt(..):

```js
age = prompt( "Please tell me your age:" );

console.log( age );
```

Как вы уже догадались, сообщение, которое вы передаете функции prompt(..), в данном случае «Please tell me your age:» — будет выведено на экран в сплывающем окне.

<img src="fig2.png" width="500">

Как только вы отправите введенный текст нажатием на «OK», вы увидите, что значение, которое вы только что ввели, сохранено в переменной age, содержимое которой затем выводится с помощью console.log(..):

<img src="fig3.png" width="500">

Для простоты, пока мы обучаемся базовым вещам, в примерах этой книги не будет использоваться ввод пользователя. Но теперь, когда вы узнали как использовать prompt(..), при желании, усложните себе задачу и поизучайте работу примеров, используя данную возможность.

## Операторы

Операторы и как мы производим какие-либо действия над переменными и значениями. Мы уже видели два JavaScript оператора в действии, это операторы: = и *.

Оператор * выполняет математическое умножение. Довольно просто, правда?

Оператор = используется для присвоения, сначала мы вычисляем значение с правой стороны (исходное значение) оператора =, а затем кладем его в переменную, которую мы обозначили на левой стороне.

**Внимание:** Может показаться, что операция присвоения выполняется в обратном порядке, что выглядит немного странно. Вместо a = 42, некоторым, возможно, была бы предпочтительнее запись в обратном порядке, где исходное значение писалось бы слева, а переменная справа, например 42 -> a (это не валидный JavaScript!). К сожалению, порядок a = 42, и похожих вариаций данной операции, превалирует в современных языках программирования. Выглядит не вполне естественно, просто потратьте немного вашего времени, чтобы привыкнуть к этой концепции.

Рассмотрим:

```js
a = 2;
b = a + 1;
```

Здесь мы присваиваем значение 2 переменной. Затем, мы берем значение переменной a (содержащей 2), прибавляя к ней затем 1, что в результате дает нам значение 3, затем сохраняем это значение в переменной b.

В каждой программе вам необходимо использовать ключевое слово var (технически это не оператор), в качестве основного способа объявлять (создавать) переменные (см. «Переменные»).

Вы должны всегда объявлять переменные перед их использованием. Но вам необходимо делать это всего один раз на каждую область видимости (Scope, см. «Scope»). Далее переменная может быть использована столько раз, сколько это необходимо. Например:

```js
var a = 20;

a = a + 1;
a = a * 2;

console.log( a );	// 42
```

Список наиболее часто употребляемых операторов JavaScript:

* Присвоение: `=` как в `a = 2`.
* Математические: `+` (сложение), `-` (вычитание), `*` (умножение), и `/` (деление), как в `a * 3`.
* Составное присваивание: `+=`, `-=`, `*=`, и `/=` составные операторы, которые сочетают математические операторы с присваиванием, например `a += 2` (тоже самое, что `a = a + 2`).
* Инкремент/Декремент: `++` (Инкремент), `--` (Декремент), как в `a++` (тоже самое, что `a = a + 1`).
* Доступ к свойствам объекта: `.` как в `console.log()`.

Объекты — это значения, которые содержат в себе другие значения в специальных именованных ячейках, называемых свойствами. obj.a означает значение ячейки с именем a объекта с названием obj. Свойства так-же доступны через запись obj[«a»]. Подробнее во второй части данной книги.
* Равенство: `==` (нестрогое равенство), `===` (строгое равенство), `!=` (не строгое неравенство), `!==` (строгое неравенство), как в `a == b`.

   Подробнее в «Values & Types» и второй части данной книги.
* Сравнение: `<` (меньше чем), `>` (больше чем), `<=` (меньше чем или не строго равно), `>=` (больше чем или не строго равно), как в `a <= b`.

   Подробнее в «Values & Types» и во второй части данной книги.
* Логические: `&&` (и), `||` (или), как в `a || b` выбирается a *или* b.

   Эти операторы применяются, когда необходимо проверить условия (см. «Conditionals»).

**Примечание:** Для более детального описания и использования операторов, не присутствующих в данном списке, смотрите документацию MDN's "Expressions and Operators" (https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators).

## ЗНАЧЕНИЯ И ТИПЫ

Если вы спросите продавца в магазине, торгующем сотовыми, сколько стоит понравившийся вам телефон и он вам ответит — «девяносто девять долларов», то вы получите конкретное числовое значение того, сколько вам необходимо заплатить за покупку данного аппарата. Если вы хотите купить два таких устройства, вы легко можете удвоить это значение в уме и получить значение равное 198 долларам.

Если тот же самый продавец протянет вам другой такой-же телефон, но при этом скажет что его вы можете взять бесплатно, то в этом случае вы не получите цену данного устройства в числовом формате, вместо этого стоимость 0.00 долларов будет обозначена словом «бесплатно».

Когда спросите: «Идет ли зарядка в комплекте к данному гаджету?», ответ продавца может быть только «Да» или «Нет».

Очень похожим способом, когда вы используете значения в программировании, вы выбираете различное представление этих значений, в зависимости от того, что вы планируете делать с ними далее.

Эти различные представления значений называются «Типами». В JavaScript есть встроенные типы для каждого из этих так называемых примитивных значений:

* Когда вам нужно что-то посчитать, вам нужно число (number).
* Когда вам нужно вывести значение на экран, вам нужна строка (string) — одна или более букв, слова, предложения.
* Когда вам необходимо принять решение в вашей программе, вам нужно булевое (boolean) значение — Ложь или Правда (true or false).

Значения, включенные напрямую в исходный код называются литералами. Строковые литералы обрамляются двойными «…» или одинарными (‘…’) кавычками — единственная разница между ними — вкусовые предпочтения. Числа и булевые литералы пишутся как есть(напр.: 42, true).

Наглядно:

```js
"I am a string";
'I am also a string';

42;

true;
false;
```

Кроме string/number/boolean типов, в языках программирования часто присутствуют также такие типы как: массивы (arrays), объекты (objects), функции (functions), и другие. Мы подробнее поговорим о различных типах далее.

### ПРЕОБРАЗОВАНИЕ ТИПОВ

Если у вас есть число и его необходимо вывести на экран, вам необходимо преобразовать данное значение в строку, в JavaScript это преобразование называется приведением к типу («coercion»). То есть, если кто-то ввел набор цифр в форме заказа на странице интернет магазина, это будет строкой, но если вам необходимо впоследствии выполнить какие-либо математические операции с данным значением, вам необходимо привести его к типу number (число).

JavaScript предоставляет несколько различных способов сделать это самостоятельно. например:

```js
var a = "42";
var b = Number( a );

console.log( a );	// "42"
console.log( b );	// 42
```

Использование Number(..) (встроенная функция) как в примере, является явным преобразованием из каких-либо других типов к типу number. Тут не должно возникнуть никаких сложностей в понимании.

Но вот вам спорный момент, что случится, когда вы попытаетесь сравнить два значения различных типов, которые не были преобразованы явно?

Сравнивая строку (string) «99.99» с числом (number) 99.99, большинство людей согласится — они равны. Но они не абсолютно одинаковы, верно? Это одно и тоже значение в двух различных представлениях, двух различных типов.

Чтобы помочь вам в таких частых задачах, JavaScript сделает под капотом неявное приведение к типам (implicit coerce) данных значений, чтобы их типы совпадали.

Если вы сделаете неявное сравнение оператором == значений: «99.99» == 99.99, JavaScript преобразует значение слева «99.99» в его числовой эквивалент 99.99. Далее произойдет сравнение 99.99 == 99.99, которое само собой вернО.

Созданное, чтобы помогать вам, неявное преобразование может создать путаницу и смутить вас, если вы не уделили чуточку вашего времени, чтобы изучить правила, которые управляют его поведением). Большинство JS разработчиков не уделяли), в связи с этим очень часто слышатся крики о том, что неявное преобразование зло, оно вносит путаницу и порождает неожиданные баги, и должно избегаться. Иногда даже слышны крики о том, что это ошибка в проектировании самого языка Javascript.

Тем не менее, неявное преобразование — это механизм, который может быть укрощен, более того, его должен знать каждый, кто решил взяться за JavaScript всерьез. Он не только станет понятным, после изучения, но так же сделает ваш код гораздо лучше! Игра стоит свеч.

**Примечание:** Более подробная информация о преобразовании в части 2 данной книги, а также части 4 книги Types & Grammar данной серии.

## Code Comments

The phone store employee might jot down some notes on the features of a newly released phone or on the new plans her company offers. These notes are only for the employee -- they're not for customers to read. Nevertheless, these notes help the employee do her job better by documenting the hows and whys of what she should tell customers.

One of the most important lessons you can learn about writing code is that it's not just for the computer. Code is every bit as much, if not more, for the developer as it is for the compiler.

Your computer only cares about machine code, a series of binary 0s and 1s, that comes from *compilation*. There's a nearly infinite number of programs you could write that yield the same series of 0s and 1s. The choices you make about how to write your program matter -- not only to you, but to your other team members and even to your future self.

You should strive not just to write programs that work correctly, but programs that make sense when examined. You can go a long way in that effort by choosing good names for your variables (see "Variables") and functions (see "Functions").

But another important part is code comments. These are bits of text in your program that are inserted purely to explain things to a human. The interpreter/compiler will always ignore these comments.

There are lots of opinions on what makes well-commented code; we can't really define absolute universal rules. But some observations and guidelines are quite useful:

* Code without comments is suboptimal.
* Too many comments (one per line, for example) is probably a sign of poorly written code.
* Comments should explain *why*, not *what*. They can optionally explain *how* if that's particularly confusing.

In JavaScript, there are two types of comments possible: a single-line comment and a multiline comment.

Consider:

```js
// This is a single-line comment

/* But this is
       a multiline
             comment.
                      */
```

The `//` single-line comment is appropriate if you're going to put a comment right above a single statement, or even at the end of a line. Everything on the line after the `//` is treated as the comment (and thus ignored by the compiler), all the way to the end of the line. There's no restriction to what can appear inside a single-line comment.

Consider:

```js
var a = 42;		// 42 is the meaning of life
```

The `/* .. */` multiline comment is appropriate if you have several lines worth of explanation to make in your comment.

Here's a common usage of multiline comments:

```js
/* The following value is used because
   it has been shown that it answers
   every question in the universe. */
var a = 42;
```

It can also appear anywhere on a line, even in the middle of a line, because the `*/` ends it. For example:

```js
var a = /* arbitrary value */ 42;

console.log( a );	// 42
```

The only thing that cannot appear inside a multiline comment is a `*/`, because that would be interpreted to end the comment.

You will definitely want to begin your learning of programming by starting off with the habit of commenting code. Throughout the rest of this chapter, you'll see I use comments to explain things, so do the same in your own practice. Trust me, everyone who reads your code will thank you!

## Variables

Most useful programs need to track a value as it changes over the course of the program, undergoing different operations as called for by your program's intended tasks.

The easiest way to go about that in your program is to assign a value to a symbolic container, called a *variable* -- so called because the value in this container can *vary* over time as needed.

In some programming languages, you declare a variable (container) to hold a specific type of value, such as `number` or `string`. *Static typing*, otherwise known as *type enforcement*, is typically cited as a benefit for program correctness by preventing unintended value conversions.

Other languages emphasize types for values instead of variables. *Weak typing*, otherwise known as *dynamic typing*, allows a variable to hold any type of value at any time. It's typically cited as a benefit for program flexibility by allowing a single variable to represent a value no matter what type form that value may take at any given moment in the program's logic flow.

JavaScript uses the latter approach, *dynamic typing*, meaning variables can hold values of any *type* without any *type* enforcement.

As mentioned earlier, we declare a variable using the `var` statement -- notice there's no other *type* information in the declaration. Consider this simple program:

```js
var amount = 99.99;

amount = amount * 2;

console.log( amount );		// 199.98

// convert `amount` to a string, and
// add "$" on the beginning
amount = "$" + String( amount );

console.log( amount );		// "$199.98"
```

The `amount` variable starts out holding the number `99.99`, and then holds the `number` result of `amount * 2`, which is `199.98`.

The first `console.log(..)` command has to *implicitly* coerce that `number` value to a `string` to print it out.

Then the statement `amount = "$" + String(amount)` *explicitly* coerces the `199.98` value to a `string` and adds a `"$"` character to the beginning. At this point, `amount` now holds the `string` value `"$199.98"`, so the second `console.log(..)` statement doesn't need to do any coercion to print it out.

JavaScript developers will note the flexibility of using the `amount` variable for each of the `99.99`, `199.98`, and the `"$199.98"` values. Static-typing enthusiasts would prefer a separate variable like `amountStr` to hold the final `"$199.98"` representation of the value, because it's a different type.

Either way, you'll note that `amount` holds a running value that changes over the course of the program, illustrating the primary purpose of variables: managing program *state*.

In other words, *state* is tracking the changes to values as your program runs.

Another common usage of variables is for centralizing value setting. This is more typically called *constants*, when you declare a variable with a value and intend for that value to *not change* throughout the program.

You declare these *constants*, often at the top of a program, so that it's convenient for you to have one place to go to alter a value if you need to. By convention, JavaScript variables as constants are usually capitalized, with underscores `_` between multiple words.

Here's a silly example:

```js
var TAX_RATE = 0.08;	// 8% sales tax

var amount = 99.99;

amount = amount * 2;

amount = amount + (amount * TAX_RATE);

console.log( amount );				// 215.9784
console.log( amount.toFixed( 2 ) );	// "215.98"
```

**Note:** Similar to how `console.log(..)` is a function `log(..)` accessed as an object property on the `console` value, `toFixed(..)` here is a function that can be accessed on `number` values. JavaScript `number`s aren't automatically formatted for dollars -- the engine doesn't know what your intent is and there's no type for currency. `toFixed(..)` lets us specify how many decimal places we'd like the `number` rounded to, and it produces the `string` as necessary.

The `TAX_RATE` variable is only *constant* by convention -- there's nothing special in this program that prevents it from being changed. But if the city raises the sales tax rate to 9%, we can still easily update our program by setting the `TAX_RATE` assigned value to `0.09` in one place, instead of finding many occurrences of the value `0.08` strewn throughout the program and updating all of them.

The newest version of JavaScript at the time of this writing (commonly called "ES6") includes a new way to declare *constants*, by using `const` instead of `var`:

```js
// as of ES6:
const TAX_RATE = 0.08;

var amount = 99.99;

// ..
```

Constants are useful just like variables with unchanged values, except that constants also prevent accidentally changing value somewhere else after the initial setting. If you tried to assign any different value to `TAX_RATE` after that first declaration, your program would reject the change (and in strict mode, fail with an error -- see "Strict Mode" in Chapter 2).

By the way, that kind of "protection" against mistakes is similar to the static-typing type enforcement, so you can see why static types in other languages can be attractive!

**Note:** For more information about how different values in variables can be used in your programs, see the *Types & Grammar* title of this series.

## Blocks

The phone store employee must go through a series of steps to complete the checkout as you buy your new phone.

Similarly, in code we often need to group a series of statements together, which we often call a *block*. In JavaScript, a block is defined by wrapping one or more statements inside a curly-brace pair `{ .. }`. Consider:

```js
var amount = 99.99;

// a general block
{
	amount = amount * 2;
	console.log( amount );	// 199.98
}
```

This kind of standalone `{ .. }` general block is valid, but isn't as commonly seen in JS programs. Typically, blocks are attached to some other control statement, such as an `if` statement (see "Conditionals") or a loop (see "Loops"). For example:

```js
var amount = 99.99;

// is amount big enough?
if (amount > 10) {			// <-- block attached to `if`
	amount = amount * 2;
	console.log( amount );	// 199.98
}
```

We'll explain `if` statements in the next section, but as you can see, the `{ .. }` block with its two statements is attached to `if (amount > 10)`; the statements inside the block will only be processed if the conditional passes.

**Note:** Unlike most other statements like `console.log(amount);`, a block statement does not need a semicolon (`;`) to conclude it.

## Conditionals

"Do you want to add on the extra screen protectors to your purchase, for $9.99?" The helpful phone store employee has asked you to make a decision. And you may need to first consult the current *state* of your wallet or bank account to answer that question. But obviously, this is just a simple "yes or no" question.

There are quite a few ways we can express *conditionals* (aka decisions) in our programs.

The most common one is the `if` statement. Essentially, you're saying, "*If* this condition is true, do the following...". For example:

```js
var bank_balance = 302.13;
var amount = 99.99;

if (amount < bank_balance) {
	console.log( "I want to buy this phone!" );
}
```

The `if` statement requires an expression in between the parentheses `( )` that can be treated as either `true` or `false`. In this program, we provided the expression `amount < bank_balance`, which indeed will either evaluate to `true` or `false` depending on the amount in the `bank_balance` variable.

You can even provide an alternative if the condition isn't true, called an `else` clause. Consider:

```js
const ACCESSORY_PRICE = 9.99;

var bank_balance = 302.13;
var amount = 99.99;

amount = amount * 2;

// can we afford the extra purchase?
if ( amount < bank_balance ) {
	console.log( "I'll take the accessory!" );
	amount = amount + ACCESSORY_PRICE;
}
// otherwise:
else {
	console.log( "No, thanks." );
}
```

Here, if `amount < bank_balance` is `true`, we'll print out `"I'll take the accessory!"` and add the `9.99` to our `amount` variable. Otherwise, the `else` clause says we'll just politely respond with `"No, thanks."` and leave `amount` unchanged.

As we discussed in "Values & Types" earlier, values that aren't already of an expected type are often coerced to that type. The `if` statement expects a `boolean`, but if you pass it something that's not already `boolean`, coercion will occur.

JavaScript defines a list of specific values that are considered "falsy" because when coerced to a `boolean`, they become `false` -- these include values like `0` and `""`. Any other value not on the "falsy" list is automatically "truthy" -- when coerced to a `boolean` they become `true`. Truthy values include things like `99.99` and `"free"`. See "Truthy & Falsy" in Chapter 2 for more information.

*Conditionals* exist in other forms besides the `if`. For example, the `switch` statement can be used as a shorthand for a series of `if..else` statements (see Chapter 2). Loops (see "Loops") use a *conditional* to determine if the loop should keep going or stop.

**Note:** For deeper information about the coercions that can occur implicitly in the test expressions of *conditionals*, see Chapter 4 of the *Types & Grammar* title of this series.

## Loops

During busy times, there's a waiting list for customers who need to speak to the phone store employee. While there's still people on that list, she just needs to keep serving the next customer.

Repeating a set of actions until a certain condition fails -- in other words, repeating only while the condition holds -- is the job of programming loops; loops can take different forms, but they all satisfy this basic behavior.

A loop includes the test condition as well as a block (typically as `{ .. }`). Each time the loop block executes, that's called an *iteration*.

For example, the `while` loop and the `do..while` loop forms illustrate the concept of repeating a block of statements until a condition no longer evaluates to `true`:

```js
while (numOfCustomers > 0) {
	console.log( "How may I help you?" );

	// help the customer...

	numOfCustomers = numOfCustomers - 1;
}

// versus:

do {
	console.log( "How may I help you?" );

	// help the customer...

	numOfCustomers = numOfCustomers - 1;
} while (numOfCustomers > 0);
```

The only practical difference between these loops is whether the conditional is tested before the first iteration (`while`) or after the first iteration (`do..while`).

In either form, if the conditional tests as `false`, the next iteration will not run. That means if the condition is initially `false`, a `while` loop will never run, but a `do..while` loop will run just the first time.

Sometimes you are looping for the intended purpose of counting a certain set of numbers, like from `0` to `9` (ten numbers). You can do that by setting a loop iteration variable like `i` at value `0` and incrementing it by `1` each iteration.

**Warning:** For a variety of historical reasons, programming languages almost always count things in a zero-based fashion, meaning starting with `0` instead of `1`. If you're not familiar with that mode of thinking, it can be quite confusing at first. Take some time to practice counting starting with `0` to become more comfortable with it!

The conditional is tested on each iteration, much as if there is an implied `if` statement inside the loop.

We can use JavaScript's `break` statement to stop a loop. Also, we can observe that it's awfully easy to create a loop that would otherwise run forever without a `break`ing mechanism.

Let's illustrate:

```js
var i = 0;

// a `while..true` loop would run forever, right?
while (true) {
	// stop the loop?
	if ((i <= 9) === false) {
		break;
	}

	console.log( i );
	i = i + 1;
}
// 0 1 2 3 4 5 6 7 8 9
```

**Warning:** This is not necessarily a practical form you'd want to use for your loops. It's presented here for illustration purposes only.

While a `while` (or `do..while`) can accomplish the task manually, there's another syntactic form called a `for` loop for just that purpose:

```js
for (var i = 0; i <= 9; i = i + 1) {
	console.log( i );
}
// 0 1 2 3 4 5 6 7 8 9
```

As you can see, in both cases the conditional `i <= 9` is `true` for the first 10 iterations (`i` of values `0` through `9`) of either loop form, but becomes `false` once `i` is value `10`.

The `for` loop has three clauses: the initialization clause (`var i=0`), the conditional test clause (`i <= 9`), and the update clause (`i = i + 1`). So if you're going to do counting with your loop iterations, `for` is a more compact and often easier form to understand and write.

There are other specialized loop forms that are intended to iterate over specific values, such as the properties of an object (see Chapter 2) where the implied conditional test is just whether all the properties have been processed. The "loop until a condition fails" concept holds no matter what the form of the loop.

## Functions

The phone store employee probably doesn't carry around a calculator to figure out the taxes and final purchase amount. That's a task she needs to define once and reuse over and over again. Odds are, the company has a checkout register (computer, tablet, etc.) with those "functions" built in.

Similarly, your program will almost certainly want to break up the code's tasks into reusable pieces, instead of repeatedly repeating yourself repetitiously (pun intended!). The way to do this is to define a `function`.

A function is generally a named section of code that can be "called" by name, and the code inside it will be run each time. Consider:

```js
function printAmount() {
	console.log( amount.toFixed( 2 ) );
}

var amount = 99.99;

printAmount(); // "99.99"

amount = amount * 2;

printAmount(); // "199.98"
```

Functions can optionally take arguments (aka parameters) -- values you pass in. And they can also optionally return a value back.

```js
function printAmount(amt) {
	console.log( amt.toFixed( 2 ) );
}

function formatAmount() {
	return "$" + amount.toFixed( 2 );
}

var amount = 99.99;

printAmount( amount * 2 );		// "199.98"

amount = formatAmount();
console.log( amount );			// "$99.99"
```

The function `printAmount(..)` takes a parameter that we call `amt`. The function `formatAmount()` returns a value. Of course, you can also combine those two techniques in the same function.

Functions are often used for code that you plan to call multiple times, but they can also be useful just to organize related bits of code into named collections, even if you only plan to call them once.

Consider:

```js
const TAX_RATE = 0.08;

function calculateFinalPurchaseAmount(amt) {
	// calculate the new amount with the tax
	amt = amt + (amt * TAX_RATE);

	// return the new amount
	return amt;
}

var amount = 99.99;

amount = calculateFinalPurchaseAmount( amount );

console.log( amount.toFixed( 2 ) );		// "107.99"
```

Although `calculateFinalPurchaseAmount(..)` is only called once, organizing its behavior into a separate named function makes the code that uses its logic (the `amount = calculateFinal...` statement) cleaner. If the function had more statements in it, the benefits would be even more pronounced.

### Scope

If you ask the phone store employee for a phone model that her store doesn't carry, she will not be able to sell you the phone you want. She only has access to the phones in her store's inventory. You'll have to try another store to see if you can find the phone you're looking for.

Programming has a term for this concept: *scope* (technically called *lexical scope*). In JavaScript, each function gets its own scope. Scope is basically a collection of variables as well as the rules for how those variables are accessed by name. Only code inside that function can access that function's *scoped* variables.

A variable name has to be unique within the same scope -- there can't be two different `a` variables sitting right next to each other. But the same variable name `a` could appear in different scopes.

```js
function one() {
	// this `a` only belongs to the `one()` function
	var a = 1;
	console.log( a );
}

function two() {
	// this `a` only belongs to the `two()` function
	var a = 2;
	console.log( a );
}

one();		// 1
two();		// 2
```

Also, a scope can be nested inside another scope, just like if a clown at a birthday party blows up one balloon inside another balloon. If one scope is nested inside another, code inside the innermost scope can access variables from either scope.

Consider:

```js
function outer() {
	var a = 1;

	function inner() {
		var b = 2;

		// we can access both `a` and `b` here
		console.log( a + b );	// 3
	}

	inner();

	// we can only access `a` here
	console.log( a );			// 1
}

outer();
```

Lexical scope rules say that code in one scope can access variables of either that scope or any scope outside of it.

So, code inside the `inner()` function has access to both variables `a` and `b`, but code in `outer()` has access only to `a` -- it cannot access `b` because that variable is only inside `inner()`.

Recall this code snippet from earlier:

```js
const TAX_RATE = 0.08;

function calculateFinalPurchaseAmount(amt) {
	// calculate the new amount with the tax
	amt = amt + (amt * TAX_RATE);

	// return the new amount
	return amt;
}
```

The `TAX_RATE` constant (variable) is accessible from inside the `calculateFinalPurchaseAmount(..)` function, even though we didn't pass it in, because of lexical scope.

**Note:** For more information about lexical scope, see the first three chapters of the *Scope & Closures* title of this series.

## Practice

There is absolutely no substitute for practice in learning programming. No amount of articulate writing on my part is alone going to make you a programmer.

With that in mind, let's try practicing some of the concepts we learned here in this chapter. I'll give the "requirements," and you try it first. Then consult the code listing below to see how I approached it.

* Write a program to calculate the total price of your phone purchase. You will keep purchasing phones (hint: loop!) until you run out of money in your bank account. You'll also buy accessories for each phone as long as your purchase amount is below your mental spending threshold.
* After you've calculated your purchase amount, add in the tax, then print out the calculated purchase amount, properly formatted.
* Finally, check the amount against your bank account balance to see if you can afford it or not.
* You should set up some constants for the "tax rate," "phone price," "accessory price," and "spending threshold," as well as a variable for your "bank account balance.""
* You should define functions for calculating the tax and for formatting the price with a "$" and rounding to two decimal places.
* **Bonus Challenge:** Try to incorporate input into this program, perhaps with the `prompt(..)` covered in "Input" earlier. You may prompt the user for their bank account balance, for example. Have fun and be creative!

OK, go ahead. Try it. Don't peek at my code listing until you've given it a shot yourself!

**Note:** Because this is a JavaScript book, I'm obviously going to solve the practice exercise in JavaScript. But you can do it in another language for now if you feel more comfortable.

Here's my JavaScript solution for this exercise:

```js
const SPENDING_THRESHOLD = 200;
const TAX_RATE = 0.08;
const PHONE_PRICE = 99.99;
const ACCESSORY_PRICE = 9.99;

var bank_balance = 303.91;
var amount = 0;

function calculateTax(amount) {
	return amount * TAX_RATE;
}

function formatAmount(amount) {
	return "$" + amount.toFixed( 2 );
}

// keep buying phones while you still have money
while (amount < bank_balance) {
	// buy a new phone!
	amount = amount + PHONE_PRICE;

	// can we afford the accessory?
	if (amount < SPENDING_THRESHOLD) {
		amount = amount + ACCESSORY_PRICE;
	}
}

// don't forget to pay the government, too
amount = amount + calculateTax( amount );

console.log(
	"Your purchase: " + formatAmount( amount )
);
// Your purchase: $334.76

// can you actually afford this purchase?
if (amount > bank_balance) {
	console.log(
		"You can't afford this purchase. :("
	);
}
// You can't afford this purchase. :(
```

**Note:** The simplest way to run this JavaScript program is to type it into the developer console of your nearest browser.

How did you do? It wouldn't hurt to try it again now that you've seen my code. And play around with changing some of the constants to see how the program runs with different values.

## Review

Learning programming doesn't have to be a complex and overwhelming process. There are just a few basic concepts you need to wrap your head around.

These act like building blocks. To build a tall tower, you start first by putting block on top of block on top of block. The same goes with programming. Here are some of the essential programming building blocks:

* You need *operators* to perform actions on values.
* You need values and *types* to perform different kinds of actions like math on `number`s or output with `string`s.
* You need *variables* to store data (aka *state*) during your program's execution.
* You need *conditionals* like `if` statements to make decisions.
* You need *loops* to repeat tasks until a condition stops being true.
* You need *functions* to organize your code into logical and reusable chunks.

Code comments are one effective way to write more readable code, which makes your program easier to understand, maintain, and fix later if there are problems.

Finally, don't neglect the power of practice. The best way to learn how to write code is to write code.

I'm excited you're well on your way to learning how to code, now! Keep it up. Don't forget to check out other beginner programming resources (books, blogs, online training, etc.). This chapter and this book are a great start, but they're just a brief introduction.

The next chapter will review many of the concepts from this chapter, but from a more JavaScript-specific perspective, which will highlight most of the major topics that are addressed in deeper detail throughout the rest of the series.
