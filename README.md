===========================================================

**Дипломный проект по профессии java-разработчик.**

Проект выполнен Командой 1(IND 13). Состав участников: Третьяков Кирилл , Аверьянов Александр, Самохвалов Алексей, Тарасов Максим.
Функционал:

Написан backend для интернет платформы объявлений по продаже вещей. Frontend часть была задана контейнером Docker.

- В проекте есть файл openapi.yaml, содержащий список конечных точек, к которым могут получить доступ пользователи. Эти конечные точки включают аутентификацию, регистрацию пользователей и различные действия, которые могут выполнять прошедшие проверку подлинности пользователи. Команда позаботилась о том, чтобы все конечные точки были безопасными. 
- Все API-методы приложения полностью идентичны методам в OpenAPI-спецификации.
- Все DTO содержат поля, которые совпадают по названиям и типам со схемами из OpenAPI-спецификации.
- Корректно работает функционал сохранения и получения картинок.
- 

**Доступ к функционалу в зависимости от типа пользователя:**

1. Анонимный пользователь:
- получение списка всех имеющихся объявлений.

2. Авторизованный пользователь(права доступа USER):
- получение списка всех имеющихся объявлений.
- получение конкретного объявления.
- создание, редактирование и удаление собственных объявлений.
- получение списка комментариев к любому объявлению.
- создание, редактирование и удаление собственных комментариев.

3. Авторизованный пользователь (права доступа ADMIN):

- получение списка всех имеющихся объявлений.
- получение списка всех имеющихся комментариев.
- создание, редактирование и удаление любых объявлений.
- создание, редактирование и удаление любых комментариев.

**Работа с базами данных.**
- Подключена удаленная БД PostgreSQL.
- Есть маппинг Entity в DTO и наоборот.
- Запросы делаются с помощью именования методов в спринговых репозиториях.
- Для управления схемой данных используется  Hibernate Framework.

Технологии, использованные в проекте

**Язык. Фреймворки. Библиотеки** - Java, Spring Framework, Spring Boot, Spring Security, Hibernate, Lombok, Mapstruct, SpringDoc OpenAPI UI

Прочее - Docker

===========================================================
