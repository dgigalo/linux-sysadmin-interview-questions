Вопросы, которые задают на собеседовании администраторам Linux и инженерам DevOps
====================================================

Вопросы собраны из разных источников интернета. Добавляйте свои


## <a name='toc'>Table of Contents</a>

  1. [Общие вопросы](#general)
  1. [Простые вопросы](#simple)
  1. [Вопросы среднего уровня](#medium)
  1. [Hard Linux Questions](#hard)
  1. [Expert Linux Questions](#expert)
  1. [Networking Questions](#network)
  1. [MySQL Questions](#mysql)
  1. [DevOps Questions](#devop)
  1. [Веселые вопросы](#fun)
  1. [Веб вопросы](#web)
  1. [Практикум](#demo)
  1. [Команды](#commands)
  1. [Other Great References](#references)


#### [[⬆]](#toc) <a name='general'>Общие вопросы:</a>

* Что вы изучали в последнее время?
* Расскажите какие инструменты разработки/администрирования вы используете(OS, Editor, Browsers, Tools etc.)
* Расскажите о последнем linux-проекте, на котором вы работали.
* Расскажите какую вы совершили ошибку недавно(давно) и какой вывод вы сделали?
* Почему мы должны вас выбрать?
* What is an A record, an NS record, a PTR record, a CNAME record, an MX record?
* What is SMTP? Give the basic scenario of how a mail message is delivered via SMTP.
* What is RAID? What is RAID0, RAID1, RAID5, RAID10?
* What is a level 0 backup? What is an incremental backup?
* Describe the general file system hierarchy of a Linux system.
* Which difference have between public and private SSH key?
* Что такое Split-Horizon DNS?

#### [[⬆]](#toc) <a name='simple'>Простые вопросы:</a>

* Как называется главный пользователь Linux системы и назовите его UID?
* Как посмотреть все файлы, включая скрытые в директории?
* Какой командой можно удалить папку вместе со всем содержимым?
* Какой командой можно посмотреть утилизацию памяти в Linux'e?
* Какой командой осуществить поиск строки "my string" внутри директории рекурсивно?
* Как подключится к удаленному серверу через SSH?
* Как посмотреть переменные среды и как их использовать?
* Когда запускаете ```ifconfig -a``` получаете ошибку "command not found". С чем это может быть связано?
* Что произойдет если нажать TAB-TAB?
* Какой командой можно посмотреть все доступное место на диске Unix/Linux системы?
* Какими командами можно проверить записи DNS?
* Какой командой можно изменить владельца файла? Установить разрешения на файл?
* Что выполнит данная команда ```chmod +x FILENAME```?
* Что означают разрешение 0750 для файла? Отличается от разрешений для директории?
* Как добавить нового юзера без разрешения на логин(login permissions)?
* Как добавить/удалить пользователя из группы?
* Что выполнит данная команда CTRL-c?
* Что находится в файле /etc/services?
* Как перенаправить стандартный вывод STDOUT и стандартный вывод ошибок STDERR? (> /dev/null 2>&1)
* Какая разница между подключением по Telnet и SSH?
* Какими командами можно посмотреть среднюю загрузку системы? Объясните 3 основных значения загрузки системы(load average)?
* Назовите опции в нижнем регистре для команды ```ls```, которые не являются рабочими.
* Что такое модуль ядра Linux'a?
* Что такое протокол ICMP? Для чего используется?
* Что такое уровень запуска и как посмотреть текущий?
* Как проверить является ли машина виртуальной?
* Как принудительно заставить систему выполнить проверку файловой системы при следующем запуске?
<br>
<a href="https://aix-adm.blogspot.com/2019/10/linux.html"> Вопросы с ответами </a>


#### [[⬆]](#toc) <a name='medium'>Вопросы среднего уровня:</a>

* Что обозначает ```&``` после команды?
* Что обозначает ```& disown``` после команды?
* Что такое фильтр пакетов (packet filter) и как он работает?
* Что такое виртуальная память(Virtual Memory)?
* Что такое swap и для чего используется?
* Какие записи ДНС вы знаете, для чего они используются?
* Что такое "sticky bit"?
* Для чего предназначен бит неизменяемости(immutable bit)?
* Что такое жесткая ссылка, символическая? Чем отличаются? Что произойдет если удалить источник, на который указывает ссылка?
* Что такое айнод(inode) и какие поля в нем хранятся?
* Что такое SNMP и для чего он используется?
* Как уменьшить размер файла, который используется в текущий момент(например, файла лога)?
* Что такое переадресация SSH-порта?
* What is the difference between local and remote port forwarding?
* What are the steps to add a user to a system without using useradd/adduser?
* What is MAJOR and MINOR numbers of special files?
* Describe the mknod command and when you'd use it.
* Describe a scenario when you get a "filesystem is full" error, but 'df' shows there is free space.
* Describe a scenario when deleting a file, but 'df' not showing the space being freed.
* Describe how 'ps' works.
* What happens to a child process that dies and has no parent process to wait for it and what’s bad about this?
* Explain briefly each one of the process states.
* How to know which process listens on a specific port?
* What is a zombie process and what could be the cause of it?
* You run a bash script and you want to see its output on your terminal and save it to a file at the same time. How could you do it?
* Explain what echo "1" > /proc/sys/net/ipv4/ip_forward does.
* Can you have several HTTPS virtual hosts sharing the same IP?
* What is a wildcard certificate?
* Which Linux file types do you know?
* What is the difference between a process and a thread? And parent and child processes after a fork system call?
* What is the difference between exec and fork?
* What is "nohup" used for?
* What is the difference between these two commands?
 * ```myvar=hello```
 * ```export myvar=hello```
* How many NTP servers would you configure in your local ntp.conf?
* What does the column 'reach' mean in ```ntpq -p``` output?
* You need to upgrade kernel at 100-1000 servers, how you would do this?
* How can you get Host, Channel, ID, LUN of SCSI disk?
* How can you limit process memory usage?
* What is bash quick substitution/caret replace(^x^y)?
* Do you know of any alternative shells? If so, have you used any?
* What is a tarpipe (or, how would you go about copying everything, including hardlinks and special files, from one server to another)?
* How can you tell if the httpd package was already installed?
* How can you list the contents of a package?
* How can you determine which package is better: openssh-server-5.3p1-118.1.el6_8.x86_64 or openssh-server-6.6p1-1.el6.x86_64 ?
* Can you explain to me the difference between block based, and object based storage?

<a href="https://dev-engineer.blogspot.com/2019/10/linux_9.html"> Вопросы с ответами </a>

#### [[⬆]](#toc) <a name='hard'>Hard Linux Questions:</a>

* Как сбросить кэш оперативной памяти?
* What is a tunnel and how you can bypass a http proxy?
* What is the difference between IDS and IPS?
* What shortcuts do you use on a regular basis?
* What is the Linux Standard Base?
* What is an atomic operation?
* Your freshly configured http server is not running after a restart, what can you do?
* What kind of keys are in ~/.ssh/authorized_keys and what it is this file used for?
* I've added my public ssh key into authorized_keys but I'm still getting a password prompt, what can be wrong?
* Did you ever create RPM's, DEB's or solaris pkg's?
* What does ```:(){ :|:& };:``` do on your system?
* How do you catch a Linux signal on a script?
* Can you catch a SIGKILL?
* What's happening when the Linux kernel is starting the OOM killer and how does it choose which process to kill first?
* Describe the linux boot process with as much detail as possible, starting from when the system is powered on and ending when you get a prompt.
* What's a chroot jail?
* When trying to umount a directory it says it's busy, how to find out which PID holds the directory?
* What's LD_PRELOAD and when it's used?
* You ran a binary and nothing happened. How would you debug this?
* What are cgroups? Can you specify a scenario where you could use them?
* How can you remove/delete a file with file-name consisting of only non-printable/non-type-able characters?
* How can you increase or decrease the priority of a process in Linux?

<a href="https://dev-engineer.blogspot.com/2019/11/linux_17.html"> Вопросы с ответами </a>

#### [[⬆]](#toc) <a name='expert'>Expert Linux Questions:</a>

* A running process gets ```EAGAIN: Resource temporarily unavailable``` on reading a socket. How can you close this bad socket/file descriptor without killing the process?
* What do you control with swapiness?
* How do you change TCP stack buffers? How do you calculate it?
* What is Huge Tables? Why isn't it enabled by default? Why and when use it?
* What is LUKS? How to use it?


#### [[⬆]](#toc) <a name='network'>Networking Questions:</a>

* What is localhost and why would ```ping localhost``` fail?
* What is the similarity between "ping" & "traceroute" ? How is traceroute able to find the hops.
* What is the command used to show all open ports and/or socket connections on a machine?
* Is 300.168.0.123 a valid IPv4 address?
* Which IP ranges/subnets are "private" or "non-routable" (RFC 1918)?
* What is a VLAN?
* What is ARP and what is it used for?
* What is the difference between TCP and UDP?
* What is the purpose of a default gateway?
* What is command used to show the routing table on a Linux box?
* A TCP connection on a network can be uniquely defined by 4 things. What are those things?
* When a client running a web browser connects to a web server, what is the source port and what is the destination port of the connection?
* How do you add an IPv6 address to a specific interface?
* You have added an IPv4 and IPv6 address to interface eth0. A ping to the v4 address is working but a ping to the v6 address gives you the response ```sendmsg: operation not permitted```. What could be wrong?
* What is SNAT and when should it be used?
* Explain how could you ssh login into a Linux system that DROPs all new incoming packets using a SSH tunnel.
* How do you stop a DDoS attack?
* How can you see content of an ip packet?
* What is IPoAC (RFC 1149)?
* What will happen when you bind port 0?


#### [[⬆]](#toc) <a name='mysql'>MySQL questions:</a>

* How do you create a user?
* How do you provide privileges to a user?
* What is the difference between a "left" and a "right" join?
* Explain briefly the differences between InnoDB and MyISAM.
* Describe briefly the steps you need to follow in order to create a simple master/slave cluster.
* Why should you run "mysql_secure_installation" after installing MySQL?
* How do you check which jobs are running?
* How would you take a backup of a MySQL database?

#### [[⬆]](#toc) <a name='devop'>DevOps Questions:</a>

* Can you describe your workflow when you create a script?
* What is GIT?
* What is a dynamically/statically linked file?
* What does "./configure && make && make install" do?
* What is puppet/chef/ansible used for?
* What is Nagios/Zenoss/NewRelic used for?
* What is Jenkins/TeamCity/GoCI used for?
* What is the difference between Containers and VMs?
* How do you create a new postgres user?
* What is a virtual IP address? What is a cluster?
* How do you print all strings of printable characters present in a file?
* How do you find shared library dependencies?
* What is Automake and Autoconf?
* ./configure shows an error that libfoobar is missing on your system, how could you fix this, what could be wrong?
* What are the advantages/disadvantages of script vs compiled program?
* What's the relationship between continuous delivery and DevOps?
* What are the important aspects of a system of continuous integration and deployment?
* How would you enable network file sharing within AWS that would allow EC2 instances in multiple availability zones to share data?

#### [[⬆]](#toc) <a name='fun'>Веселые вопросы:</a>

* Админ случайно выполнил команду: ```chmod 444 /bin/chmod ```. Как починить?
* Вы забыли(потеряли) пароль рута, что делать? 
* Вы перезапустили удаленно сервер, но через 10 минут вы по-прежнему не можете к нему подключиться по SSH. В чем может быть проблема?
* Вы застряли на необитаемом острове, какие 5 утилит командной строки вы бы выбрали?
* Вы случайно удалали файл с запущенным скриптом, возможно ли его можно восстановить? 
* Что приозойдет 19 Января 2038?
* Как перегрузить сервер, если команда reboot  не отвечает?
* Чем отличается rest от json'a? <br />

<a href="https://dev-engineer.blogspot.com/2019/10/linux_8.html"> Вопросы с ответами </a>

#### [[⬆]](#toc) <a name='web'>Веб вопросы:</a>
* Какую функцию выполняет DNS в сети?
* Что такое HTTP?
* Что такое HTTP-proxy и как он работает?
* Кратко опишите как работает HTTPS.
* Что означает директива upstream в настройках nginx'a?
* Кратко опишите действия по созданию и установке ssl-сертифката для сайта https://foo.example.com

<a href="https://dev-engineer.blogspot.com/2019/11/linux.html"> Вопросы с ответами </a>

#### [[⬆]](#toc) <a name='demo'>Практикум</a>

* В директории 500 файлов, необходимо найти все файлы свыше 20 ГБ, отсортировать по размеру, отобразить 5 самых больших файлов.
* Как разделить файл на несколько частей без архиватора? Например, 10 гб файл разделить по 1 гб.
* Unpack test.tar.gz without man pages or google.
* Remove all "*.pyc" files from testdir recursively?
* Search for "my konfu is the best" in all *.py files.
* Replace the occurrence of "my konfu is the best" with "I'm a linux jedi master" in all *.txt files.
* Test if port 443 on a machine with IP address X.X.X.X is reachable.
* Get http://myinternal.webserver.local/test.html via telnet.
* How to send an email without a mail client, just on the command line?
* Write a ```get_prim``` method in python/perl/bash/pseudo.
* Find all files which have been accessed within the last 30 days.
* Explain the following command ```(date ; ps -ef | awk '{print $1}' | sort | uniq | wc -l ) >> Activity.log```
* Write a script to list all the differences between two directories.
* In a log file with contents as ```<TIME> : [MESSAGE] : [ERROR_NO] - Human readable text``` display summary/count of specific error numbers that occurred every hour or a specific hour.


#### [[⬆]](#toc) <a name='commands'>Команды:</a>
* Что выполняют следующие команды?
 * ```tee```
 * ```awk```
 * ```tr```
 * ```cut```
 * ```tac```
 * ```curl```
 * ```wget```
 * ```watch```
 * ```head```
 * ```tail```
 * ```less```
 * ```cat```
 * ```touch```
 * ```sar```
 * ```netstat```
 * ```tcpdump```
 * ```lsof```
 * ```cpio```
 * ```ps```
 * ```nohup```
 
 <a href="https://dev-engineer.blogspot.com/2019/11/linux_44.html"> Вопросы с ответами </a>
 
#### [[⬆]](#toc) <a name='references'>Other Great References:</a>

Другие интересные ссылки(некоторые вопросы были позаимствованы):

* https://github.com/darcyclarke/Front-end-Developer-Interview-Questions
* https://github.com/kylejohnson/linux-sysadmin-interview-questions/blob/master/test.md
* http://slideshare.net/kavyasri790693/linux-admin-interview-questions
* http://blog.sedicomm.com/2019/09/25/40-voprosov-dlya-sobesedovaniya-na-temu-linux/
