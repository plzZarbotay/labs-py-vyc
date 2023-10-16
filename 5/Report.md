# Отчет по лабораторной работе № 5
## по курсу "Фундаментальная информатика"

Студент группы М8О-108Б-23 Ганяк Александр Олегович

Работа выполнена 

Преподаватель: каф. 806 Севастьянов Виктор Сергеевич

1. **Тема**: Машины Тьюринга
2. **Цель работы**: Написать на предоставленном Эмуляторе машины Тьюринга в  четверках.
3. **Задание (вариант №45)**:  Перевод числа из 3 системы счисления в 9 систему счисления.
4. **Идея, метод, алгоритм решения задачи**: Изучили как работает Машина Тьюринга на базовом уровне, чтобв научиться писать программу ==> Придумали алгоритм для своего варианта ==> реализовали его на предоставленном Эмуляторе машины Тьюринга в  четверках выполнили задания варианта.
5. **Сценарий выполнения работы**:
   1. Открыли предоставленный Эмулятор машины Тьюринга в  четверках
   2. Придумали алгоритм для своего варианта\
   3. Написали алгоритм
   4. Протестировать
   5. Залили маркдаун
7. **Протокол**:
   ```
    00, ,<,start

start,2,<,2_checked
start,1,<,2_checked
start,0,<,2_checked
start, ,>,new_start


2_checked,1,<,start
2_checked,2,<,start
2_checked,0,<,start
2_checked, ,>,true_start_2

true_start_2,2, ,true_start_write_2
true_start_2,1, ,true_start_write_1
true_start_2,0, ,true_start_write_001

#Первый Ноль
true_start_write_001, ,>,true_start_write_001_001
true_start_write_001_001,2,>,true_start_write_001_001
true_start_write_001_001,1,>,true_start_write_001_001
true_start_write_001_001,0,>,true_start_write_001_001
true_start_write_001_001, ,>,true_start_write_001_001_true
true_start_write_001_001_true, ,0,true_start_write_001_001_yes
true_start_write_001_001_yes,0,<,true_start_write_001_001_yes
true_start_write_001_001_yes, ,<,true_start_write_001_001_ye
true_start_write_001_001_ye,2,<,true_start_write_001_001_ye
true_start_write_001_001_ye,0,<,true_start_write_001_001_ye
true_start_write_001_001_ye,1,<,true_start_write_001_001_ye
true_start_write_001_001_ye, ,0,true_start_write_001_001_yeo
true_start_write_001_001_yeo,0,>,new_start

#Первая единица
true_start_write_1, ,>,true_start_write_1_1
true_start_write_1_1,2,>,true_start_write_1_1
true_start_write_1_1,1,>,true_start_write_1_1
true_start_write_1_1,0,>,true_start_write_1_1
true_start_write_1_1, ,>,true_start_write_1_1_true
true_start_write_1_1_true, ,1,true_start_write_1_1_yes
true_start_write_1_1_yes,1,<,true_start_write_1_1_yes
true_start_write_1_1_yes, ,<,true_start_write_1_1_ye
true_start_write_1_1_ye,2,<,true_start_write_1_1_ye
true_start_write_1_1_ye,0,<,true_start_write_1_1_ye
true_start_write_1_1_ye,1,<,true_start_write_1_1_ye
true_start_write_1_1_ye, ,1,true_start_write_1_1_yeo
true_start_write_1_1_yeo,1,>,new_start

#Первая двойка
true_start_write_2, ,>,true_start_write_2_1
true_start_write_2_1,2,>,true_start_write_2_1
true_start_write_2_1,1,>,true_start_write_2_1
true_start_write_2_1,0,>,true_start_write_2_1
true_start_write_2_1, ,>,true_start_write_2_1_true
true_start_write_2_1_true, ,2,true_start_write_2_1_yes
true_start_write_2_1_yes,2,<,true_start_write_2_1_yes
true_start_write_2_1_yes, ,<,true_start_write_2_1_ye
true_start_write_2_1_ye,2,<,true_start_write_2_1_ye
true_start_write_2_1_ye,0,<,true_start_write_2_1_ye
true_start_write_2_1_ye,1,<,true_start_write_2_1_ye
true_start_write_2_1_ye, ,2,true_start_write_2_1_yeo
true_start_write_2_1_yeo,2,>,new_start



new_start,1, ,1_check_this_tmp
new_start,2, ,2_check_this_tmp
new_start,0, ,0_check_this_tmp


#ЛАСТ ДЭЙ ИН ЗИС АЙЛОНД!

new_start, ,>,skip_to_finish

skip_to_finish,8,>,skip_to_finish
skip_to_finish,7,>,skip_to_finish
skip_to_finish,6,>,skip_to_finish
skip_to_finish,5,>,skip_to_finish
skip_to_finish,4,>,skip_to_finish
skip_to_finish,3,>,skip_to_finish
skip_to_finish,2,>,skip_to_finish
skip_to_finish,1,>,skip_to_finish
skip_to_finish,0,>,skip_to_finish
skip_to_finish, ,#,skip_to_finish


0_check_this_tmp, ,>,0_check_this
1_check_this_tmp, ,>,1_check_this
2_check_this_tmp, ,>,2_check_this

0_check_this,0, ,its_00_check_this_tmp
0_check_this,1, ,its_01_check_this_tmp
0_check_this,2, ,its_02_check_this_tmp

1_check_this,2, ,its_12_check_this_tmp
1_check_this,1, ,its_11_check_this_tmp
1_check_this,0, ,its_10_check_this_tmp

2_check_this,0, ,its_20_check_this_tmp
2_check_this,1, ,its_21_check_this_tmp
2_check_this,2, ,its_22_check_this_tmp





# 00 КОМБ
its_00_check_this_tmp, ,>,its_00_check_this
its_00_check_this,2,>,its_00_check_this
its_00_check_this,1,>,its_00_check_this
its_00_check_this,0,>,its_00_check_this
its_00_check_this, ,>,its_00_check_this_1

its_00_check_this_1,8,>,its_00_check_this_1
its_00_check_this_1,7,>,its_00_check_this_1
its_00_check_this_1,6,>,its_00_check_this_1
its_00_check_this_1,5,>,its_00_check_this_1
its_00_check_this_1,4,>,its_00_check_this_1
its_00_check_this_1,3,>,its_00_check_this_1
its_00_check_this_1,2,>,its_00_check_this_1
its_00_check_this_1,1,>,its_00_check_this_1
its_00_check_this_1,0,>,its_00_check_this_1

its_00_check_this_1, ,=,its_00_check_write_5
its_00_check_write_5, ,0,true_start_write_00_1_yes

true_start_write_00_1_yes,8,<,true_start_write_00_1_yes
true_start_write_00_1_yes,7,<,true_start_write_00_1_yes
true_start_write_00_1_yes,6,<,true_start_write_00_1_yes
true_start_write_00_1_yes,5,<,true_start_write_00_1_yes
true_start_write_00_1_yes,4,<,true_start_write_00_1_yes
true_start_write_00_1_yes,3,<,true_start_write_00_1_yes
true_start_write_00_1_yes,2,<,true_start_write_00_1_yes
true_start_write_00_1_yes,1,<,true_start_write_00_1_yes
true_start_write_00_1_yes,0,<,true_start_write_00_1_yes
true_start_write_00_1_yes, ,<,true_start_write_00_1_ye

true_start_write_00_1_ye,2,<,true_start_write_00_1_ye
true_start_write_00_1_ye,1,<,true_start_write_00_1_ye
true_start_write_00_1_ye,0,<,true_start_write_00_1_ye
true_start_write_00_1_ye, ,<,true_start_write_00_1_ye_1
true_start_write_00_1_ye_1, ,0,true_start_write_00_1_ye_2
true_start_write_00_1_ye_2,0,>,true_start_write_00_1_ye_3
true_start_write_00_1_ye_3, ,0,true_start_write_00_1_ye_4
true_start_write_00_1_ye_4,0,>,new_start


# 01 КОМБ
its_01_check_this_tmp, ,>,its_01_check_this
its_01_check_this,2,>,its_01_check_this
its_01_check_this,1,>,its_01_check_this
its_01_check_this,0,>,its_01_check_this
its_01_check_this, ,>,its_01_check_this_1

its_01_check_this_1,8,>,its_01_check_this_1
its_01_check_this_1,7,>,its_01_check_this_1
its_01_check_this_1,6,>,its_01_check_this_1
its_01_check_this_1,5,>,its_01_check_this_1
its_01_check_this_1,4,>,its_01_check_this_1
its_01_check_this_1,3,>,its_01_check_this_1
its_01_check_this_1,2,>,its_01_check_this_1
its_01_check_this_1,1,>,its_01_check_this_1
its_01_check_this_1,0,>,its_01_check_this_1

its_01_check_this_1, ,=,its_01_check_write_5
its_01_check_write_5, ,1,true_start_write_01_1_yes

true_start_write_01_1_yes,8,<,true_start_write_01_1_yes
true_start_write_01_1_yes,7,<,true_start_write_01_1_yes
true_start_write_01_1_yes,6,<,true_start_write_01_1_yes
true_start_write_01_1_yes,5,<,true_start_write_01_1_yes
true_start_write_01_1_yes,4,<,true_start_write_01_1_yes
true_start_write_01_1_yes,3,<,true_start_write_01_1_yes
true_start_write_01_1_yes,2,<,true_start_write_01_1_yes
true_start_write_01_1_yes,1,<,true_start_write_01_1_yes
true_start_write_01_1_yes,0,<,true_start_write_01_1_yes
true_start_write_01_1_yes, ,<,true_start_write_01_1_ye

true_start_write_01_1_ye,2,<,true_start_write_01_1_ye
true_start_write_01_1_ye,1,<,true_start_write_01_1_ye
true_start_write_01_1_ye,0,<,true_start_write_01_1_ye
true_start_write_01_1_ye, ,<,true_start_write_01_1_ye_1
true_start_write_01_1_ye_1, ,0,true_start_write_01_1_ye_2
true_start_write_01_1_ye_2,0,>,true_start_write_01_1_ye_3
true_start_write_01_1_ye_3, ,1,true_start_write_01_1_ye_4
true_start_write_01_1_ye_4,1,>,new_start


# 00 КОМБ
its_02_check_this_tmp, ,>,its_02_check_this
its_02_check_this,2,>,its_02_check_this
its_02_check_this,1,>,its_02_check_this
its_02_check_this,0,>,its_02_check_this
its_02_check_this, ,>,its_02_check_this_1

its_02_check_this_1,8,>,its_02_check_this_1
its_02_check_this_1,7,>,its_02_check_this_1
its_02_check_this_1,6,>,its_02_check_this_1
its_02_check_this_1,5,>,its_02_check_this_1
its_02_check_this_1,4,>,its_02_check_this_1
its_02_check_this_1,3,>,its_02_check_this_1
its_02_check_this_1,2,>,its_02_check_this_1
its_02_check_this_1,1,>,its_02_check_this_1
its_02_check_this_1,0,>,its_02_check_this_1

its_02_check_this_1, ,=,its_02_check_write_5
its_02_check_write_5, ,2,true_start_write_02_1_yes

true_start_write_02_1_yes,8,<,true_start_write_02_1_yes
true_start_write_02_1_yes,7,<,true_start_write_02_1_yes
true_start_write_02_1_yes,6,<,true_start_write_02_1_yes
true_start_write_02_1_yes,5,<,true_start_write_02_1_yes
true_start_write_02_1_yes,4,<,true_start_write_02_1_yes
true_start_write_02_1_yes,3,<,true_start_write_02_1_yes
true_start_write_02_1_yes,2,<,true_start_write_02_1_yes
true_start_write_02_1_yes,1,<,true_start_write_02_1_yes
true_start_write_02_1_yes,0,<,true_start_write_02_1_yes
true_start_write_02_1_yes, ,<,true_start_write_02_1_ye

true_start_write_02_1_ye,2,<,true_start_write_02_1_ye
true_start_write_02_1_ye,1,<,true_start_write_02_1_ye
true_start_write_02_1_ye,0,<,true_start_write_02_1_ye
true_start_write_02_1_ye, ,<,true_start_write_02_1_ye_1
true_start_write_02_1_ye_1, ,0,true_start_write_02_1_ye_2
true_start_write_02_1_ye_2,0,>,true_start_write_02_1_ye_3
true_start_write_02_1_ye_3, ,2,true_start_write_02_1_ye_4
true_start_write_02_1_ye_4,2,>,new_start



# 10 КОМБ
its_10_check_this_tmp, ,>,its_10_check_this
its_10_check_this,2,>,its_10_check_this
its_10_check_this,1,>,its_10_check_this
its_10_check_this,0,>,its_10_check_this
its_10_check_this, ,>,its_10_check_this_1

its_10_check_this_1,8,>,its_10_check_this_1
its_10_check_this_1,7,>,its_10_check_this_1
its_10_check_this_1,6,>,its_10_check_this_1
its_10_check_this_1,5,>,its_10_check_this_1
its_10_check_this_1,4,>,its_10_check_this_1
its_10_check_this_1,3,>,its_10_check_this_1
its_10_check_this_1,2,>,its_10_check_this_1
its_10_check_this_1,1,>,its_10_check_this_1
its_10_check_this_1,0,>,its_10_check_this_1

its_10_check_this_1, ,=,its_10_check_write_5
its_10_check_write_5, ,3,true_start_write_10_1_yes

true_start_write_10_1_yes,8,<,true_start_write_10_1_yes
true_start_write_10_1_yes,7,<,true_start_write_10_1_yes
true_start_write_10_1_yes,6,<,true_start_write_10_1_yes
true_start_write_10_1_yes,5,<,true_start_write_10_1_yes
true_start_write_10_1_yes,4,<,true_start_write_10_1_yes
true_start_write_10_1_yes,3,<,true_start_write_10_1_yes
true_start_write_10_1_yes,2,<,true_start_write_10_1_yes
true_start_write_10_1_yes,1,<,true_start_write_10_1_yes
true_start_write_10_1_yes,0,<,true_start_write_10_1_yes
true_start_write_10_1_yes, ,<,true_start_write_10_1_ye

true_start_write_10_1_ye,2,<,true_start_write_10_1_ye
true_start_write_10_1_ye,1,<,true_start_write_10_1_ye
true_start_write_10_1_ye,0,<,true_start_write_10_1_ye
true_start_write_10_1_ye, ,<,true_start_write_10_1_ye_1
true_start_write_10_1_ye_1, ,1,true_start_write_10_1_ye_2
true_start_write_10_1_ye_2,1,>,true_start_write_10_1_ye_3
true_start_write_10_1_ye_3, ,0,true_start_write_10_1_ye_4
true_start_write_10_1_ye_4,0,>,new_start


# 11 КОМБ
its_11_check_this_tmp, ,>,its_11_check_this
its_11_check_this,2,>,its_11_check_this
its_11_check_this,1,>,its_11_check_this
its_11_check_this,0,>,its_11_check_this
its_11_check_this, ,>,its_11_check_this_1

its_11_check_this_1,8,>,its_11_check_this_1
its_11_check_this_1,7,>,its_11_check_this_1
its_11_check_this_1,6,>,its_11_check_this_1
its_11_check_this_1,5,>,its_11_check_this_1
its_11_check_this_1,4,>,its_11_check_this_1
its_11_check_this_1,3,>,its_11_check_this_1
its_11_check_this_1,2,>,its_11_check_this_1
its_11_check_this_1,1,>,its_11_check_this_1
its_11_check_this_1,0,>,its_11_check_this_1

its_11_check_this_1, ,=,its_11_check_write_5
its_11_check_write_5, ,4,true_start_write_11_1_yes

true_start_write_11_1_yes,8,<,true_start_write_11_1_yes
true_start_write_11_1_yes,7,<,true_start_write_11_1_yes
true_start_write_11_1_yes,6,<,true_start_write_11_1_yes
true_start_write_11_1_yes,5,<,true_start_write_11_1_yes
true_start_write_11_1_yes,4,<,true_start_write_11_1_yes
true_start_write_11_1_yes,3,<,true_start_write_11_1_yes
true_start_write_11_1_yes,2,<,true_start_write_11_1_yes
true_start_write_11_1_yes,1,<,true_start_write_11_1_yes
true_start_write_11_1_yes,0,<,true_start_write_11_1_yes
true_start_write_11_1_yes, ,<,true_start_write_11_1_ye

true_start_write_11_1_ye,2,<,true_start_write_11_1_ye
true_start_write_11_1_ye,1,<,true_start_write_11_1_ye
true_start_write_11_1_ye,0,<,true_start_write_11_1_ye
true_start_write_11_1_ye, ,<,true_start_write_11_1_ye_1
true_start_write_11_1_ye_1, ,1,true_start_write_11_1_ye_2
true_start_write_11_1_ye_2,1,>,true_start_write_11_1_ye_3
true_start_write_11_1_ye_3, ,1,true_start_write_11_1_ye_4
true_start_write_11_1_ye_4,1,>,new_start



# 12 КОМБ
its_12_check_this_tmp, ,>,its_12_check_this
its_12_check_this,2,>,its_12_check_this
its_12_check_this,1,>,its_12_check_this
its_12_check_this,0,>,its_12_check_this
its_12_check_this, ,>,its_12_check_this_1

its_12_check_this_1,8,>,its_12_check_this_1
its_12_check_this_1,7,>,its_12_check_this_1
its_12_check_this_1,6,>,its_12_check_this_1
its_12_check_this_1,5,>,its_12_check_this_1
its_12_check_this_1,4,>,its_12_check_this_1
its_12_check_this_1,3,>,its_12_check_this_1
its_12_check_this_1,2,>,its_12_check_this_1
its_12_check_this_1,1,>,its_12_check_this_1
its_12_check_this_1,0,>,its_12_check_this_1

its_12_check_this_1, ,=,its_12_check_write_5
its_12_check_write_5, ,5,true_start_write_12_1_yes

true_start_write_12_1_yes,8,<,true_start_write_12_1_yes
true_start_write_12_1_yes,7,<,true_start_write_12_1_yes
true_start_write_12_1_yes,6,<,true_start_write_12_1_yes
true_start_write_12_1_yes,5,<,true_start_write_12_1_yes
true_start_write_12_1_yes,4,<,true_start_write_12_1_yes
true_start_write_12_1_yes,3,<,true_start_write_12_1_yes
true_start_write_12_1_yes,2,<,true_start_write_12_1_yes
true_start_write_12_1_yes,1,<,true_start_write_12_1_yes
true_start_write_12_1_yes,0,<,true_start_write_12_1_yes
true_start_write_12_1_yes, ,<,true_start_write_12_1_ye

true_start_write_12_1_ye,2,<,true_start_write_12_1_ye
true_start_write_12_1_ye,1,<,true_start_write_12_1_ye
true_start_write_12_1_ye,0,<,true_start_write_12_1_ye
true_start_write_12_1_ye, ,<,true_start_write_12_1_ye_1
true_start_write_12_1_ye_1, ,1,true_start_write_12_1_ye_2
true_start_write_12_1_ye_2,1,>,true_start_write_12_1_ye_3
true_start_write_12_1_ye_3, ,2,true_start_write_12_1_ye_4
true_start_write_12_1_ye_4,2,>,new_start


# 20 КОМБ
its_20_check_this_tmp, ,>,its_20_check_this
its_20_check_this,2,>,its_20_check_this
its_20_check_this,1,>,its_20_check_this
its_20_check_this,0,>,its_20_check_this
its_20_check_this, ,>,its_20_check_this_1

its_20_check_this_1,8,>,its_20_check_this_1
its_20_check_this_1,7,>,its_20_check_this_1
its_20_check_this_1,6,>,its_20_check_this_1
its_20_check_this_1,5,>,its_20_check_this_1
its_20_check_this_1,4,>,its_20_check_this_1
its_20_check_this_1,3,>,its_20_check_this_1
its_20_check_this_1,2,>,its_20_check_this_1
its_20_check_this_1,1,>,its_20_check_this_1
its_20_check_this_1,0,>,its_20_check_this_1

its_20_check_this_1, ,=,its_20_check_write_5
its_20_check_write_5, ,6,true_start_write_20_1_yes

true_start_write_20_1_yes,8,<,true_start_write_20_1_yes
true_start_write_20_1_yes,7,<,true_start_write_20_1_yes
true_start_write_20_1_yes,6,<,true_start_write_20_1_yes
true_start_write_20_1_yes,5,<,true_start_write_20_1_yes
true_start_write_20_1_yes,4,<,true_start_write_20_1_yes
true_start_write_20_1_yes,3,<,true_start_write_20_1_yes
true_start_write_20_1_yes,2,<,true_start_write_20_1_yes
true_start_write_20_1_yes,1,<,true_start_write_20_1_yes
true_start_write_20_1_yes,0,<,true_start_write_20_1_yes
true_start_write_20_1_yes, ,<,true_start_write_20_1_ye

true_start_write_20_1_ye,2,<,true_start_write_20_1_ye
true_start_write_20_1_ye,1,<,true_start_write_20_1_ye
true_start_write_20_1_ye,0,<,true_start_write_20_1_ye
true_start_write_20_1_ye, ,<,true_start_write_20_1_ye_1
true_start_write_20_1_ye_1, ,2,true_start_write_20_1_ye_2
true_start_write_20_1_ye_2,2,>,true_start_write_20_1_ye_3
true_start_write_20_1_ye_3, ,0,true_start_write_20_1_ye_4
true_start_write_20_1_ye_4,0,>,new_start



# 21 КОМБ
its_21_check_this_tmp, ,>,its_21_check_this
its_21_check_this,2,>,its_21_check_this
its_21_check_this,1,>,its_21_check_this
its_21_check_this,0,>,its_21_check_this
its_21_check_this, ,>,its_21_check_this_1

its_21_check_this_1,8,>,its_21_check_this_1
its_21_check_this_1,7,>,its_21_check_this_1
its_21_check_this_1,6,>,its_21_check_this_1
its_21_check_this_1,5,>,its_21_check_this_1
its_21_check_this_1,4,>,its_21_check_this_1
its_21_check_this_1,3,>,its_21_check_this_1
its_21_check_this_1,2,>,its_21_check_this_1
its_21_check_this_1,1,>,its_21_check_this_1
its_21_check_this_1,0,>,its_21_check_this_1

its_21_check_this_1, ,=,its_21_check_write_5
its_21_check_write_5, ,7,true_start_write_21_1_yes

true_start_write_21_1_yes,8,<,true_start_write_21_1_yes
true_start_write_21_1_yes,7,<,true_start_write_21_1_yes
true_start_write_21_1_yes,6,<,true_start_write_21_1_yes
true_start_write_21_1_yes,5,<,true_start_write_21_1_yes
true_start_write_21_1_yes,4,<,true_start_write_21_1_yes
true_start_write_21_1_yes,3,<,true_start_write_21_1_yes
true_start_write_21_1_yes,2,<,true_start_write_21_1_yes
true_start_write_21_1_yes,1,<,true_start_write_21_1_yes
true_start_write_21_1_yes,0,<,true_start_write_21_1_yes
true_start_write_21_1_yes, ,<,true_start_write_21_1_ye

true_start_write_21_1_ye,2,<,true_start_write_21_1_ye
true_start_write_21_1_ye,1,<,true_start_write_21_1_ye
true_start_write_21_1_ye,0,<,true_start_write_21_1_ye
true_start_write_21_1_ye, ,<,true_start_write_21_1_ye_1
true_start_write_21_1_ye_1, ,2,true_start_write_21_1_ye_2
true_start_write_21_1_ye_2,2,>,true_start_write_21_1_ye_3
true_start_write_21_1_ye_3, ,1,true_start_write_21_1_ye_4
true_start_write_21_1_ye_4,1,>,new_start


#22 КОМБ
its_22_check_this_tmp, ,>,its_22_check_this
its_22_check_this,2,>,its_22_check_this
its_22_check_this,1,>,its_22_check_this
its_22_check_this,0,>,its_22_check_this
its_22_check_this, ,>,its_22_check_this_1

its_22_check_this_1,8,>,its_22_check_this_1
its_22_check_this_1,7,>,its_22_check_this_1
its_22_check_this_1,6,>,its_22_check_this_1
its_22_check_this_1,5,>,its_22_check_this_1
its_22_check_this_1,4,>,its_22_check_this_1
its_22_check_this_1,3,>,its_22_check_this_1
its_22_check_this_1,2,>,its_22_check_this_1
its_22_check_this_1,1,>,its_22_check_this_1
its_22_check_this_1,0,>,its_22_check_this_1

its_22_check_this_1, ,=,its_22_check_write_5
its_22_check_write_5, ,8,true_start_write_22_1_yes

true_start_write_22_1_yes,8,<,true_start_write_22_1_yes
true_start_write_22_1_yes,7,<,true_start_write_22_1_yes
true_start_write_22_1_yes,6,<,true_start_write_22_1_yes
true_start_write_22_1_yes,5,<,true_start_write_22_1_yes
true_start_write_22_1_yes,4,<,true_start_write_22_1_yes
true_start_write_22_1_yes,3,<,true_start_write_22_1_yes
true_start_write_22_1_yes,2,<,true_start_write_22_1_yes
true_start_write_22_1_yes,1,<,true_start_write_22_1_yes
true_start_write_22_1_yes,0,<,true_start_write_22_1_yes
true_start_write_22_1_yes, ,<,true_start_write_22_1_ye

true_start_write_22_1_ye,2,<,true_start_write_22_1_ye
true_start_write_22_1_ye,1,<,true_start_write_22_1_ye
true_start_write_22_1_ye,0,<,true_start_write_22_1_ye
true_start_write_22_1_ye, ,<,true_start_write_22_1_ye_1
true_start_write_22_1_ye_1, ,2,true_start_write_22_1_ye_2
true_start_write_22_1_ye_2,2,>,true_start_write_22_1_ye_3
true_start_write_22_1_ye_3, ,2,true_start_write_22_1_ye_4
true_start_write_22_1_ye_4,2,>,new_start

   ```
9. **Замечания автора** по существу работы: Все было ровно, за исключением того, что мнепришлось придумывать новый алгоритм(
10. **Выводы**: Мы научились работать с машиной Тьюринга в четвёрках. Научились создавать на ней свои алгоритмы. Прокачали свой мозг. Благодаря своей лабороторной работе, я могу переводить из 3 в 9 систему счисления гораздо быстрее. А еще мы осознали насколько быстро работают машины тьюринга! ```Thats ALL```
