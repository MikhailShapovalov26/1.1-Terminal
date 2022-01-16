Домашнее задание к занятию "3.1. Работа в терминале, лекция 1"
===================================================
1. Установка Oracle VM VirtualBox
2. Установка Vagrant Hashicorp
3. Выполнено
4. Выполнено
5. Выполнено (RAM:1024 CPU:1 cpu HDD 64 gb video: 8 mb)
6. Можно дописать в ini файл строки:

                vb.memory = "1024" 
                vb.cpu = 2
7. Выполнено
8. 
    + HISTFILESIZE,Manual page bash(1) line 1033, HISTSIZE,  Manual page bash(1) line 1052. 
    + ignoreboth это команда используется всесто двух отдельных ignorespace и ignoredups. Не даёт сохранить строки начинающие с пробела и совпадающие с последней выполненой командой. 
9. {} -используются при использование списков, зарезервированных слов. Используются в циклах, или при ограничении тело функции. К примеру команда:

        touch /home/DevOps_{A..D}
        ls 
        DevOps_A  DevOps_B  DevOps_C  DevOps_D> 

(строка 304 { list; })
10. touch /home/DevOps_{00001..1000000}, 
не получится 3000000 даже на меньшее чило выдает ошибку:

        <touch test_{0000001..20000000}
        bash: /usr/bin/touch: Слишком длинный список аргументов> 
11. [[ -d /tmp ]] для проверки существования каталога tmp
12. 

        mkdir /tmp/new_path_dir/
        cp /bin/bash /tmp/new_path_dir/
        type -a bash
        bash is /usr/bin/bash
        bash is /bin/bash
        PATH=/tmp/new_path_dir/:$PATH
        type -a bash
        bash is /tmp/new_path_dir/bash
        bash is /usr/bin/bash
        bash is /bin/bash
13. Команда batch "Нет справочной страницы для batch"at "Нет справочной страницы для at"
14. vagrant suspend