Demo link  [Demo link](https://leonid1313.github.io/Product_card/).

1. Создать проект на ReactJS + Webpack. Можно `create-react-app`
2. В проекте сверстать страницу Cards и Модальное окно: [https://www.figma.com/file/yPQsftMIwgUJmGad6jc0MV/Test?node-id=0%3A1](https://www.figma.com/file/yPQsftMIwgUJmGad6jc0MV/Test?node-id=0%3A1)
    - Обязательно разбить страницу на компоненты, в остальном архитектура проекта на ваше усмотрение
    - Визуально верстка должна быть приближена к дизайну, но pixel perfect не нужен.
    - Нужна верстка для мобильных, ее нужно сделать без макета, дизайн на ваше усмотрение
    - Состояния для элементов (hover, error) нужно взять из блока States (есть на дизайне), если каких состояний не хватает - сделайте их на свое усмотрение.
3. Получить список карточек с сервера: [https://run.mocky.io/v3/b7d36eea-0b3f-414a-ba44-711b5f5e528e](https://www.notion.so/b7d36eea0b3f414aba44711b5f5e528e) и вывести эти данные в верстку
4. При клике на кнопку buy на карточке должно открываться модальное окно покупки товара. Есть на макете.
5. При клике на **Buy cheapest** нужно открывать модальное окно покупки самого дешевого товара. 
6. Поля в модальном окне должны валидироваться. Для валидации нельзя использовать готовые библиотеки. Как работает валидация:
    - Валидация должна срабатывать в двух случаях:
        - Когда юзер ввел невалидные данные и убрал фокус с поля, мы показываем невалидное состояние для этого поля.
        - Когда юзер не заполнил обязательные поля и нажал кнопку Submit, мы показываем невалидное состояние для всех пустых обязательных полей и для всех полей которые заполнены некорректно
    - Когда юзер начал заполнять данные в невалидном поле - невалидный стейт нужно убрать
    - Правила валидации:
        - Поле **Name**
            - Считается невалидным, если осталось незаполненным. Текст ошибки: "This field in required"
            - Должно содержать только буквы. Текст ошибки: "Only letters allowed"
        - Поля **Phone number**
            - Считается невалидным, если остались незаполненным. Текст ошибки: "This field in required"
            - Должно содержать только цифры. Текст ошибки: "Only numbers allowed"
            - Должно содержать 12 символов. Текст ошибки: "Should contain 12 characters"
    - Если все поля корректно заполнены, после нажатия на Submit данные формы должны выводиться в консоль
7. И верстка и JS должны корректно работать в последних версиях Chrome, Firefox и Edge.
8. Выполненое задание нужно залить на github или bitbucket и предоставить ссылку
