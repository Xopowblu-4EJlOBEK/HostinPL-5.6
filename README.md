# HostinPL-5.6 Nulled
Панель управления игровым хостингом HostinPL 5.6 (Nulled by PavelDolmatov vipadmin.club)

Modify by Xopowblu-4EJlOBEK
> *Что изменено:*
> 1. Исправлены ошибки в установщике
> 2. Файлы серверов перенесены на GIT для стабильности доступа (на случай если сайт-первоисточник "ляжет")
> 3. В панели вырезаны все шеллы/дыры

## Поддержка систем
+ **Debian 9**
 
## Установка
**Утанавливать как панель так и локацию рекомендуется на чистую машину.**

*(Если вы устанавливаете с архива, переходите к пункту с установкой прав на запуск файла install)*

Перед установкой панели/локации, установите GIT командой:
> sudo apt-get update && sudo apt-get install git -y

Далее перейдите в директорию /usr/src:
> cd /usr/src

Потом клонируйте этот репозиторий командой:
> sudo git clone https://github.com/Xopowblu-4EJlOBEK/HostinPL-5.6.git

После идем в папку с репозиторием:
> cd HostinPL-*

Далее установите права на выполнение на файл install командой:
> sudo chmod +x install

И запустите установку:
> sudo ./install

Все команды одной строккой (для ленивых, скопировал - вставил - выполнил):
> sudo apt-get update && sudo apt-get install git -y && cd /usr/src && sudo git clone https://github.com/Xopowblu-4EJlOBEK/HostinPL-5.6.git && cd HostinPL-* && sudo chmod +x install && sudo ./install

## Рекомендуемые требования к системе с панелью
+ ОЗУ: 1024 Мб
+ Ядра процессора: 2
+ Диск: 10 Гб

## Рекомендуемые требования к системе с локацией
+ ОЗУ: 2048 Мб
+ Ядра процессора: 2
+ Диск: 100+ Гб (Зависит от планируемого количества серверов. Оптимально выделять 1-2 Гб на сервер)
---
Данная панель предоставлена чисто в ознакомительных целях. Используйте ее на свой страх и риск. Поддержка дополнительных систем в будущем.
