# Тестовое. Фронт-енд разработчик. JavaScript #
## Описание для ревьюера ##
**Студенту было дано задание реализовать интерфейс с Fetch API, пользуясь ООП.
     У пользователя должна быть возможность**
     
* Ввести необходимые данные в форму.
* Исходя из данных, введенных в форму - получить свой рейтинг.
* Возможность проводить данную операцию несколько раз.
* Воспользоваться моковым поиском по имени для просмотра рейтинга других пользователей.

*Необходимо прокомментировать JS-код. Частные комментарии можно оставлять в соответствующих файлах. Общие комментарии оставьте внизу файла script.js*

## При проверке задайте себе вопросы  ##

* Корректно ли реализован Fetch, должным ли образом обрабатываются собираемые и получаемые данные?
* Имеет ли код уязвимости, если да - то какие?
* Корректно ли работает реализованный функционал? Соответствует ли он поставленной перед студентом задаче?
* Насколько хорошо организован и чист код: как его можно улучшить, изменить, упростить?
* Корректно ли используются моковые данные, все ли ок с названием переменных, их расположением в коде/файлах?
* Как обстоят дела с методами внутри классов? Возможно ли что-то упростить или реорганизовать?

## Коментарии от код-ревьюера ##

- APIKey, city сделать параметрами к функции isSunny, сейчас всегда захардкожен. Cмайлики в коде вынести в костанты чтобы легче читать 
```sh
if (happiness === 4) {
  Man._iconElement.innerHTML = HAPPY;
}
```

- Добавить валидацию поставить на то что юзер сразу нажмет на кнопку подсчета

- Создать отдельный компонент на мултипл чойс который несколько раз повторяется
```sh
<h2 class="column__heading">
    {{question}}
</h2>
<label class="column__label">
    <input type="radio" value="yes" name="{{name}}">
    <span>Да</span>
</label>
<label class="column__label">
    <input type="radio" value="no" name="{{name}}">
    <span>Нет</span>
</label>
```