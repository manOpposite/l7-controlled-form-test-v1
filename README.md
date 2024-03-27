## Правила и регламент

- [Экзамен: правила, рекомендации и порядок проведения](https://hexly.notion.site/d9289c18871c44508bc7c7f05a51d94f)

## Запуск и сборка приложения

Для запуска фронтенда приложения используйте команду:
<<<<<<< HEAD
=======

>>>>>>> 02f9cff (delete branch)
```bash
make run
```

Для запуска сервера используйте в отдельном терминале команду:
<<<<<<< HEAD
=======

>>>>>>> 02f9cff (delete branch)
```bash
make start-server
```

## Задание

Дана готовая разметка. Ваша задача написать функции для валидации предоставленной формы и функцию, отвечающую за работу всего приложения в файле **src/application.js**.

## Задача 1

<<<<<<< HEAD
Напишите и экспортируйте функцию `validateName()`, которая валидирует строку с условием, что валидным именем считается любая строка с длиной больше 0, исключая пробелы. Если имя валидно, то функция возвращает пустой объект, иначе возвращается объект с ключом errors, который содержит массив со строкой 'введите имя'.

```javascript
validateName('example'); // []
validateName(''); // ['name cannot be empty']
validateName('    '); // ['name cannot be empty']
=======
Напишите и экспортируйте по умолчанию функцию `app()`, отвечающую за работу веб-приложения.
При старте приложения должна рендериться форма внутри родительского элемента с классом `.form-container`.
Форма выглядит следующим образом. Для скорости работы, вы можете добавить ее через `innerHTML`.

```html
    <form id="registrationForm">
      <div class="form-group">
        <label for="inputName">Name</label>
        <input type="text" class="form-control" id="inputName" placeholder="Введите ваше имя" name="name" required>
      </div>
      <div class="form-group">
        <label for="inputEmail">Email</label>
        <input type="text" class="form-control" id="inputEmail" placeholder="Введите email" name="email" required>
      </div>
      <input type="submit" value="Submit" class="btn btn-primary" disabled>
    </form>
>>>>>>> 02f9cff (delete branch)
```

## Задача 2

<<<<<<< HEAD
Напишите и экспортируйте функцию `validateEmail()`, которая валидирует email, с условием, что валидной почтой считается любая строка с символом `@` посередине, с любой длиной символов, исключая пробелы до и после нее. Если почта валидна, то функция возвращает пустой объект, иначе возвращается объект с ключом errors, который содержит массив со строкой 'введите валидный email'.

```javascript
validateEmail('example@gmail.com'); // []
validateEmail('@gmail.com'); // ['invalid email']
validateEmail('g@ и'); // ['invalid email']
validateEmail('g@s'); // []
```

## Задача 3

Напишите и экспортируйте функцию `app()`, которая будет ответственна за запуск и работу приложения.

Форма, данная в файле **index.html**, имеет кнопку `submit` c текстом `'зарегистрироваться'`. Ваша задача состоит в том, чтобы реализовать для этой кнопки статус `disabled`, когда хотя бы одно из полей невалидно. Иначе кнопка не должна иметь атрибут `disabled`.

## Задача 4

Внутри функции `app()` напишите код, который реализует контролируемый input для каждого поля формы. Инпут должны иметь класс `is-valid`, если его содержимое валидно. Иначе input должен иметь класс `is-invalid`.

## Задача 5

При нажатии кнопки `зарегистрироваться` должен отправляться запрос на сервер с данными формы и в случае успешного ответа содержимое `document.body` нужно заменить на текст ответа сервера, завернутый в теги `<p></p>` таким образом:
=======
Форма, данная в файле **index.html**, имеет кнопку `submit` c текстом `'зарегистрироваться'`. Ваша задача состоит в том, чтобы реализовать для этой кнопки статус `disabled`, когда хотя бы одно из полей невалидно. Иначе кнопка не должна иметь атрибут `disabled`.

## Задача 3

Внутри функции `app()` напишите код, который реализует контролируемый input для каждого поля формы. Инпут должны иметь класс `is-valid`, если его содержимое валидно. Иначе input должен иметь класс `is-invalid`.

## Задача 4

При нажатии кнопки `зарегистрироваться` должен отправляться запрос на сервер с данными формы и в случае успешного ответа содержимое `document.body` нужно заменить на текст ответа сервера, завернутый в теги `<p></p>` таким образом:

>>>>>>> 02f9cff (delete branch)
```html
 `<p>Ответ сервера</p>`.
```
