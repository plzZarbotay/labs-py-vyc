arts@LemonCorp:~$ echo Я эти команды пишу уже 5 раз, потому что случайно закрываю консоль, ааааааааа
Я эти команды пишу уже 5 раз, потому что случайно закрываю консоль, ааааааааа
arts@LemonCorp:~$ who
arts     tty2         2023-10-02 02:28 (tty2)
arts@LemonCorp:~$ pwd
/home/arts
arts@LemonCorp:~$ ls
 ld   lol.txt   ol.txt   snap   Видео   Документы   Загрузки   Изображения   Музыка   Общедоступные  'Рабочий стол'   Шаблоны
arts@LemonCorp:~$ cd Документы/
arts@LemonCorp:~/Документы$ ды
ды: команда не найдена
arts@LemonCorp:~/Документы$ ls
f1.txt  f1.txt~  herniya  labspython  LemOS
arts@LemonCorp:~/Документы$ cd labspython/
arts@LemonCorp:~/Документы/labspython$ ls
history.txt  id_rsa  id_rsa.pub  labs-py-vyc  Oil
arts@LemonCorp:~/Документы/labspython$ mkdir delete
arts@LemonCorp:~/Документы/labspython$ rmdir delete
arts@LemonCorp:~/Документы/labspython$ ls
history.txt  id_rsa  id_rsa.pub  labs-py-vyc  Oil
arts@LemonCorp:~/Документы/labspython$ mkdir delete
arts@LemonCorp:~/Документы/labspython$ ls
delete  history.txt  id_rsa  id_rsa.pub  labs-py-vyc  Oil
arts@LemonCorp:~/Документы/labspython$ mkdir delete
mkdir: невозможно создать каталог «delete»: Файл существует
arts@LemonCorp:~/Документы/labspython$ rmdir delete
arts@LemonCorp:~/Документы/labspython$ ls
history.txt  id_rsa  id_rsa.pub  labs-py-vyc  Oil
arts@LemonCorp:~/Документы/labspython$ mkdir aa
arts@LemonCorp:~/Документы/labspython$ cd aa
arts@LemonCorp:~/Документы/labspython/aa$ ls
arts@LemonCorp:~/Документы/labspython/aa$ cat > da.txt
aaaaaa, не хочу, поставь 5 плиз
arts@LemonCorp:~/Документы/labspython/aa$ сфе
сфе: команда не найдена
arts@LemonCorp:~/Документы/labspython/aa$ cat da.txt
aaaaaa, не хочу, поставь 5 плиз
arts@LemonCorp:~/Документы/labspython/aa$ tail da.txt 1
==> da.txt <==
aaaaaa, не хочу, поставь 5 плиз
tail: невозможно открыть '1' для чтения: Нет такого файла или каталога
arts@LemonCorp:~/Документы/labspython/aa$ tail 1 da.txt
tail: невозможно открыть '1' для чтения: Нет такого файла или каталога
==> da.txt <==
aaaaaa, не хочу, поставь 5 плиз
arts@LemonCorp:~/Документы/labspython/aa$ tail-n 1 da.txt
tail-n: команда не найдена
arts@LemonCorp:~/Документы/labspython/aa$ tail -n 1 da.txt
aaaaaa, не хочу, поставь 5 плиз
arts@LemonCorp:~/Документы/labspython/aa$ head -n 1 da.txt
aaaaaa, не хочу, поставь 5 плиз
arts@LemonCorp:~/Документы/labspython/aa$ grep 5  da.txt
aaaaaa, не хочу, поставь 5 плиз
arts@LemonCorp:~/Документы/labspython/aa$ history 
  179  history > history.txt
  180  ls
  181  cat history.txt
  182  cd Документы
  183  ды
  184  ls
  185  cd labspython/
  186  ls
  187  history 
  188  who
  189  pwd
  190  ls
  191  cd Документы/
  192  ls
  193  cd labspython/
  194  ls
  195  cat > lol.txt
  196  cat > ol.txt
  197  cp lol.txt ol.txt
  198  cat ol.txt
  199  ls
  200  mkdir Oil
  201  mv ol.txt Oil/ol.txt
  202  ls
  203  cd Oil/
  204  ls
  214  cd ../
  215  ls
  216  rm lol.txt
  217  ps
  218  ps -A
  219  cd Oil/
  220  ls
  221  tail ol.txt
  222  head ol.txt
  223  grep sadl ol.txt
  224  history
  225  cd ../
  226  cd ./
  227  cd -
  228  cd /
  229  ls
  230  cd ../
  231  cd ./
  232  cd ~/
  233  cd Документы/
  234  cd labspython/
  235  LS
  236  ls
  237  mkdir none
  238  ls
  239  rmdir none
  240  sudo
  241  man sudo
  242  sudo -h
  243  echo Lol
  244  echo Зачем это делать?
  245  echo Виктор, поставь 5
  246  ssh a_ganyak@185.5.249.140
  247  history
  248  who
  249  clear
  250  echo Я эти команды пишу уже 5 раз, потому что случайно закрываю консоль, ааааааааа
  251  who
  252  pws
  253  pwd
  254  ls
  255  cd Документы/
  256  ды
  257  ls
  258  cd labspython/
  259  ls
  260  mkdir delete
  261  rmdir delete
  262  ls
  263  mkdir delete
  264  ls
  265  mkdir delete
  266  rmdir delete
  267  ls
  268  mkdir aa
  269  cd aa
  270  ls
  271  cat > da.txt
  272  сфе
  273  cat da.txt
  274  tail da.txt 1
  275  tail 1 da.txt
  276  tail-n 1 da.txt
  277  tail -n 1 da.txt
  278  head -n 1 da.txt
  279  grep 5  da.txt
  280  history 
