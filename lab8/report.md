# Отчет по лабораторной работе № 5
## по курсу "Фундаментальная информатика"

Студент группы М8О-108Б-23 Ганяк Александр Олегович

Работа выполнена 

Преподаватель: каф. 806 Севастьянов Виктор Сергеевич

1. **Тема**: Системы программирования на языке С
2. **Цель работы**: Изучение конкретной системы программирования на Си и получение навыков подготовки текстов и отладка программ. 
3. **Задание (вариант №45)**:  Перевод числа из 3 системы счисления в 9 систему счисления.
4. **Идея, метод, алгоритм решения задачи**: изучить и освоить возможности лабораторной СП по содержащейся в практикуме документации и другим источникам,
   в том числе основные этапы процесса компиляции и подготовки программ к выполнению. Составить и отладить простейшую программу на Си и в терминвльном классе. Изучить различные системы программирования Cи на других платформах:
   Gnu, MS VS...
6. **Сценарий выполнения работы**:
   1. Открыли птерминал
   2. Юзаем Emacs ***.c
   3. Написали код на с
   4. сс ***.c
   5. Залили маркдаун
7. **Протокол**:
   ```
      arts@LemonCorp:~$ ls
 ld        snap     Видео       Загрузки      Музыка         'Рабочий стол'
 lol.txt   sorted   Документы   Изображения   Общедоступные   Шаблоны
arts@LemonCorp:~$ cd Документы/
arts@LemonCorp:~/Документы$ ды
ды: команда не найдена
arts@LemonCorp:~/Документы$ дыв
дыв: команда не найдена
arts@LemonCorp:~/Документы$ ls
f1.txt  f1.txt~  herniya  labspython  LemOS
arts@LemonCorp:~/Документы$ cd herniya
arts@LemonCorp:~/Документы/herniya$ ls
io1
arts@LemonCorp:~/Документы/herniya$ mkdir Oil
arts@LemonCorp:~/Документы/herniya$ cd Oil
arts@LemonCorp:~/Документы/herniya/Oil$ emacs lab8.c
Warning: Missing charsets in String to FontSet conversion
arts@LemonCorp:~/Документы/herniya/Oil$ fg
bash: fg: текущий: нет такого задания
arts@LemonCorp:~/Документы/herniya/Oil$ emacs +1 lab8.c
^Carts@LemonCorp:~/Документы/herniya/Oil$ cc lab8.c
arts@LemonCorp:~/Документы/herniya/Oil$ ls
a.out  lab8.c
arts@LemonCorp:~/Документы/herniya/Oil$ gcc -std=c99 -Wall -pedantic lab8.c
arts@LemonCorp:~/Документы/herniya/Oil$ ls
a.out  lab8.c
arts@LemonCorp:~/Документы/herniya/Oil$ emacs lab8.c
^X
^Z
[1]+  Остановлен    emacs lab8.c
arts@LemonCorp:~/Документы/herniya/Oil$ 
arts@LemonCorp:~/Документы/herniya/Oil$ gcc -std=c99 -Wall -pedantic lab8.c
lab8.c:1:3: error: stray ‘#’ in program
    1 | ad#include <stdio.h>
      |   ^
lab8.c:1:1: error: unknown type name ‘ad’
    1 | ad#include <stdio.h>
      | ^~
lab8.c:1:12: error: expected ‘=’, ‘,’, ‘;’, ‘asm’ or ‘__attribute__’ before ‘<’ token
    1 | ad#include <stdio.h>
      |            ^
arts@LemonCorp:~/Документы/herniya/Oil$ emacs lab8.c
^Z
[2]+  Остановлен    emacs lab8.c
arts@LemonCorp:~/Документы/herniya/Oil$ gcc -std=c99 -Wall -pedantic lab8.c
lab8.c:1:3: error: stray ‘#’ in program
    1 | ad#include <stdio.h>
      |   ^
lab8.c:1:1: error: unknown type name ‘ad’
    1 | ad#include <stdio.h>
      | ^~
lab8.c:1:12: error: expected ‘=’, ‘,’, ‘;’, ‘asm’ or ‘__attribute__’ before ‘<’ token
    1 | ad#include <stdio.h>
      |            ^
arts@LemonCorp:~/Документы/herniya/Oil$ emacs lab8.c
arts@LemonCorp:~/Документы/herniya/Oil$ emacs lab8.c
arts@LemonCorp:~/Документы/herniya/Oil$ emacs lab8.c
arts@LemonCorp:~/Документы/herniya/Oil$ gcc -std=c99 -Wall -pedantic lab8.c
arts@LemonCorp:~/Документы/herniya/Oil$ ls
a.out  lab8.c  lab8.c~
arts@LemonCorp:~/Документы/herniya/Oil$ gcc -std=c99 -Wall -pedantic lab8.c 2>&1 | more

























(END)
[3]+  Остановлен    gcc -std=c99 -Wall -pedantic lab8.c 2>&1 | more
arts@LemonCorp:~/Документы/herniya/Oil$ ./a.out
Hello, Viktor!
arts@LemonCorp:~/Документы/herniya/Oil$ gcc -std=c99 -Wall -pedantic lab8.c && ./a.out
Hello, Viktor!
arts@LemonCorp:~/Документы/herniya/Oil$ A
   ```
9. **Замечания автора** по существу работы: Все было ровно
10. **Выводы**: Мы научились работать Си, поняли что находиться под капотом! Написали банальный алгоритм на Си. Осознали величие emacs по сравнению со всем, что присуствует в Unix подобных системах!
