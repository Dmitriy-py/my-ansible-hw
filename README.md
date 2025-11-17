# Домашнее задание к занятию 1 «Введение в Ansible»

## ` Дмитрий Климов `

Подготовка к выполнению
Установите Ansible версии 2.10 или выше.
Создайте свой публичный репозиторий на GitHub с произвольным именем.
Скачайте Playbook из репозитория с домашним заданием и перенесите его в свой репозиторий.
Основная часть
Попробуйте запустить playbook на окружении из test.yml, зафиксируйте значение, которое имеет факт some_fact для указанного хоста при выполнении playbook.
Найдите файл с переменными (group_vars), в котором задаётся найденное в первом пункте значение, и поменяйте его на all default fact.
Воспользуйтесь подготовленным (используется docker) или создайте собственное окружение для проведения дальнейших испытаний.
Проведите запуск playbook на окружении из prod.yml. Зафиксируйте полученные значения some_fact для каждого из managed host.
Добавьте факты в group_vars каждой из групп хостов так, чтобы для some_fact получились значения: для deb — deb default fact, для el — el default fact.
Повторите запуск playbook на окружении prod.yml. Убедитесь, что выдаются корректные значения для всех хостов.
При помощи ansible-vault зашифруйте факты в group_vars/deb и group_vars/el с паролем netology.
Запустите playbook на окружении prod.yml. При запуске ansible должен запросить у вас пароль. Убедитесь в работоспособности.
Посмотрите при помощи ansible-doc список плагинов для подключения. Выберите подходящий для работы на control node.
В prod.yml добавьте новую группу хостов с именем local, в ней разместите localhost с необходимым типом подключения.
Запустите playbook на окружении prod.yml. При запуске ansible должен запросить у вас пароль. Убедитесь, что факты some_fact для каждого из хостов определены из верных group_vars.
Заполните README.md ответами на вопросы. Сделайте git push в ветку master. В ответе отправьте ссылку на ваш открытый репозиторий с изменённым playbook и заполненным README.md.
Предоставьте скриншоты результатов запуска команд.

## Ответ:


<img width="1920" height="1080" alt="Снимок экрана (1875)" src="https://github.com/user-attachments/assets/e6e48e38-684a-4790-8602-9742add702f4" />


<img width="1920" height="1080" alt="Снимок экрана (1874)" src="https://github.com/user-attachments/assets/84115fff-91cb-4698-8c5d-487ee16c29a0" />

<img width="1920" height="1080" alt="Снимок экрана (1873)" src="https://github.com/user-attachments/assets/091c4244-25e4-4e65-afea-2d89c670398f" />

<img width="1920" height="1080" alt="Снимок экрана (1872)" src="https://github.com/user-attachments/assets/d0fa7433-d1f3-4616-8b21-e40553ef66b1" />

<img width="1920" height="1080" alt="Снимок экрана (1870)" src="https://github.com/user-attachments/assets/d2aa66e7-2d59-4eb0-b10b-8a02c18c6159" />

<img width="1920" height="1080" alt="Снимок экрана (1869)" src="https://github.com/user-attachments/assets/b8d4a4f6-298c-4e0c-ba99-a08060e7cac8" />

<img width="1920" height="1080" alt="Снимок экрана (1868)" src="https://github.com/user-attachments/assets/f7bb99e8-1050-44c8-b2fd-8711addb36bf" />