arts@LemonCorp:~/Документы/labspython/aa$ ps
    PID TTY          TIME CMD
   7745 pts/0    00:00:00 bash
   9254 pts/0    00:00:00 ps
arts@LemonCorp:~/Документы/labspython/aa$ sudo -f
sudo: неверный ключ — «f»
usage: sudo -h | -K | -k | -V
usage: sudo -v [-ABknS] [-g group] [-h host] [-p prompt] [-u user]
usage: sudo -l [-ABknS] [-g group] [-h host] [-p prompt] [-U user] [-u user] [command]
usage: sudo [-ABbEHknPS] [-r role] [-t type] [-C num] [-D directory] [-g group] [-h host] [-p prompt] [-R directory] [-T timeout] [-u user] [VAR=value] [-i|-s] [<command>]
usage: sudo -e [-ABknS] [-r role] [-t type] [-C num] [-D directory] [-g group] [-h host] [-p prompt] [-R directory] [-T timeout] [-u user] file ...
arts@LemonCorp:~/Документы/labspython/aa$ sudo -h
sudo — выполнение команд от имени другого пользователя

usage: sudo -h | -K | -k | -V
usage: sudo -v [-ABknS] [-g group] [-h host] [-p prompt] [-u user]
usage: sudo -l [-ABknS] [-g group] [-h host] [-p prompt] [-U user] [-u user] [command]
usage: sudo [-ABbEHknPS] [-r role] [-t type] [-C num] [-D directory] [-g group] [-h host] [-p prompt] [-R directory] [-T timeout] [-u user] [VAR=value] [-i|-s] [<command>]
usage: sudo -e [-ABknS] [-r role] [-t type] [-C num] [-D directory] [-g group] [-h host] [-p prompt] [-R directory] [-T timeout] [-u user] file ...

Параметры:
  -A, --askpass                 использовать вспомогательную программу для ввода пароля
  -b, --background              выполнить команду в фоновом режиме
  -B, --bell                    ring bell when prompting
  -C, --close-from=num          закрыть все дескрипторы файлов >= num
  -D, --chdir=directory         change the working directory before running command
  -E, --preserve-env            сохранить пользовательское окружение при выполнении команды
      --preserve-env=list       preserve specific environment variables
  -e, --edit                    редактировать файлы вместо выполнения команды
  -g, --group=group             выполнить команду от имени или ID указанной группы
  -H, --set-home                установить для переменной HOME домашний каталог указанного пользователя
  -h, --help                    показать справку и выйти
  -h, --host=host               выполнить команду на узле (если поддерживается модулем)
  -i, --login                   запустить оболочку входа в систему от имени указанного пользователя; также можно задать
                                команду
  -K, --remove-timestamp        полностью удалить файл timestamp
  -k, --reset-timestamp         объявить недействительным файл timestamp
  -l, --list                    показать список прав пользователя или проверить заданную команду; в длинном формате
                                используется дважды
  -n, --non-interactive         автономный режим без не вывода запросов пользователю
  -P, --preserve-groups         сохранить вектор группы вместо установки целевой группы
  -p, --prompt=prompt           использовать указанный запрос пароля
  -R, --chroot=directory        change the root directory before running command
  -r, --role=role               создать контекст безопасности SELinux с указанной ролью
  -S, --stdin                   читать пароль из стандартного ввода
  -s, --shell                   запустить оболочку от имени указанного пользователя; также можно задать команду
  -t, --type=type               создать контекст безопасности SELinux указанного типа
  -T, --command-timeout=timeout terminate command after the specified time limit
  -U, --other-user=user         в режиме списка показывать права пользователя
  -u, --user=user               выполнить команду (или редактировать файл) от имени или ID указанного пользователя
  -V, --version                 показать сведения о версии и выйти
  -v, --validate                обновить временную метку пользователя без выполнения команды
  --                            прекратить обработку аргументов командной строки
