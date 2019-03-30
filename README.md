# Labka-3.1-v.1

Варіант 57: 
Обробляється один «перший» об’єкт і послідовність «других» об’єктів. «Перший» – це об’єкт, заданий більшою кількістю чисел, ніж другий. Виводиться результат обробки кожного з «других» об’єктів. 
1.	Визначити, як розташована пряма відносно трикутника – а) нема спільних точок, б) є одна спільна точка, в) одна зі сторін належить прямій, г) трикутник перетинається прямою. 

Написати програму, яка використовує клас точок на площині й, можливо, залежно від варіанту, інші класи. Програма багаторазово отримує набори точок, що утворюють один або кілька геометричних об’єктів на площині (залежно від варіанту завдання, це пряма, відрізок, ламана, трикутник тощо), визначає його (їх) властивості та виводить результати. 
Вимоги до виконання 
1.	Реалізувати програму за допомогою проекту, що містить п'ять файлів. У файлі g2.h записати клас точок і, можливо (залежно від варіанту), класи інших геометричних об’єктів на площині, у файлі g2.cpp – методи цих класів. У файлі g2use.h записати прототипи інших підпрограм, які працюють з геометричними об’єктами, у файлі g2use.cpp – самі ці підпрограми. У головному файлі записати головну функцію й, можливо, допоміжні до неї, не зв’язані з обробкою геометричних об’єктів. 
2.	Послідовність екземплярів вхідних даних записано у файлі. Гарантовано, що вхідний файл містить коректні числові константи, розділені пробілами та кінцями рядків. Кількість геометричних об’єктів у файлі не задано, а закінчення даних визначається кінцем файлу. Результати обробки виводяться в інший файл.
3.	Головна функція викликає функцію, яка виводить прізвище студента-виконавця й позначення завдання у варіанті кількома словами. Далі головна функція двічі викликає функцію отримання шляху до файлу (для вхідних і вихідних даних), а потім функцію processData, параметризовану вхідним і вихідним потоками типу ifstream і ofstream. 
4.	Функція отримання шляху до файлу виводить запрошення до введення шляху та повертає отриманий рядок. Якщо користувач задав порожній шлях до вхідного файлу, то дані вводяться з файлу in.txt, а якщо порожній шлях до вихідного файлу, то дані виводяться у файл out.txt. Якщо вхідний потік не відкрився успішно, то програма повертає користувача до введення шляху до вхідного файлу. 
5.	Функція processData багаторазово отримує з файлу екземпляр вхідних даних, формує необхідні геометричні об'єкти, викликає функцію їх обробки для розв'язання задачі, вказаної у варіанті, отримує результат і викликає функцію виведення результатів у вихідний файл. 
6.	У класі точок означити: конструктор без параметрів, конструктор з двома дійсними параметрами, методи отримання окремих координат точки, присвоювання =, порівняння == та !=. Приховані координати точок мають тип double. Залежно від варіанту, можливі й інші методи, як відкриті, так і приховані (допоміжні). 
7.	Залежно від варіанту, можливо, в аналогічний спосіб означити клас (класи) інших об’єктів (відрізків, прямих, трикутників тощо). Не оголошувати його як дружній у класі точок. Пряма або відрізок визначаються парою різних точок. В роботі з прямими та відрізками врахувати: точки, які мають їх зображувати, можуть збігатися. Пара однакових точок не задає пряму, але визначає відрізок довжини 0. 
8.	Якщо в програмі означено клас точок, відрізків, прямих тощо, то для введення з потоку та виведення в потік означити окремі функції введення та виведення, не оголошуючи їх як дружні у класі геометричних об'єктів. 
9.	Функція виведення результатів обробки виводить у файл зображення геометричного об'єкта (або об'єктів) та після двокрапки результати його (їх) обробки. 
10.	Створити два текстових файли: один містить вхідні дані, інший – ці самі дані та додатково правильні результати їх обробки. 
