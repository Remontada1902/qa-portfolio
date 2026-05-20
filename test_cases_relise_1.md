# Project_store manager релиз 1

|ID|Расположение|Наименование|Предусловия|Шаги|Постусловия|Ожидаемый результат|Приоритет|Статус|
|---|---|---|---|---|---|---|---|---|
|75|store manager релиз 1 -> Экран регистрации|[открыта форма регистрации](https://team-fn99.testit.software/projects/1/tests/75)|||||Средний|Готов|
|||||открыть страницу регистраци http://localhost:8000/register/ и нажать кнопку “Зарегистрируйтесь”||открылась форма для регистрации  есть надписи в полях:  •  Подсказка (placeholder): «Email».  •  Подсказка (placeholder): «Имя пользователя».  •  Подсказка (placeholder): «Пароль».|||
|72|store manager релиз 1 -> Экран регистрации|[UI-1 Успешная регистрация](https://team-fn99.testit.software/projects/1/tests/72)|||||Средний|Готов|
|||||открыть страницу регистраци http://localhost:8000/register/ и нажать кнопку “Зарегистрируйтесь”||открылась форма для регистрации  есть надписи в полях:  •  Подсказка (placeholder): «Email».  •  Подсказка (placeholder): «Имя пользователя».  •  Подсказка (placeholder): «Пароль».|||
|||||ввести валидные значения Имя пользователя, Email, Пароль нажать Зарегистрироваться||успешная регистрация зеленое уведомление с текстом «Регистрация прошла успешно». и перенаправление на страницу входа|||
|73|store manager релиз 1 -> Экран регистрации|[UI-2 Ошибка регистрации Имя пользователя 2 символа](https://team-fn99.testit.software/projects/1/tests/73)|||||Средний|Готов|
|||||открыть страницу регистраци http://localhost:8000/register/ и нажать кнопку “Зарегистрируйтесь”||открылась форма для регистрации  есть надписи в полях:  •  Подсказка (placeholder): «Email».  •  Подсказка (placeholder): «Имя пользователя».  •  Подсказка (placeholder): «Пароль».|||
|||||ввести в поле “Имя пользователя” 2 символа  ввести валидные значения: Email, Пароль и нажать Зарегистрироваться||отобразилось красное уведомление об ошибке, что введено меньше 3 символов|||
|76|store manager релиз 1 -> Экран регистрации|[UI-3 Ошибка регистрации Имя пользователя 51 символ](https://team-fn99.testit.software/projects/1/tests/76)|||||Средний|Готов|
|||||открыть страницу регистраци http://localhost:8000/register/ и нажать кнопку “Зарегистрируйтесь”||открылась форма для регистрации  есть надписи в полях:  •  Подсказка (placeholder): «Email».  •  Подсказка (placeholder): «Имя пользователя».  •  Подсказка (placeholder): «Пароль».|||
|||||ввести в поле “Имя пользователя” 51 символ  ввести валидные значения: Email, Пароль и нажать Зарегистрироваться||отобразилось красное уведомление об ошибке, что введено больше 50 символов|||
|77|store manager релиз 1 -> Экран регистрации|[UI-4 Ошибка регистрации  “email ” невалидное значение](https://team-fn99.testit.software/projects/1/tests/77)|||||Средний|Готов|
|||||открыть страницу регистраци http://localhost:8000/register/ и нажать кнопку “Зарегистрируйтесь”||открылась форма для регистрации  есть надписи в полях:  •  Подсказка (placeholder): «Email».  •  Подсказка (placeholder): «Имя пользователя».  •  Подсказка (placeholder): «Пароль».|||
|||||ввести в поле “email ” невалидное значение (например 1234mail.ru)  ввести валидные значения: Имя пользователя, Пароль и нажать Зарегистрироваться||красное уведомление об ошибке - email не соответствует стандартному формату|||
|78|store manager релиз 1 -> Экран регистрации|[UI-5 Ошибка регистрации  email уже зарегистрирован](https://team-fn99.testit.software/projects/1/tests/78)|||||Средний|Готов|
|||||открыть страницу регистраци http://localhost:8000/register/ и нажать кнопку “Зарегистрируйтесь”||открылась форма для регистрации  есть надписи в полях:  •  Подсказка (placeholder): «Email».  •  Подсказка (placeholder): «Имя пользователя».  •  Подсказка (placeholder): «Пароль».|||
|||||ввести в поле “email ” значение, ранее зарегистрированное   ввести валидные значения: Имя пользователя, Пароль и нажать Зарегистрироваться||красное уведомление об ошибке - email уже зарегистрирован|||
|79|store manager релиз 1 -> Экран регистрации|[UI-6 Ошибка регистрации  пароль меньше 8 символов](https://team-fn99.testit.software/projects/1/tests/79)|||||Средний|Готов|
|||||открыть страницу регистраци http://localhost:8000/register/ и нажать кнопку “Зарегистрируйтесь”||открылась форма для регистрации  есть надписи в полях:  •  Подсказка (placeholder): «Email».  •  Подсказка (placeholder): «Имя пользователя».  •  Подсказка (placeholder): «Пароль».|||
|||||ввести в поле “пароль” значение, меньше 8 символов  ввести валидные значения: Имя пользователя, email и нажать Зарегистрироваться||красное уведомление об ошибке - пароль меньше 8 символов  Пароль должен быть скрыт (знаки вместо символов).|||
|80|store manager релиз 1 -> Экран регистрации|[UI-7 Ошибка регистрации не заполнено обязательное поле](https://team-fn99.testit.software/projects/1/tests/80)|||||Средний|Готов|
|||||открыть страницу регистраци http://localhost:8000/register/ и нажать кнопку “Зарегистрируйтесь”||открылась форма для регистрации  есть надписи в полях:  •  Подсказка (placeholder): «Email».  •  Подсказка (placeholder): «Имя пользователя».  •  Подсказка (placeholder): «Пароль».|||
|||||не заполнять поле “пароль”  ввести валидные значения: Имя пользователя, email и нажать Зарегистрироваться||уведомление - не заполнено обязательное поле|||
|||||не заполнять поле “имя пользователя”  ввести валидные значения: пароль, email и нажать Зарегистрироваться||уведомление - не заполнено обязательное поле|||
|||||не заполнять поле “email”  ввести валидные значения: имя пользователя, пароль и нажать Зарегистрироваться||уведомление - не заполнено обязательное поле|||
|81|store manager релиз 1 -> Экран авторизации|[логин](https://team-fn99.testit.software/projects/1/tests/81)|||||Средний|Готов|
|||||открыть страницу входа http://localhost:8000/login/||открыта страница  есть подсказки •  Подсказка (placeholder): «Email».  •  Подсказка (placeholder): «Пароль».   есть кнопка для перехода на экран регистрации («Нет аккаунта? Зарегистрируйтесь»).  есть кнопка «запомнить меня» для сохранения токена авторизации.|||
|82|store manager релиз 1 -> Экран авторизации|[UI-8 Авторизация - успешная](https://team-fn99.testit.software/projects/1/tests/82)|||||Средний|Готов|
|||||открыть страницу входа http://localhost:8000/login/||открыта страница  есть подсказки •  Подсказка (placeholder): «Email».  •  Подсказка (placeholder): «Пароль».   есть кнопка для перехода на экран регистрации («Нет аккаунта? Зарегистрируйтесь»).  есть кнопка «запомнить меня» для сохранения токена авторизации.|||
|||||ввести корректный email и пароль||есть доступ к системе|||
|83|store manager релиз 1 -> Экран авторизации|[UI-9 Авторизация - ошибка ](https://team-fn99.testit.software/projects/1/tests/83)|||||Средний|Готов|
|||||открыть страницу входа http://localhost:8000/login/||открыта страница  есть подсказки •  Подсказка (placeholder): «Email».  •  Подсказка (placeholder): «Пароль».   есть кнопка для перехода на экран регистрации («Нет аккаунта? Зарегистрируйтесь»).  есть кнопка «запомнить меня» для сохранения токена авторизации.|||
|||||ввести некорректный email и корректный пароль||выводится красное уведомление об ошибке: «Неверный email или пароль».|||
|||||ввести корректный email и некорректный пароль||выводится красное уведомление об ошибке: «Неверный email или пароль».|||
|90|store manager релиз 1 -> Экран авторизации|[Открытие экрана авторизации в Chrome на ПК](https://team-fn99.testit.software/projects/1/tests/90)|||||Средний|Готов|
|||||открыть экран авторизации в браузере CHROME на ПК||экран успешно открыт|||
|94|store manager релиз 1 -> Экран авторизации|[Открытие экрана авторизации в Chrome на мобил](https://team-fn99.testit.software/projects/1/tests/94)|||||Средний|Готов|
|||||открыть экран авторизации в браузере CHROME на мобил||экран успешно открыт|||
|91|store manager релиз 1 -> Экран авторизации|[Открытие экрана авторизации в Firefox на ПК](https://team-fn99.testit.software/projects/1/tests/91)|||||Средний|Готов|
|||||открыть экран авторизации в браузере Firefox на ПК||экран успешно открыт|||
|95|store manager релиз 1 -> Экран авторизации|[Открытие экрана авторизации в Firefox на мобил](https://team-fn99.testit.software/projects/1/tests/95)|||||Средний|Готов|
|||||открыть экран авторизации в браузере Firefox на мобил||экран успешно открыт|||
|92|store manager релиз 1 -> Экран авторизации|[Открытие экрана авторизации в Safari на пк](https://team-fn99.testit.software/projects/1/tests/92)|||||Средний|Готов|
|||||открыть экран авторизации в браузере Safari на пк||экран успешно открыт|||
|96|store manager релиз 1 -> Экран авторизации|[Открытие экрана авторизации в Safari на мобил](https://team-fn99.testit.software/projects/1/tests/96)|||||Средний|Готов|
|||||открыть экран авторизации в браузере Safari на мобил||экран успешно открыт|||
|93|store manager релиз 1 -> Экран авторизации|[Открытие экрана авторизации в Edge на пк](https://team-fn99.testit.software/projects/1/tests/93)|||||Средний|Готов|
|||||открыть экран авторизации в браузере Edge на пк||экран успешно открыт|||
|97|store manager релиз 1 -> Экран авторизации|[Открытие экрана авторизации в Edge на мобил](https://team-fn99.testit.software/projects/1/tests/97)|||||Средний|Готов|
|||||открыть экран авторизации в браузере Edge на мобил||экран успешно открыт|||
|98|store manager релиз 1 -> Экран управления продуктами|[Отображение только одобренных продуктов](https://team-fn99.testit.software/projects/1/tests/98)|||||Средний|Готов|
||||Пользователь авторизован в системе.|||В базе данных есть продукты: Product A (is_available=true), Product B (is_available=true), Product C (is_available=false)|||
|||||Перейти на страницу "Управление продуктами||Отображаются только продукты с is_available = true (Product A и Product B). Product C не отображается|||
|99|store manager релиз 1 -> Экран управления продуктами|[«Добавить новый продукт»](https://team-fn99.testit.software/projects/1/tests/99)|||||Средний|Готов|
|||||авторизоваться в системе||отображается Кнопка «Добавить новый продукт»|||
|||||нажать Кнопку «Добавить новый продукт»||Открывает модальное окно для создания нового продукта или редактирования.|||
|100|store manager релиз 1 -> Экран управления продуктами|[Заголовок страницы: «Управление продуктами».](https://team-fn99.testit.software/projects/1/tests/100)|||||Средний|Готов|
|||||авторизоваться в системе||отображается Заголовок страницы: «Управление продуктами».|||
|101|store manager релиз 1 -> Экран управления продуктами|[поиска продукта по названию](https://team-fn99.testit.software/projects/1/tests/101)|||||Средний|Готов|
||||||||||
|84|store manager релиз 1 -> Экран супер-админа|[UI-10 Проверка столбцов Таблицы с пользователями](https://team-fn99.testit.software/projects/1/tests/84)|||||Средний|Готов|
|||||выполнена авторизация на сайте под ролью супер-админа||Доступна Таблица с пользователями и столбцы: •  ID (UUID).  •  Имя.  •  Email.  •  Роль (супер-админ/обычный пользователь).   таблица поддерживает постраничную навигацию (pagination) (после 10 записей).|||
|85|store manager релиз 1 -> Экран супер-админа|[авторизация супер админ](https://team-fn99.testit.software/projects/1/tests/85)|||||Средний|Готов|
|||||выполнена авторизация на сайте под ролью супер-админа||Доступна Таблица с пользователями: Столбцы: •  ID (UUID).  •  Имя.  •  Email.  •  Роль (супер-админ/обычный пользователь)|||
|86|store manager релиз 1 -> Экран супер-админа|[UI-11 поиск в таблице](https://team-fn99.testit.software/projects/1/tests/86)|||||Средний|Готов|
|||||выполнена авторизация на сайте под ролью супер-админа||Доступна Таблица с пользователями: Столбцы: •  ID (UUID).  •  Имя.  •  Email.  •  Роль (супер-админ/обычный пользователь)|||
|||||выполнить поиск по имени||успешный поиск|||
|||||выполнить поиск по email||успешный поиск|||
|87|store manager релиз 1 -> Экран супер-админа|[UI-12 фильтр по статусу супер-админ](https://team-fn99.testit.software/projects/1/tests/87)|||||Средний|Готов|
|||||выполнена авторизация на сайте под ролью супер-админа||Доступна Таблица с пользователями: Столбцы: •  ID (UUID).  •  Имя.  •  Email.  •  Роль (супер-админ/обычный пользователь)|||
|||||выполнить фильтр по статусу супер-админ||отображены пользователи с ролью супер админ  отсутствует Кнопка «Повысить до супер-админа» в|||
|88|store manager релиз 1 -> Экран супер-админа|[UI-13 фильтр по статусу обычный пользователь](https://team-fn99.testit.software/projects/1/tests/88)|||||Средний|Готов|
|||||выполнена авторизация на сайте под ролью супер-админа||Доступна Таблица с пользователями: Столбцы: •  ID (UUID).  •  Имя.  •  Email.  •  Роль (супер-админ/обычный пользователь)|||
|||||выполнить фильтр по статусу обычный пользователь||отображены пользователи с ролью обычный пользователь имеется Кнопка «Повысить до супер-админа» в строке каждого пользователя|||
|102|store manager релиз 1 -> API|[Регистрация - успешная](https://team-fn99.testit.software/projects/1/tests/102)|||||Самый высокий|Готов|
|||||1. Выполнить POST-запрос на /register/ с валидными name (3-50 символов), email, password (минимум 8 символов)  {   "name": "Иван Петров",   "email": "ivan.petrov@example.com",   "password": "password123" }||Ответ Статус 201 Created.  В ответе сообщение об успешной регистрации|||
|||||выполнить в pfAdmin  SELECT * FROM public.users ORDER BY id ASC||В БД появилась запись с переданными данными  Пароль сохранен в виде bcrypt хеша Пользователь создан как limited_user  is_superadmin = false|||
|103|store manager релиз 1 -> API|[Регистрация - email уже существует](https://team-fn99.testit.software/projects/1/tests/103)|||||Высокий|Готов|
||||проверить данные в БД|||есть пользователь  { "name": "Иван Петров", "email": "ivan.petrov@example.com", "password": "password123" }|||
|||||Выполнить POST-запрос на /register/   { "name": "Иван Петров", "email": "ivan.petrov@example.com", "password": "password123" }||Получено Сообщение об ошибке, что email уже зарегистрирован  400 {     "detail": "Email already registered" }|||
|||||выполнить в pfAdmin  SELECT * FROM public.users ORDER BY id ASC||Новый пользователь не создан в БД|||
|104|store manager релиз 1 -> API|[Регистрация - имя из пробелов](https://team-fn99.testit.software/projects/1/tests/104)|||||Средний|Готов|
|||||1. Выполнить POST-запрос на /register/ с name = 3 пробела "name": "   ", "email": "ivan@example.com", "password": "password123"||Статус 422 Validation Error  Сообщение об ошибке валидации имени "msg": "ensure this value has at least 3 characters", "type": "value_error.any_str.min_length", "ctx": { "limit_value": 3|||
|||||выполнить в pfAdmin  SELECT * FROM public.users ORDER BY id ASC||Пользователь отсутствует БД|||
|105|store manager релиз 1 -> API|[Регистрация - имя больше 50 символов](https://team-fn99.testit.software/projects/1/tests/105)|||||Высокий|Готов|
|||||Выполнить POST-запрос на /register/ с name = 51 символ  { "name": "ИванПетровааааааааааааап51", "email": "ivan@example.com", "password": "password123" }||Статус 422 Validation Error\n2. Сообщение об ошибке валидации имени|||
|||||выполнить в pfAdmin  SELECT * FROM public.users ORDER BY id ASC||Пользователь не создан|||
|106|store manager релиз 1 -> API|[Регистрация - невалидный email](https://team-fn99.testit.software/projects/1/tests/106)|||||Высокий|Готов|
|||||1. Выполнить POST-запрос на /register/ с email = "not-an-email"  {   "name": "Тест Тест",   "email": "not-an-email",   "password": "password123" }||Статус 422 Validation Error  Сообщение об ошибке валидации email|||
|||||выполнить в pfAdmin  SELECT * FROM public.users ORDER BY id ASC||Пользователь не создан|||
|107|store manager релиз 1 -> API|[Регистрация - пароль меньше 8 символов](https://team-fn99.testit.software/projects/1/tests/107)|||||Высокий|Готов|
|||||Выполнить POST-запрос на /register/ с password = 7 символов  {   "name": "Тест Тест",   "email": "fail@example.com",   "password": "1234567" }||Статус 422 Validation Error  Сообщение об ошибке валидации пароля|||
|||||выполнить в pfAdmin  SELECT * FROM public.users ORDER BY id ASC||Пользователь не создан|||
|108|store manager релиз 1 -> API|[Регистрация - отсутствует обязательное поле](https://team-fn99.testit.software/projects/1/tests/108)|||||Высокий|Готов|
|||||1. Выполнить POST-запрос на /register/ без поля name (или email, или password)||1. Статус 422 Validation Error\n2. Сообщение об ошибке|||
|||||выполнить в pfAdmin  SELECT * FROM public.users ORDER BY id ASC||Новый пользователь не создан в БД|||
|109|store manager релиз 1 -> API|[Авторизация - успешная](https://team-fn99.testit.software/projects/1/tests/109)|||||Средний|Готов|
||||Пользователь зарегистрирован    "email": "ivan.petrov@example.com",   "password": "password123"||||||
|||||Выполнить POST-запрос на /login/    "email": "ivan.petrov@example.com",   "password": "password123"||Статус 200 OK  В ответе access_token (JWT)\token_type = "bearer"  Время жизни токена 30 минут|||
|110|store manager релиз 1 -> API|[Авторизация - неверный пароль](https://team-fn99.testit.software/projects/1/tests/110)|||||Высокий|Готов|
||||Пользователь зарегистрирован     "email": "ivan.petrov@example.com",   "password": "password123"||||||
|||||Выполнить POST-запрос на /login/ с email "ivan.petrov@example.com", и неверным паролем||Статус 400 Bad Request Сообщение "Invalid email or password Токен не выдан|||
|111|store manager релиз 1 -> API|[Авторизация - несуществующий email](https://team-fn99.testit.software/projects/1/tests/111)|||||Высокий|Готов|
|||||Выполнить POST-запрос на /login/ с email, которого нет в БД "email": "nonexistent@example.com", "password": "password123"||Статус 400 Bad Request  Сообщение "Invalid email or password  Токен не выдан|||
|113|store manager релиз 1 -> API|[Просмотр данных - с невалидным токеном](https://team-fn99.testit.software/projects/1/tests/113)|||||Средний|Готов|
|||||Выполнить GET-запрос на /users/ с невалидным токеном в заголовке Authorization||ошибка|||
|117|store manager релиз 1 -> API|[Получение списка - супер-админ](https://team-fn99.testit.software/projects/1/tests/117)|||||Средний|Готов|
||||Супер-админ авторизован||||||
|||||Выполнить GET-запрос на /users/ с Bearer токеном супер-админа||Статус 200 OK  В ответе список всех пользователей с полями id, name, email, is_superadmin|||
|||||выполнить запрос в pgAdmin||сравнить ответ бд с АПИ|||
|118|store manager релиз 1 -> API|[Получение списка - обычный пользователь](https://team-fn99.testit.software/projects/1/tests/118)|||||Средний|Готов|
||||Обычный пользователь авторизован||||||
|||||Выполнить GET-запрос на /users/ с Bearer токеном обычного пользователя||200 данные только о себе|||
|115|store manager релиз 1 -> API|[Повышение - обычный пользователь пытается повысить](https://team-fn99.testit.software/projects/1/tests/115)|||||Средний|Готов|
||||Обычный пользователь авторизован||||||
|||||Выполнить PUT-запрос на /users/promote/{user_id} с Bearer токеном обычного пользователя||Статус 403 Forbidden\n2. Сообщение "Insufficient rights"|||
|116|store manager релиз 1 -> API|[Повышение - несуществующий пользователь](https://team-fn99.testit.software/projects/1/tests/116)|||||Средний|Готов|
||||Супер-админ авторизован||||||
|||||1. Выполнить PUT-запрос от супер админа на /users/promote/{fake_uuid}||Статус 404 Not Found\n2. Сообщение "User not found"|||
|114|store manager релиз 1 -> API|[Повышение - успешное](https://team-fn99.testit.software/projects/1/tests/114)|||||Средний|Готов|
||||Супер-админ выполнил login  в БД Есть обычный пользователь с ID = 47e774da-d0d0-42a7-a157-32b8d0e80033||||||
|||||Выполнить PUT-запрос на /users/promote/{47e774da-d0d0-42a7-a157-32b8d0e80033} с Bearer токеном супер-админа||Статус 200 OK  Сообщение "User successfully promoted to super admin"|||
|||||выполнить запрос в pdAdmin||В БД у пользователя is_superadmin = true|||
|119|store manager релиз 1 -> API|[Редактирование - успешное](https://team-fn99.testit.software/projects/1/tests/119)|||||Средний|Готов|
||||Супер-админ авторизован. Есть другой пользователь с ID = user_id||||||
|||||Выполнить PUT-запрос на /users/edit/{user_id} с новыми name и/или email Bearer токен супер-админа||Статус 200 OK В ответе сообщение "User successfully updated" и поля id, name, email обновленного пользователя|||
|120|store manager релиз 1 -> API|[Редактирование - несуществующий пользователь](https://team-fn99.testit.software/projects/1/tests/120)|||||Средний|Готов|
||||Супер-админ авторизован|||1. Статус 404 Not Found\n2. Сообщение "User not found"|||
|||||1. Выполнить PUT-запрос на /users/edit/{fake_uuid}||1. Статус 404 Not Found\n2. Сообщение "User not found"|||
|121|store manager релиз 1 -> API|[Редактирование - обычный пользователь](https://team-fn99.testit.software/projects/1/tests/121)|||||Средний|Готов|
||||Обычный пользователь авторизован|||1. Статус 403 Forbidden\n2. Сообщение "Insufficient rights"|||
|||||1. Выполнить PUT-запрос на /users/edit/{user_id}||1. Статус 403 Forbidden\n2. Сообщение "Insufficient rights"|||
|135|store manager релиз 1 -> API|[Редактирование самого себя - успешное](https://team-fn99.testit.software/projects/1/tests/135)|||||Средний|Готов|
||||Супер-админ авторизован.||||||
|||||Выполнить PUT-запрос на /users/edit/{user_id} с новыми name и/или email для самого себя Bearer токен супер-админа||Статус 200 OK В ответе сообщение "User successfully updated" и поля id, name, email обновленного пользователя|||
|122|store manager релиз 1 -> API|[Удаление - успешное](https://team-fn99.testit.software/projects/1/tests/122)|||||Средний|Готов|
||||Супер-админ авторизован. Есть другой пользователь с ID = user_id||||||
|||||Выполнить DELETE-запрос на /users/delete/{user_id} с Bearer токеном супер-админа||Статус 200 OK  В ответе сообщение "User successfully deleted" и email удаленного пользователя  Пользователь удален из БД|||
|123|store manager релиз 1 -> API|[Удаление - несуществующий пользователь](https://team-fn99.testit.software/projects/1/tests/123)|||||Средний|Готов|
||||Супер-админ авторизован||||||
|||||Выполнить DELETE-запрос на /users/delete/{fake_uuid}||Статус 404 Not Found Сообщение "User not found"|||
|124|store manager релиз 1 -> API|[Удаление - обычный пользователь](https://team-fn99.testit.software/projects/1/tests/124)|||||Средний|Готов|
||||Обычный пользователь авторизован||||||
|||||Выполнить DELETE-запрос на /users/delete/{user_id}||Статус 403 Forbidden Сообщение "Insufficient rights"|||
|136|store manager релиз 1 -> API|[Удаление самого себя супер админом - ошибка](https://team-fn99.testit.software/projects/1/tests/136)|||||Средний|Готов|
||||Супер-админ авторизован||||||
|||||Выполнить DELETE-запрос от супер-админа самого себя на /users/delete/{user_id} с Bearer токеном супер-админа||ошибка|||
|137|store manager релиз 1 -> API|[Авторизация - email в другом регистре](https://team-fn99.testit.software/projects/1/tests/137)|||||Средний|Готов|
||||Пользователь зарегистрирован    "email": "ivan.petrov@example.com",   "password": "password123"||||||
|||||Выполнить POST-запрос на /login/  "email": "Ivan.petrov@example.com", "password": "password123"||Статус 200 OK  В ответе access_token (JWT)\token_type = "bearer"  Время жизни токена 30 минут|||
|138|store manager релиз 1 -> API|[Регистрация - c email в другом регистре](https://team-fn99.testit.software/projects/1/tests/138)|||||Самый высокий|Готов|
||||Пользователь зарегистрирован "email": "ivan.petrov@example.com", "password": "password123"||||||
|||||1. Выполнить POST-запрос на /register/ с валидными name (3-50 символов), email, password (минимум 8 символов)  { "name": "Иван Петров", "email": "IVAN@example.com", "password": "password123" }||Ответ Статус 400.      "detail": "Email already registered"|||
|||||выполнить в pfAdmin  SELECT * FROM public.users ORDER BY id ASC||В БД отсутствует запись с переданными данными|||
|139|store manager релиз 1 -> API|[Повышение - супер админ сам себя](https://team-fn99.testit.software/projects/1/tests/139)|||||Средний|Готов|
||||супер админ пользователь авторизован   "email": "ivan@example.com",   "password": "Password123"в базе его id - 3fa5e5af-40bb-4793-9fd5-63cada0be151||||||
|||||Выполнить PUT-запрос на /users/promote/3fa5e5af-40bb-4793-9fd5-63cada0be151 с Bearer токеном супер админ||ошибка (403 например)|||
|140|store manager релиз 1 -> API|[Редактирование юзера - имя больше 50 символов](https://team-fn99.testit.software/projects/1/tests/140)|||||Высокий|Готов|
|||||Выполнить PUT-запрос на / /users/edit/{user_id}/ с name = 51 символ    "email": "ivan@example.com",   "name": "ИванПетровааааааааааааап51"||Статус 422 Validation Error\n2. Сообщение об ошибке валидации имени|||
|||||выполнить в pfAdmin  SELECT * FROM public.users ORDER BY id ASC||Пользователь не создан|||
|141|store manager релиз 1 -> API|[Редактирование юзера - email принадлежит другому](https://team-fn99.testit.software/projects/1/tests/141)|||||Высокий|Готов|
||||в базе есть юзер с  email": "IVAN@example.com||||||
|||||Выполнить PUT-запрос на / /users/edit/{user_id}/ с name = 51 символ    "email": "IVAN@example.com",   "name": "ИванПетровааааааааааааап51"||Статус 400 например что email уже есть|||
|||||выполнить в pfAdmin  SELECT * FROM public.users ORDER BY id ASC||Пользователь не изменен|||
|142|store manager релиз 1 -> API|[Редактирование юзера - email не валидный](https://team-fn99.testit.software/projects/1/tests/142)|||||Высокий|Готов|
||||в базе есть юзер с  email": "IVAN@example.com||||||
|||||Выполнить PUT-запрос на / /users/edit/{user_id}/ с name = 51 символ    "email": "IVANexample.com",   "name": "ИванПетровааааааааааааап51"||Статус 422             "msg": "value is not a valid email address",             "type": "value_error.email"|||
|||||выполнить в pfAdmin  SELECT * FROM public.users ORDER BY id ASC||Пользователь не изменен|||
|144|store manager релиз 1 -> API|[Регистрация - пароль 6 пробелов](https://team-fn99.testit.software/projects/1/tests/144)|||||Средний|Готов|
|||||1. Выполнить POST-запрос на /register/ с name = 6 пробелов "name": "123456",  "email": "will_rock666@mail.ru",  "password": "      "||Статус 422 Validation Error  Сообщение об ошибке валидации имени "msg": "ensure this value has at least 3 characters", "type": "value_error.any_str.min_length", "ctx": { "limit_value": 3|||
|||||выполнить в pfAdmin  SELECT * FROM public.users ORDER BY id ASC||Пользователь отсутствует БД|||
|145|store manager релиз 1 -> API|[Редактирование юзера - имя из пробелов](https://team-fn99.testit.software/projects/1/tests/145)|||||Высокий|Готов|
|||||Выполнить PUT-запрос на / /users/edit/{user_id}/ с name = 51 символ    "email": "ivan@example.com",   "name": "   "||Статус 422 Validation Error\n2. Сообщение об ошибке валидации имени|||
|||||выполнить в pfAdmin  SELECT * FROM public.users ORDER BY id ASC||Пользователь не создан|||
|146|store manager релиз 1 -> API|[Редактирование юзера - имя пустое](https://team-fn99.testit.software/projects/1/tests/146)|||||Высокий|Готов|
|||||Выполнить PUT-запрос на / /users/edit/{user_id}/ с name = 51 символ    "email": "ivan@example.com",   "name": ""||Статус 422 Validation Error\n2. Сообщение об ошибке валидации имени|||
|||||выполнить в pfAdmin  SELECT * FROM public.users ORDER BY id ASC||Пользователь не создан|||
|147|store manager релиз 1 -> API|[Редактирование юзера - не указан user_id](https://team-fn99.testit.software/projects/1/tests/147)|||||Высокий|Готов|
|||||Выполнить PUT-запрос на / /users/edit/{user_id}/  user_id - не указывать    "email": "ivan@example.com",   "name": "ИванПетровааааааааааааап51"||Ошибка 400 об отсутствии user_id|||
|||||выполнить в pfAdmin  SELECT * FROM public.users ORDER BY id ASC||Пользователь не создан|||
||||||||||