arts@LemonCorp:~/Документы/labspython/aa$ sudo apt install
[sudo] пароль для arts: 
Чтение списков пакетов… Готово
Построение дерева зависимостей… Готово
Чтение информации о состоянии… Готово         
Обновлено 0 пакетов, установлено 0 новых пакетов, для удаления отмечено 0 пакетов, и 212 пакетов не обновлено.
arts@LemonCorp:~/Документы/labspython/aa$ cd ../
arts@LemonCorp:~/Документы/labspython$ ls
aa  history.txt  id_rsa  id_rsa.pub  labs-py-vyc  Oil
arts@LemonCorp:~/Документы/labspython$ cd Oil
arts@LemonCorp:~/Документы/labspython/Oil$ ls
ol.txt
arts@LemonCorp:~/Документы/labspython/Oil$ scp ol.txt a_ganyak@185.5.249.140
arts@LemonCorp:~/Документы/labspython/Oil$ ssh  a_ganyak@185.5.249.140
Welcome to Ubuntu 20.04.6 LTS (GNU/Linux 5.4.0-162-generic x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage
New release '22.04.3 LTS' available.
Run 'do-release-upgrade' to upgrade to it.

Last login: Mon Oct  2 00:02:51 2023 from 87.249.25.133
a_ganyak@vds2476450:~$ ls
dont_see  my_arch.tar  random.txt
a_ganyak@vds2476450:~$ logout
Connection to 185.5.249.140 closed.
arts@LemonCorp:~/Документы/labspython/Oil$ scp 
::1:                     fe00::0:                 ff02::1:                 ip6-allnodes:            ip6-localhost:           ip6-loopback:            LemonCorp:               ol.txt 
a_ganyak@185.5.249.140   ff00::0:                 ff02::2:                 ip6-allrouters:          ip6-localnet:            ip6-mcastprefix:         localhost:               
arts@LemonCorp:~/Документы/labspython/Oil$ scp 
::1:                     fe00::0:                 ff02::1:                 ip6-allnodes:            ip6-localhost:           ip6-loopback:            LemonCorp:               ol.txt 
a_ganyak@185.5.249.140   ff00::0:                 ff02::2:                 ip6-allrouters:          ip6-localnet:            ip6-mcastprefix:         localhost:               
arts@LemonCorp:~/Документы/labspython/Oil$ ls
a_ganyak@185.5.249.140  ol.txt
arts@LemonCorp:~/Документы/labspython/Oil$ scp ol.txt a_ganyak@185.5.249.140:/Oil
scp: dest open "/Oil": Permission denied
scp: failed to upload file ol.txt to /Oil
arts@LemonCorp:~/Документы/labspython/Oil$ scp ol.txt a_ganyak@185.5.249.140:/
scp: dest open "/ol.txt": Permission denied
scp: failed to upload file ol.txt to /
arts@LemonCorp:~/Документы/labspython/Oil$ cd ../
arts@LemonCorp:~/Документы/labspython$ ls 
aa  history.txt  id_rsa  id_rsa.pub  labs-py-vyc  Oil
arts@LemonCorp:~/Документы/labspython$ cd labs-py-vyc/
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ ls
1  README.md  scr.sh
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ cat ol.txt
cat: ol.txt: Нет такого файла или каталога
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ cat > ol.txt
asda
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ scp ol.txt a_ganyak@185.5.249.140:/
scp: dest open "/ol.txt": Permission denied
scp: failed to upload file ol.txt to /
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ ls
1  ol.txt  README.md  scr.sh
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ scp ol.txt a_ganyak@185.5.249.140:/home/a_ganyak/
ol.txt                                                                                                                                                                    100%    5     1.3KB/s   00:00    
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ ssh  a_ganyak@185.5.249.140
Welcome to Ubuntu 20.04.6 LTS (GNU/Linux 5.4.0-162-generic x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage
New release '22.04.3 LTS' available.
Run 'do-release-upgrade' to upgrade to it.

Last login: Mon Oct  2 00:21:02 2023 from 87.249.25.133
a_ganyak@vds2476450:~$ ls
dont_see  my_arch.tar  ol.txt  random.txt
a_ganyak@vds2476450:~$ logout
Connection to 185.5.249.140 closed.
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ ssh-keygen
Generating public/private rsa key pair.
Enter file in which to save the key (/home/arts/.ssh/id_rsa): id_rsa
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in id_rsa
Your public key has been saved in id_rsa.pub
The key fingerprint is:
SHA256:XMT+FNGo0oVDUwymcNUGUB2YM4u3+ouV3E4YnAOxU6A arts@LemonCorp
The key's randomart image is:
+---[RSA 3072]----+
|      . =B@@+=   |
|       + BO.O .  |
|      E =+.O .   |
|       .o=*..    |
|        So=+     |
|         ..*.    |
|         .= o    |
|        .o o     |
|        ..o..    |
+----[SHA256]-----+
arts@LemonCorp:~/Документы/labspython/labs-py-vyc$ ssh-copy-id -i ~/.ssh/id_rsa.pub a_ganyak@185.5.249.140 -p cALFKPT97SSMG
