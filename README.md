# **Clean Architecture (а-ля Модульный подход)**

## **Предисловие**

Это руководство было написано в стиле *"своими словами"* и пытается более менее понятным языком описать концепцию и идеалы, к которому мы стремимся.

Если у вас появилась идея дополнить, отредактировать руководство, то согласуйте это с её автором или командой разработчиков.

## **Проблема**

Работая над продуктом меняются поколения разработчиков, каждый из которых вносит свой вклад в развитие и расширение кодовой базы. Спустя N-время кодовая база превращается в изобилие разных подходов (словно главных улиц города, где между историческими зданиями располагаются стеклянные бизнес-центры) разработчика при реализации какой-то задачи, что со временем работа с такой хуйнёй приводит к:

- Новому сотруднику (да и старым) тяжело быстро вкатиться и ознакомиться с проектом или конкретным разделом кодовой базы;
- Кодовая база приводит к увеличению затрат человекочасов на выполнение задачи;
- Хуёвая кодовая база повышает шансы, что где-то много взаимосвязанного кода, который незнающий разработчик может изменить и сломать то, о чём он даже не догадывался;
- Код тяжело расширять за счёт костылей и других зависимостей;
- Частичная зависимость кода от автора, который его написал.

## **Мотивация**

Чтобы решить проблемы, описанные выше, мир придумал паттерны проектирования, которые избавляют от большинства проблем. Вдаваться в проблемы того или иного паттерна, мы, конечно же, не будем.

Собственно, принято соглашение использовать "Чистую архитектуру" (она же а-ля "Модульный подход"). В кратце о возможностях, которые предлагает подход в качестве награды:

- Независимая от UI бизнес-логика;
- Отзывчивость при написании тестов или эмуляции сервера (моки);
- Огранизованный\Структурированный\Читабельный код;
- и так далее...

## Полезные ссылки

- [Moving away from ReactJs and VueJs on front-end using Clean Architecture](https://dev.to/xurxodev/moving-away-from-reactjs-and-vuejs-on-front-end-using-clean-architecture-3olk)
- [Заблуждения Clean Architecture](https://habr.com/ru/companies/mobileup/articles/335382/)