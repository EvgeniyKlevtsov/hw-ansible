Самоконтроль выполнения задания
Где расположен файл с some_fact из второго пункта задания?
Какая команда нужна для запуска вашего playbook на окружении test.yml?
Какой командой можно зашифровать файл?
Какой командой можно расшифровать файл?
Можно ли посмотреть содержимое зашифрованного файла без команды расшифровки файла? Если можно, то как?
Как выглядит команда запуска playbook, если переменные зашифрованы?
Как называется модуль подключения к host на windows?
Приведите полный текст команды для поиска информации в документации ansible для модуля подключений ssh
Какой параметр из модуля подключения ssh необходим для того, чтобы определить пользователя, под которым необходимо совершать подключение?
Ответ:

group_vars/all/example.yml
ansible-playbook -i inventory/test.yml site.yml
ansible-vault encrypt group_vars/el/exampl.yml
ansible-vault decrypt group_vars/el/exampl.yml
ansible-vault view group_vars/deb/exampl.yml
ansible-playbook -i inventory/prod.yml site.yml --ask-vault-password // с ключом --ask-vault-password
winrm - Run tasks over Microsoft's WinRM
ansible-doc -t connection ssh
remote_user or ansible_user or ansible_ssh_user
