# Появление элементов при прокрутке

Домашнее задание к занятию 2.1 «DOM».

## Описание 

Необходимо реализовать механизм появления блоков в тот момент, когда прокрутка 
дойдёт до них

![Demo](./demo.gif)

### Исходные данные

1. Основная HTML-разметка
2. Базовая CSS-разметка

Разметка элементов выглядит следующим образом:

```html
<div class="reveal">
    <!-- содержимое блока -->
</div>
```

Отображение блока осуществляется путём присовения класса *reveal_active*:

```html
<div class="reveal reveal_active">
    <!-- содержимое блока -->
</div>
```

### Процесс реализации

1. Отслеживайте изменение прокрутки окна
2. При изменении прокрутки, получите информацию о конкретном положении элемента
с классом *reveal*.
3. При нахождении элемента в поле зрения, присвойте этому элементу класс *reveal_active*

## Подсказки (спойлеры)

<details>
<summary>Используемые темы</summary>

1. Событие *scroll*
2. Метод *getBoundingClientRect*

</details>

<details>
<summary>Советы</summary>

Обратите внимание, что при прокрутке возвращаемые координаты
*getBoundingClientRect()* меняются

</details>

## Решение задач
1. Перейти в папку задания. `cd ./dom/reveal`.
2. Открыть файл `task.js` в вашем редакторе кода и выполнить задание.
3. Открыть файл `task.html` в вашем браузере и убедиться в правильности выводимых результатов.
4. Добавить файл `task.js` в индекс git с помощью команды `git add %file-path%`, где %file-path% - путь до целевого файла. `git add task.js`.
5. Сделать коммит используя команду `git commit -m '%comment%'`, где %comment% - это произвольный комментарий к вашему коммиту. `git commit -m 'first commit reveal'`.
6. Опубликовать код в репозиторий homeworks с помощью команды `git push -u origin master`.
7. Прислать ссылку на репозиторий через личный кабинет на сайте [Нетологии][6].

[0]: https://github.com/
[1]: https://www.sublimetext.com/
[2]: https://code.visualstudio.com/
[3]: https://github.com/netology-code/guides/tree/master/github
[4]: https://git-scm.com/
[5]: https://github.com/netology-code/guides/blob/master/git/REAMDE.md
[6]: https://netology.ru/

*Никаких файлов прикреплять не нужно.*

Все задачи обязательны к выполнению для получения зачета. Присылать на проверку можно каждую задачу по отдельности или все задачи вместе. Во время проверки по частям ваша домашняя работа будет со статусом "На доработке".

Любые вопросы по решению задач задавайте в Slack-канале.
