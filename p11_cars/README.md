# Определение стоимости автомобилей

**Дано:**  
Сервис по продаже автомобилей с пробегом «Не бит, не крашен» разрабатывает приложение, чтобы привлечь новых клиентов. В нём можно будет узнать рыночную стоимость своего автомобиля. Необходимо построить модель, которая умеет её определять. Есть данные о технических характеристиках, комплектации и ценах других автомобилей.

Критерии, которые важны:
- качество предсказания;
- время обучения модели;
- время предсказания модели.

**Условия:** 
1. Не ограничиваться градиентным бустингом
2. Для оценки качества моделей применять метрику RMSE. RMSE должно быть меньше 2500.
3. Освоить библиотеку LightGBM и её средствами построить модели градиентного бустинга.
4. Ввести время выполнения ячейки кода
5. В модели градиентного бустинга можно изменять только два-три параметра. 

# Вывод
В проекте:
- загрузила  данные и провела их предобработку - очистку, заполнение, удаление лишних данных
- сравнила 3 модели с разными гиперпараметрами и выборками
- выбрала лучшую модель по 3 показателям - RMSE, время обучения и время предскзания - и проверила ее на тестовой выборке

Итог - наилучшей моделью стала LGBMRegressor с OHE, которая на финальном тестировании показала RMSE 1302, несмотря на требуемое бОльшее время на обучение и предсказание. То есть если есть время, то лучше пользоваться данной моделью