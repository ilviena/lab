# Выполнено Ямалетдиновой И. И., гр. 432Б

### Установка
   
1.1 Установка Python и pip, проверила версию.

   <img width="485" height="146" alt="image" src="https://github.com/user-attachments/assets/355e20c1-c3fe-43fc-bd3b-260da8bfeb9f" />

1.2 Установила Ansible, проверила версию.

   <img width="802" height="265" alt="image" src="https://github.com/user-attachments/assets/beaba6d0-5adc-4549-ade0-e20b27b21588" />

   ---
   
### Подготовка SSH ключей
2.1 Сгенерировала SSH ключи командой `ssh-keygen -t rsa -b 4096 -f ~/.ssh/ansible_key -N ""`. Проверила ключи.

   <img width="744" height="463" alt="image" src="https://github.com/user-attachments/assets/3c1f6778-a314-4115-960e-67c17a5ce9ee" />

2.2 Установила права доступа на приватный ключ.

   <img width="543" height="75" alt="image" src="https://github.com/user-attachments/assets/1daad998-0f38-420e-965d-458ba5f651fc" />

---

### Запуск управляемого контейнера в Docker
3.1 Создала файлы *Dockerfile* и *docker-compose.yml*, вставила содержимое из репозитория методички.

   <img width="357" height="160" alt="image" src="https://github.com/user-attachments/assets/bf68bd74-cb63-4a49-b3fe-3d9054263a12" />

3.2 Собрала образ и запустила докер в фоновом режиме.

   <img width="546" height="169" alt="image" src="https://github.com/user-attachments/assets/ba312c68-d594-402b-b12b-eb07901fa058" />

3.3 Проверка контейнера:

   <img width="1014" height="175" alt="image" src="https://github.com/user-attachments/assets/d4b7c759-4da6-4104-87bc-3cf748e141c0" />

3.4 Создала директорию, скопировала публичный ключ в контейнер, установила правильные права.

  <img width="1069" height="169" alt="image" src="https://github.com/user-attachments/assets/3de43a1e-cd87-441b-a09e-b9cae9d2403a" />

---

### Проверка SSH подключение к контейнеру.

  <img width="829" height="268" alt="image" src="https://github.com/user-attachments/assets/57b66af6-e510-42b1-96bc-4d47078ffad6" />

---

### Создание инвентарного файла
5.1 Создала файл *inventori.ini*, вставила код из репозитория. Осуществила проверку командой `ansible-inventory -i inventory.ini --list`, вывел JSON формат.
   
   <img width="861" height="542" alt="image" src="https://github.com/user-attachments/assets/eb885489-55c1-47f8-9da0-ec44fa5ec064" />

---

### Проверка подключения Ansible к управляемому хосту
6.1 Тест *ping*.

   <img width="777" height="115" alt="image" src="https://github.com/user-attachments/assets/df27db9c-05f5-49d1-8d43-549503adba07" />

6.2 Сбор информации о системе.

<img width="754" height="301" alt="image" src="https://github.com/user-attachments/assets/b76dde7d-be3c-4060-9710-8305875587f8" />

6.3 Выполнение простой команды `ansible -i inventory.ini managed1 -m command -a "uname -a"`.

<img width="881" height="136" alt="image" src="https://github.com/user-attachments/assets/79812b0f-7494-4c8b-bee4-0daec5404f29" />

---

### Создание и запуск Ansible Playbook

7.1 Создала файл *playbook.yml*, вставила содержимое из репозитория.

<img width="526" height="239" alt="image" src="https://github.com/user-attachments/assets/075771f6-4e4f-4868-b55b-2eb2f380031a" />

7.2 Запустила *playbook.yml*.

<img width="773" height="513" alt="image" src="https://github.com/user-attachments/assets/9c84258a-64fd-41c2-898b-23775ab25407" />

---

### Базовые ad-hoc команды. Ошибок нет.

<img width="1068" height="145" alt="image" src="https://github.com/user-attachments/assets/40f1a4de-8e2e-4da5-9fd8-f1ca6cb19c82" />


---

### Работа с файлами
Создала новый *playbook* `task3_files.yml`. Запустила командой `ansible-playbook -i inventory.ini task3_files.yml`.

   <img width="811" height="489" alt="image" src="https://github.com/user-attachments/assets/cfe7c66b-0642-4763-a7a2-17425570053b" />


---

# Заключение
#### В ходе лабораторной работы были получены практические навыки использования *Ansible*.
