# Задача 
Определить токсичность комментариев

**Цель:** найти инструмент, который будет искать токсичные комментарии и отправлять их на модерацию - найти модель классификации комментариев на позитивные и негативные со значением метрики качества F1 >= 0.75

# Вывод
Наилучшей моделью стала LogisticRegression, которая на тестировании показала F1 = 0.76 (среднее гармоническое точности и полноты), то есть LogisticRegression с вероятностью 76% правильно определит, токсичен комментарий или нет

# Стек технологий
BERT, Pandas, Python, nltk, tf-idf

# Статус проекта
Завершен
