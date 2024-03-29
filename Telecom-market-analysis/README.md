# Прогноз оттока киентов

## Описание проекта
Оператор связи «Ниединогоразрыва.ком» хочет научиться прогнозировать отток клиентов. Если выяснится, что пользователь планирует уйти, ему будут предложены промокоды и специальные условия. Команда оператора собрала персональные данные о некоторых клиентах, информацию об их тарифах и договорах.

## Описание данных
Данные состоят из файлов, полученных из разных источников:

contract.csv — информация о договоре;

**Характеристики таблицы ** 

`customerID`- Код клиента          
`begin_date`- Дата начала договора         
`end_date` - Дата окончания договора         
`type` - Тип оплаты (месячная, годовая)             
`paperless_billing`-Безбумажное выставление счетов   
`payment_method`- Метод оплаты      
`monthly_charges`- Ежемесячные платежи    
`total_charges` - Всего начислений    

personal.csv — персональные данные клиента;

**Характеристики таблицы ** 

`customerID`     - Код клиента    
`gender`         - Пол (муж, жен)     
`senior_citizen` - Пенсионер    
`partner`        - Партнер       
`dependents`     - Иждивенцы  

internet.csv — информация об интернет-услугах;

**Характеристики таблицы ** 

`customerID`       - Код клиента    
`internet_service` - Интернет-сервис  
`online_security`  - Блокировка небезопасных сайтов  
`online_backup`    - Облачное хранилище файлов для резервного копирования данных  
`device_protection`- Антивирус   
`tech_support`     - Выделенная линия технической поддержки  
`streaming_t_v`    - Стриминговое телевидение  
`streaming_movies` - Каталог фильмов  

phone.csv — информация об услугах телефонии.

**Характеристики таблицы ** 

`customerID`       - Код клиента    
`multiple_lines` - Несколько линий  

## Вывод

Обучили 4 модели LogisticRegression, DecisionTreeClassifier, RandomForestClassifier и CatBoostClassifier
Лучший результат показала модель CatBoostClassifier со значением метрики ROC-AUC в 0.92



