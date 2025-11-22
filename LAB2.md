# Выполнено Ямалетдиновой И. И., гр. 432Б

### Ход работы:
1. Авторизировалась на *Jenkins*, создала *item*, указав уникальные данные проекта.
   
  <img width="598" height="345" alt="image" src="https://github.com/user-attachments/assets/0df4f60d-95e7-4115-a110-88a777422f1f" />


2. В списке типов проектов выбрала *Pipeline* и вставила заготовленный скрипт, заранее отредактировав его.

   <img width="1291" height="610" alt="image" src="https://github.com/user-attachments/assets/f65bdbf3-2264-4e8c-9d1c-1e57be8500db" />

4. Запустила сборку, результат успешный.

   <img width="285" height="90" alt="image" src="https://github.com/user-attachments/assets/18bde64a-7232-40c5-a5c6-e608b35412a8" />


3. Перейдя по адресу `http://158.160.194.244:8085/`, можно увидеть результат работы.

   <img width="1920" height="978" alt="image" src="https://github.com/user-attachments/assets/3e110920-c43c-48a1-a05b-c3f2102a91a3" />

5. Далее необходимо было настроить *GitHub webhook* для автоматического запуска сборки. Это делается через меню *Settings* > *Webhooks* > *Add webhook*.
   В поле *Payload URL* ввела адрес *Jenkins* вебхука.

7. Изменила в файле *index.html* цвет текста на белый. Снова инициировала сборку, появилось окошко.

   <img width="425" height="149" alt="image" src="https://github.com/user-attachments/assets/d446bcb6-6260-4ea2-bfe9-eba9c873df20" />
   

8. Вывод на `http://158.160.194.244:8085/` изменился.

   <img width="1920" height="981" alt="image" src="https://github.com/user-attachments/assets/b965d0c9-f557-4104-944e-0595b5390820" />

---

# Заключение
#### В ходе лабораторной работы были получены практические навыки автоматизации процесса непрерывной интеграции и развертывания (CI/CD) с использованием Jenkins.
