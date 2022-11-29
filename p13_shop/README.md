# Проект для «Викишоп»

**Дано:** интернет-магазин «Викишоп» запускает новый сервис. Теперь пользователи могут редактировать и дополнять описания товаров, как в вики-сообществах. То есть клиенты предлагают свои правки и комментируют изменения других

**Задача:** найти инструмент, который будет искать токсичные комментарии и отправлять их на модерацию - найти модель классификации комментариев на позитивные и негативные со значением метрики качества F1 >= 0.75

# Вывод:
В проекте:
1. загрузила данные и провела их предобработку - удаление лишних данных, очистку текстов, лемматизацию 
2. обучила 4 модели с разными гиперпараметрами и выборками и проверила их на тестовой выборке
3. выбрала лучшую модель по показателю F1

Аутсайдером среди моделей стали RandomForestClassifier и DecisionTreeClassifier, так как дали наименьшее F1. 

Наилучшей моделью стала LogisticRegression, которая на тестировании показала F1 = 0.76. Поскольку требовалось найти модель классификации комментариев на позитивные и негативные со значением метрики качества F1 >= 0.75, рекомендовать могу LogisticRegression