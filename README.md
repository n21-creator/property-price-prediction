## «Модель прогнозирования стоимости жилья для агентства недвижимости»

### Цели и задачи проекта
Разработать модель машинного обучения, которая поможет обрабатывать объявления и позволит предсказывать стоимость объектов недвижимоси по характеристикам.

# Краткая информация о данных:

        ● 'status' — статус продажи;
        ● 'private pool' и 'PrivatePool' — наличие собственного бассейна;
        ● 'propertyType' — тип объекта недвижимости;
        ● 'street' — адрес объекта;
        ● 'baths' — количество ванных комнат;
        ● 'homeFacts' — сведения об объекте (год постройки,год реконструкции, наличие системы отопления и кондиционирования,паркинга,цена за квадратный фут,площадь участка);
        ● 'fireplace' — наличие камина;
        ● 'city' — город;
        ● 'schools' — сведения о школах в районе(рейтинг,название учебного заведения,расстояние до учебного заведения);
        ● 'sqft' — площадь в футах;
        ● 'zipcode' — почтовый индекс;
        ● 'beds' — количество спален;
        ● 'state' — штат;
        ● 'stories' — количество этажей;
        ● 'mls-id' и 'MlsId' — идентификатор MLS (Multiple Listing Service,Id агента по продаже недвижимости );
        ● 'target' — цена объекта недвижимости

Этапы работы над проектом:

# EDA

* Отчистка датасета от дубликатов,пропущенных значений, неинформативных признаков.
  
* Анализ данных с помощью средств визуализации(pyplot,seaborn).



# Создание и обучение модели:

* Обработака и отнормирование признаков

 
* Построена модель LinearRegression


* Построена модель RandomForestRegressor


* Построена модель с L1 и L2 регуляризаций ElasticNetCV


* Построена модель градиентного бустинга CatBoostRegressor с RandomizedSearchCV


* Построена модель градиентного бустинга CatBoostRegressor Optuna

* Анализ важности признаков

* Сравнительная таблица метрик всех моделей



# Постановка экспериментов на воспроизводимость модели
-ошибка при создании функции-->изменение функции(доработка,09.04.24)
