# test_web_qa 

Тест-план

1. Введение
Цель документа: Тестирование страницы сайта https://wortex.by/catalog#shurupoverty
Обзор проекта: Данная страница позволяет просматривать каталог продукции, переходить на личную страницу продукта, просматривать характеристики каждого продукта, скачивать данный каталог. Сайт должен работать как на десктопе, так и на мобильном устройстве.
2. Объем тестирования
Включенные области:
Просмотр каталога товаров.
Поиск товаров.
Просмотр характеристик товаров
Скачивание каталога товаров
3. Методология и типы тестирования
Функциональное тестирование:
Проверка всех ключевых функций системы, чтобы убедиться, что они работают согласно требованиям.
UI/UX тестирование:
Оценка удобства использования интерфейса и соответствия дизайна макетам.
4. Проверка каждой отдельной области
Просмотр каталога товаров


Вся доступная продукция присутствует на странице
У каждого товара присутствуют: названия(До раздела Аккумуляторы и зарядные устройства(Аккум.+ название товара(с маленькой буквы))), характеристики, картинка товара
У каждого раздела присутствуют: название и картинка раздела

Поиск товара
При вводе короткого названия категории в поле поиска должна отображаться страница с всеми товарами из разных категорий в котором присутствует данное название
Пример: при вводе “шлифмашина” должны отображаться все товары из категорий “Углошлифмашины” и “Ленточные шлифмашины”
При вводе конкретного товара должен отображаться данный товар
При любом из данных поисков должна присутствовать строка в начале страницы “Результаты поиска” + строка вводимая в поисковую строку
Пример:

Просмотр характеристик товаров 
При нажатии на название товара отображенного в каталоге должна открываться страница со всеми характеристиками данного товара
На данной странице должны присутствовать: Технические данные, Описание товара, Основные преимущества и Комплектация товара
Также должен присутствовать слайдер картинок, который показывает продукт с разных сторон
И должна присутствовать кнопка следующий/предыдущий, при нажатии на который происходит переключение между товарами в категории без возврата на страницу каталога

Скачивание каталога товаров
При нажатии на кнопку скачать каталог товаров должно происходить скачивание документа содержащего весь каталог товара представленный на странице


Чек-лист

Просмотр каталога товаров
Отображение списка товаров в категории.
Отображение карточки товара с корректной информацией (название, цена, изображение, описание).
Отображение картинок в начале каждой категории
Поиск товара
Ввод категории -> Все товары из категории видны
Ввод названия товара -> Товар найден
Просмотр характеристик товаров 
Отображение страницы товара
Отображение всей необходимой информации о данном товаре на странице
Присутствие и работа кнопок следующий/предыдущий
Скачивание каталога товаров
Нажатие на кнопку скачать каталог -> каталог скачивается


Баг-репорт

ID: 1
Название: Ошибка отображения картинок продуктов
Описание:
Не отображаются картинки разделов и картинки продуктов
Шаги для воспроизведения:
Открыть страницу каталога
Ожидаемый результат:
При каждом разделе в каталоге стоит картинка раздела и каждая карточка продукта содержит картинку продукта
Фактический результат:
Картинки отсутствуют
Приоритет: Низкий
Серьезность: Низкая

ID: 2
Название: Ошибка поиска товара
Описание:
При попытке найти определенный товар находящийся в каталоге продукт не отображается
Шаги для воспроизведения:
Открыть каталог
Ввести в поисковую строку “Аккум. дрель-шуруповерт BD 2030-1 DLi”
Нажать на кнопку поиска
Ожидаемый результат:
Карточка товара должна отобразиться
Фактический результат:
Товар не отображается.
Приоритет: Высокий
Серьезность: Средняя

ID: 3
Название: Ошибка скачивания товара
Описание:
При попытке скачать каталог товаров происходит перенаправление на такую же страницу, но скачивание не происходит
Шаги для воспроизведения:
Открыть каталог
Нажать на кнопку “скачать каталог”
Ожидаемый результат:
Каталог должен скачаться
Фактический результат:
Переход на новую страницу
Приоритет: Высокий
Серьезность: Средняя


