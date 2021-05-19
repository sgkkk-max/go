# Структура проекта
index.js - Входная точка проекта 

routes.js - Роутинг,все роты приватные, выкидывают на логин, если нет токена

Папка src/api - содержит запросы для работы с сервером

Папка src/assests - Иконки, картинки 

Папка src/components -  Содержит компоненты, например кастомные кнопки и т.д

Папка src/constants -  константы проекта

Папка src/helpers - вспомогательные функции, которые используются на проекте

Папка src/pages - страницы проекта, могут содержать в себе компоненты, необходимые для страницы

Папка src/scss - Общие стили проекта

Папка src/store - Работа с тором проекта, используется redux + redux-saga, redux-saga используется для работы с api.

На проекте используется библиотека styled-components, предназначена для работы со стилями. 

# Как запустить наш проект

Наш проект доступен по адресу [http://go.alras63.ru/](http://go.alras63.ru/)

## Доступные команды

В папке с проектом, вы можете запустить проект локально (у себя на компьютере)

### `yarn start`

Запускает приложение в режиме отладки.\
Откройте [http://localhost:3000](http://localhost:3000) для просмотра проекта в браузере

### `yarn build`

Собирает билд проекта в папку build


## Реализованные подсказки
### 1. Лучший ход
Данный сценарий выдаст вам оптимальный ход, исходя из ситуации на доске. Данная
подсказка предназначена, скорее, для профессионалов, которые в сложной ситуации не знают как
лучше сходить. Начинающие игроки будут использовать этот алгоритм бездумно.
### 2. Лучший ход соперника
Показывает лучший ход, который может совершить противник. Подсказка однозначно для
профессиональных игроков в Го, начинающие не поймут, как правильно производить
контратаку, опираясь на лучший ход соперника
### 3. Развитие игры на 2 хода вперед
В настоящий момент времени рассчитывает и показывает 2 лучших хода подряд.
Пригодится начиняющим игрокам
### 4. Плохой ход соперника
Показывает вариант плохого хода соперника. Универсальная подсказка, пригодится всем,
кто умеет анализировать и на основе плохого хода соперника делать свой, лучший
### 5. Тепловая карта всей доски. Детализированная
Показывает области, подконтрольные «дыханиям» камней с разной силой – когда до
камня 1 клетка, на тепловой карте отображается большой круг, по мере удаления от камня
размер круга тепловой карты уменьшается. Детализированность тепловой карты
максимальная, т.е. показывает удаленные максимально пересечения. Пригодится только
профессиональным игрокам в Го

### 6. Тепловая карта всей доски. Менее детализированная
Повторяет функционал детализированной тепловой карты с меньшей степенью
детализации
### 7. В какой четверти доски будет лучший ход соперника?
Показывает, где соперник может сделать лучший ход. Подсказка универсальная, для всех.
Помогает выбрать четверть доски для активной игры.
### 8. В какой половине доски будет лучший ход соперника?
Тоже самое, для половины доски
### 9. Показать лучший из заданных 2 ходов соперника
Задаем два хода, и система показывает нам, как соперник может сходить, чтобы нам было
очень больно. Пригодится профессиональным игрокам.
### 10. В какой четверти доски сейчас лучший ход?
Алгоритм выбирает наиболее перспективную 1⁄4 часть доски и предлагает ход.
Универсальная.
### 11. В какой половине доски сейчас лучший ход?
Алгоритм выбирает наиболее перспективную 1/2 часть доски и предлагает ход.
Универсальная
### 12. Тепловая карта 1-й четверти доски
Строит тепловую карту только для первой четверти доски. Подсказка для профессионалов.
### 13. Тепловая карта 1-й и 2-й четвертей доски
Строит тепловую карту для первой и второй четверти доски. Подсказка для
профессионалов.
### 14. Какой перевес в очках на данный момент?
ИИ рассчитывает очки каждого игрока и выводит перевес
### 15. Кто побеждает на данный момент?
ИИ считает статистику партии на данный момент и выводит текущего победителя

## Кроме того, мы реализовали следующие сценарии из подсказок:
1. Захват начальной территории
2. Атака по двум четвертям
3. Защита
4. Продолжать играть?

## Стек используемых технологий для реализации frontend-решения хакатона "Игры разумов"

+ Javascript
+ React.js
+ HTML, CSS
+ Styled components
+ Saas
+ Redux

## Описание улучшений по сравнению с изначальной версией

+ Исправлены неработающие блоки, кнопки
+ Добавлен функционал предложения воспользоваться тем или иным сценарием в ходе игры
+ Реализована обработка неправильных ходов пользователя (самоубийственный, ко-борьба)
+ Исправлены размеры шрифтов
+ Добавлена обработка 500-ых ошибок сервера
+ Починили поиск в рейтинге игроков

## Состав команды и роли

+ Рассохин Алексей Александрович - дизайн, верстка, написание текстов, немного react.js
+ Блынский Арсений Валерьевич - верстка, написание текстов, генерирование креатива
+ Евдокимов Сергей Эдуардович - программирование на стороне клиента, react.js, бек-фулстек
+ Любченко Елена Александровна - наставник, сопровождающий