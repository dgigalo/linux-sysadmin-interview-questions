База знаний
====================================================

Вопросы собраны из разных источников интернета. Добавляйте свои


## <a name='toc'>Table of Contents</a>

  1. [Общие вопросы](#general)
  1. [Простые вопросы](#simple)
  1. [Вопросы среднего уровня](#medium)
  1. [Hard Linux Questions](#hard)
  1. [Expert Linux Questions](#expert)
  1. [MySQL Questions](#mysql)
  1. [DevOps Questions](#devop)
  1. [Веселые вопросы](#fun)
  1. [Сетевые вопросы](#web)
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
* Как принудительно заставить систему выполнить проверку файловой системы при следующем запуске? <br>
  Для этого нужно создать файл forcefsck в корневом разделе: touch /forcefsck <br>
* Напишите скрипт, чтобы посмотреть основную информацию о системе: hostname, IP адрес, залогинившихся пользователей, uptime, load average, статистику по оперативной памяти, подкачке и дисках.<br>
#!/bin/bash
hostname
hostname -I 
who
uptime
free
df -h	
<br>
<a href="https://dev-engineer.blogspot.com/2019/10/linux.html"> Вопросы с ответами </a>


#### [[⬆]](#toc) <a name='medium'>Вопросы среднего уровня:</a>

* Что обозначает ```&``` после команды?
* Что обозначает ```& disown``` после команды?
* Что такое фильтр пакетов (packet filter) и как он работает?
* Что такое виртуальная память(Virtual Memory)?
* Что такое swap и для чего используется?
* Что такое "sticky bit"?
* Для чего предназначен бит неизменяемости(immutable bit)?
* Что такое жесткая ссылка, символическая? Чем отличаются? Что произойдет если удалить источник, на который указывает ссылка?
* Что такое айнод(inode) и какие поля в нем хранятся?
* Что такое SNMP и для чего он используется?
* Как уменьшить размер файла, который используется в текущий момент(например, файла лога)?
* Что такое переадресация SSH-порта?
* Как добавить пользователя без использования команд useradd/adduser?
* Опишите команду mknod и расскажите когда вы её используете?
* Загрузка диского пространства 100%, вы удалили огромный файл логов, но df показывает - нет свободного места. В чем проблема?
* Вы получаете ошибку "filesystem is full", хотя 'df' говорит об обратном, место есть. В чем проблема?
* Расскажите как работает команда 'ps'.
* Что происходит с дочерним процессом, который завершил свое выполнение, но у которого нет родительского процесса ожидающего его завершение? Почему это плохо?
* Кратко опишите каждое состояние процесса(process states) в ОС Linux.
* Вы запускаете скрипт и хотите посмотреть вывод в терминале и сохранить в файл, как это можно сделать?
* Объясните, что выполнит данная команда echo "1" > /proc/sys/net/ipv4/ip_forward
* Какие типы файлов вы знаете в ОС Linux?
* В чем разница между процессом и потоком?
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
* What is MAJOR and MINOR numbers of special files?

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
* Что такое ELK-стек? Расскажите про основные компоненты. 

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

#### [[⬆]](#toc) <a name='web'>Сетевые вопросы:</a>
* Какую функцию выполняет DNS в сети?<br>
  DNS — система для получения информации о доменах. Чаще всего используется для получения IP-адреса по имени хоста, получения информации о маршрутизации почты. <br>
* Какие записи ДНС вы знаете, для чего они используются? <br>
  Записи DNS, или ресурсные записи (resource records), — единицы хранения и передачи информации в DNS.
  Запись A (address record) или запись адреса связывает имя хоста с адресом протокола IPv4
  Запись AAAA (IPv6 address record) связывает имя хоста с адресом протокола IPv6.
  Запись CNAME (canonical name record) или каноническая запись имени (псевдоним) используется для перенаправления на другое имя.
  Запись MX (mail exchange) или почтовый обменник указывает сервер(ы) обмена почтой для данного домена.
  Запись NS (name server) указывает на DNS-сервер для данного домена.
  Запись PTR (pointer[5][6]) обратная DNS-запись или запись указателя связывает IP-адрес хоста с его каноническим именем.<br>
* Что такое HTTP? <br>
  HTTP (от англ. HyperText Transfer Protocol — протокол передачи гипертекста) — это прикладной протокол передачи данных в сети.<br>
* Что такое HTTP-proxy и как он работает? <br>
  Сервер-посредник — промежуточный сервер в сети, выполняющий роль посредника между пользователем и целевым сервером, позволяющий клиентам как выполнять косвенные запросы (принимая и передавая их через прокси-сервер) к другим сетевым службам, так и получать ответы. Клиент подключается к прокси-серверу и запрашивает какой-либо ресурс, расположенный на другом сервере. Затем прокси-сервер либо подключается к указанному серверу и получает ресурс у него, либо возвращает ресурс из собственного кэша (в случаях, если прокси имеет свой кэш). <br>
* Кратко опишите как работает HTTPS.<br>
  HTTPS не является отдельным протоколом передачи данных, а представляет собой расширение протокола HTTP с надстройкой шифрования, т.к.
передаваемые по протоколу HTTP данные не защищены. <br>
* На каком уровне работает протокол HTTP? А протокол HTTPS? В чем различие HTTP и HTTPS<br>
  На прикладном уровне. <br>
  HTTPS (от англ. HyperText Transfer Protocol Secure — безопасный протокол передачи гипертекста) — это расширение протокола HTTP,   поддерживающее шифрование посредством криптографических протоколов SSL и TLS. <br>
  HTTPS обеспечивает конфиденциальность информации путем ее шифрования;<br>
  HTTP использует порт 80, HTTPS — порт 443.<br>
* Что означает директива upstream в настройках nginx'a? <br>
  Данная директива включает балансировку нагрузки. По умолчанию, соединения распределяются по серверам циклически (в режиме round-robin) с учётом весов серверов.<br>
* Кратко опишите действия по созданию и установке ssl-сертифката для сайта https://foo.example.com <br>
  1. Купить сертификат у проверенного центра авторизации или сгенерировать само подписанный
  2. В настройках вашего сервера включить поддержку ssl и указать путь к сертификату. <br>
* Можно ли использовать несколько SSL-хостов на одном айпи-адресе? <br>
  Да, с помощью веб-сервера это можно сделать. <br>
* Что такое wildcard сертификат?
  Wildcard-сертификат — сертификат открытого ключа, который может использоваться с несколькими поддоменами.
Например, один сертификат для *.example.com обеспечит домены payment.example.com, contact.example.com, login-secure.example.com <br>
* Что такое NAT, как он работает и зачем нужен?<br>
  NAT (Network Address Translation) – технология преобразовывания приватных IP-адресов во внешние в IPv4. Благодаря этому процессу ваша виртуальная машина получает доступ в Интернет. Механизм NAT как раз осуществляет подмену (или «маскировку») серых адресов на белые и наоборот. <br>
* На каком уровне коммуникационной модели OSI возможны сжатие и шифрование данных? <br>
  Уровень представления (англ. Presentation layer) — шестой уровень сетевой модели OSI. Этот уровень отвечает за преобразование протоколов и кодирование/декодирование данных. Запросы приложений, полученные с уровня приложений, он преобразует в формат для передачи по сети, а полученные из сети данные преобразует в формат, понятный приложениям.<br>
* Какие порты, согласно решению IANA, являются зарезервированными (Registered Ports)? <br>
  Зарегистрированными или пользовательскими портами являются 1024-49151 <br>
* Что такое TCP? <br>
  Transmission Control Protocol - Транспортный протокол передачи данных в сетях TCP/IP, предварительно устанавливающий соединение с сетью.<br>
* Что такое UDP? <br>
  User Datagram Protocol - Транспортный протокол, передающий сообщения-датаграммы без необходимости установки соединения в IP-сети. <br>
* Чем отличается TCP от UDP? <br>
  TCP исключает потери данных, дублирование и перемешивание пакетов, задержки. UDP все это допускает, и соединение для работы ему не требуется. <br>
* What is localhost and why would ```ping localhost``` fail?
* What is the similarity between "ping" & "traceroute" ? How is traceroute able to find the hops.
* What is the command used to show all open ports and/or socket connections on a machine?
* Is 300.168.0.123 a valid IPv4 address?
* Which IP ranges/subnets are "private" or "non-routable" (RFC 1918)?
* What is a VLAN?
* What is ARP and what is it used for?
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

#### [[⬆]](#toc) <a name='demo'>Практикум</a>

* В директории 500 файлов, необходимо найти все файлы свыше 20 ГБ, отсортировать по размеру, отобразить 5 самых больших файлов.
* Как разделить файл на несколько частей без архиватора? Например, 10 гб файл разделить по 1 гб.
* Распакуйте test.tar.gz без использрования google и справки.
* Рекурсивно удалите все файлы с раширением "*.pyc" из тестовой директории?
* Найдите строку "my konfu is the best" во всех файлах с расширением *.py.
* Замените вхождение фразы "my konfu is the best" на "I'm a linux jedi master" во всех *.txt файлах.
* Проверить доступность 443 порта на машине с IP-адресом X.X.X.X
* Получить содержимое http://myinternal.webserver.local/test.html с помощью telnet'a.
* Отправить письмо используя командную строку(command line).
* Найти все файлы, которые использовались за последние 30 дней.
* Объясните следующую команду ```(date ; ps -ef | awk '{print $1}' | sort | uniq | wc -l ) >> Activity.log```
* Как узнать какой процесс запущен на определенном порту?
* Write a ```get_prim``` method in python/perl/bash/pseudo.
* Write a script to list all the differences between two directories.
* In a log file with contents as ```<TIME> : [MESSAGE] : [ERROR_NO] - Human readable text``` display summary/count of specific error numbers that occurred every hour or a specific hour.

<a href="https://dev-engineer.blogspot.com/2019/11/linux_28.html"> Вопросы с ответами </a>

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
