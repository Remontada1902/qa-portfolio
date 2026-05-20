# QA Portfolio — Евгений Прокашев

## Тестирование StoreSystem (https://github.com/meshkovQA/StoreSystem) (релиз 1)

Микросервис управления пользователями (FastAPI + PostgreSQL + Docker).

### Что внутри

| Артефакт | Описание |
|----------|----------|
- [Тест-кейсы](./test_cases_relise_1.xlsx) | 46 тест-кейсов (UI + API) в TestIT |
- [Баг-репорты](./bug_reports_relise_1.xlsx) | 19 багов, 14 исправлено, 5 открыто |
- [Postman коллекция](./StoreSystem_API.postman_collection.json) | API-тесты с авто-проверками |

### Итог по релизу

- Найдены критические баги:
  - валидация кириллицы не работает (регистрация и редактирование)
  - авторизация с email в другом регистре не работает
  - редактирование с чужим email → 500 ошибка
- Регресс подтвердил исправление 14 багов

**Инструменты:** TestIT, Postman, Docker, Git, pgAdmin, Kibana
