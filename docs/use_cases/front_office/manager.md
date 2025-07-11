# Use-кейсы для менеджера по продажам



## Поиск и инициирование контакта с новым юрлицом

### Сценарий
Менеджер получает информацию о потенциальном клиенте (например, из базы лидов, рекомендации, отраслевого мероприятия).

### Действия
1. Создает карточку юридического лица (ИНН, отрасль, размер).
2. Добавляет ключевые контакты (ЛПР, КЦО) с ролями.
3. Проверяет данные через интеграцию с СПАРК/Контур.Фокус (автозаполнение реквизитов).
4. Фиксирует источник лида.
5. Заводит сделку, назначает этап воронки (например, "Первичный контакт").
6. Планирует первое касание (звонок/email/встреча) через календарь CRM.

### Цель
Упорядочить старт работы с клиентом, избежать дублей.



## Обработка входящей заявки на страхование

### Сценарий
Клиент присылает запрос через сайт/email/телефон.

### Действия
1. Находит или создает карточку юрлица.
2. Фиксирует запрос (объект страхования, риски, сроки).
3. Создает задачу на подготовку КП с дедлайном.
4. Заводит сделку на этапе "Анализ потребностей".
5. Использует шаблон письма для подтверждения получения заявки.

### Цель
Не упустить клиента, зафиксировать требования.



## Подготовка и согласование КП

### Сценарий
Менеджер формирует коммерческое предложение после уточнения деталей.

### Действия
1. Открывает карточку сделки → нажимает "Создать КП".
2. Выбирает продукт из справочника (страхование имущества, ОСАГО для юрлиц и т.д.).
3. Заполняет параметры риска (объект, сумма, франшиза).
4. Запускает предварительный расчет через интеграцию с андеррайтингом.
5. Отправляет КП на согласование (автоматический workflow):
    - Андеррайтер: проверка тарифа,
    - Юрист: проверка условий,
    - Руководитель: утверждение скидки.
6. Отслеживает статус согласования в реальном времени.
7. Отправляет клиенту финальное КП (PDF) прямо из CRM.

### Цель
Ускорить подготовку КП, исключить ошибки, контролировать сроки.



## Проведение переговоров и фиксация возражений

### Сценарий
Клиент созванивается с менеджером, чтобы обсудить условия КП.

### Действия
1. Перед звонком: смотрит историю взаимодействий и КП в карточке клиента.
2. Звонит через интеграцию с IP-телефонией (клик-ту-колл).
3. Фиксирует запись разговора (автоматически прикрепляется к сделке).
4. Записывает возражения в карточку контакта (например, "Цена выше рынка").
5. Использует базу знаний CRM для поиска ответов на возражения.
6. При необходимости обращается к продуктологу за примерами успешных продаж или эффективных ответов на возражения.
7. Обновляет этап сделки (например, "Устранение возражений").
8. Ставит задачу себе или андеррайтеру на доработку КП.

### Цель
Повысить конверсию, систематизировать работу с возражениями.



## Закрытие сделки и оформление договора

### Сценарий
Клиент согласен подписать договор на предложенных условиях.

### Действия
1. Переводит сделку в этап "Договор оформляется".
2. Нажимает "Создать договор" → данные из КП автоматически переносятся.
3. Отправляет договор на финальные проверки (юрист, андеррайтер).
4. Отслеживает электронную подпись через интеграцию с ЭДО.
5. После подписания:
    - Статус сделки → "Выиграна",
    - Данные автоматически передаются в бэк-офис (Policy Admin System) для выпуска полиса,
    - Фиксируется дата начала действия полиса.
6. CRM автоматически создает задачу на "Продление" за 45 дней до окончания срока.

### Цель
Обеспечить безошибочное оформление, запустить постпродажное обслуживание.



## Работа с текущими клиентами (продление/док продажи)

### Сценарий
За N-дней до окончания полиса CRM напоминает о продлении.

### Действия
1. Видит задачу "Продление договора" в своем календаре.
2. Открывает карточку клиента → смотрит историю договоров, КП, возражений.
3. Анализирует актуальные риски клиента (изменился ли бизнес?).
4. Готовит новое КП (через копирование прошлого + корректировки).
5. Предлагает дополнительные продукты (например, если раньше страховали только имущество, добавляет ответственность).
6. Фиксирует результат переговоров (продан, ушел к конкуренту, на паузе).

### Цель
Удержать клиента, увеличить LTV (пожизненную ценность).



## Работа с потерянными сделками

### Сценарий
Клиент отказался от сотрудничества или выбрал конкурента.

### Действия
1. Переводит сделку в этап "Проиграна".
2. Обязательно указывает причину из справочника (например, "Выбрали конкурента X", "Отложили на год").
3. Добавляет комментарий с деталями (какие условия предложил конкурент?).
4. Ставит напоминание о повторном контакте (через 3/6/12 месяцев).
5. Отмечает контакт как "холодный" (но сохраняет в базе).

### Цель
Собрать аналитику для улучшения продукта/процессов, сохранить потенциал на будущее.