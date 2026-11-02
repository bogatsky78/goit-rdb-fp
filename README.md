# goit-rdb-fp

Фінальний проєкт курсу «Relational Databases for Data Science»: статистика інфекційних захворювань за країнами й роками в PostgreSQL 16.

Усі запити й результати в HW_FP.ipynb

1. Схема `pandemic`, `SET search_path`, імпорт `data/infectious_cases.csv` через `COPY` у таблицю `infectious_cases`.
2. Нормалізація до 3НФ: `entities` (унікальні пари Entity/Code) і `infectious_cases_norm` (показники з `entity_id`).
3. AVG, MIN, MAX і SUM для `Number_rabies` по кожній сутності, топ-10 за середнім.
4. Дата 1 січня з `Year`, поточна дата і різниця в роках вбудованими функціями.
5. Функції `fn_years_since(year)` і `fn_avg_cases_per_period(cases, divisor)` та запити з ними (дільники 12, 4, 2).

## Скриншоти

У теці `screenshots/` — скриншоти створених таблиць `entities`, `infectious_cases` і `infectious_cases_norm`. Результати всіх запитів можна переглянути в ноутбуці HW_FP.ipynb.
