Из «Бета-Банка» стали уходить клиенты. Каждый месяц. Немного, но заметно. Банковские маркетологи посчитали: сохранять текущих клиентов дешевле, чем привлекать новых.

Нужно спрогнозировать, уйдёт клиент из банка в ближайшее время или нет. Вам предоставлены исторические данные о поведении клиентов и расторжении договоров с банком.

Постройте модель с предельно большим значением F1-меры. Чтобы сдать проект успешно, нужно довести метрику до 0.59. Проверьте F1-меру на тестовой выборке самостоятельно.

Дополнительно измеряйте AUC-ROC, сравнивайте её значение с F1-мерой.

Источник данных: https://www.kaggle.com/barelydedicated/bank-customer-churn-modeling

**Введение:

По имеющимся данным заказчик просит спрогнозировать, уйдет ли клиент в ближайшее время.

**Цель:

Подготовить модель, имеющую F1 меру не менее 0,59


Было перебрано по меньшей мере около 4100 моделей типа логистическая регрессия, решающее дерево и случайный лес. В результате получилось достичь значения F1 меры 0.597051597051597 
при модели RandomForestClassifier(class_weight='balanced', max_depth=13, n_estimators=20, random_state=12345) с 9-и кратно увеличенной выборкой по редким классам.

Значение F1-меры для best_model на тестовой выборке показывает ~0,64