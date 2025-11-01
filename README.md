# Выполнено Ямалетдиновой И. И., гр. 432Б

### Ход работы:
1. Установка *Docker Desktop*. Вместе с ним автоматически устанавливаются *wsl + docker-compose*.
   
   <img width="577" height="347" alt="image" src="https://github.com/user-attachments/assets/3f39fda9-ec0d-413a-b12f-7c2b87a7f717" />

2. Далее была создана папка *first-docker*. В неё помещен файл *app.py* с *GitHub*.
3. В этой же папке создан *Dockerfile*. С помощью редактора *PyCharm* создан код внутри файла, учтен проброс порта 1234.
   
   <img width="326" height="243" alt="image" src="https://github.com/user-attachments/assets/ec5b96c3-d391-457a-8723-22ae49886262" />
4. В терминале *Docker Desktop* собрала образ с помощью команды `docker build -t my-image .`
   
   <img width="578" height="124" alt="image" src="https://github.com/user-attachments/assets/8ce91fa2-a795-4eab-824d-2a2b5f80503f" />
5. Теперь можно запустить контейнер с помощью команды `docker run -p 1234:1234 my-image`
   
   <img width="630" height="228" alt="image" src="https://github.com/user-attachments/assets/f8cc12bf-ac74-49a8-a9f0-c4b997728e12" />
6. Сейчас, переходя по ссылке `http://localhost:1234/`, можно увидеть надпись:

   <img width="431" height="150" alt="image" src="https://github.com/user-attachments/assets/55451ab4-58bc-4210-905b-e20e9bdaae6b" />
7. Следующим этапом было создание файла `docker-compose.yml`. В нем были прописаны следующие инструкции:

<img width="905" height="832" alt="image" src="https://github.com/user-attachments/assets/2d303425-6a26-41f8-9159-1528aedabe64" />

8. В терминале был пересобран образ. И запущен стек с помощью команды `docker compose up`.

   <img width="632" height="145" alt="image" src="https://github.com/user-attachments/assets/844835df-a954-4e35-b61f-01703fb5cb6f" />
9. Теперь, переходя по ссылке `http://localhost:1234/`, можно увидеть надпись:

<img width="426" height="129" alt="image" src="https://github.com/user-attachments/assets/9fb1f6c3-57fb-419d-b2a2-bf6a268d70d5" />

---

# Заключение
#### В ходе лабораторной работы были изучены основы контейнеризации с использованием *Docker*. Были освоены команды для управления контейнерами и образами, а также изучена надстройка *Docker-compose*, с помощью которой можно было запускать стек контейнеров.
