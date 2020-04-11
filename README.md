# Коллоквиум по дискретной математике

Это лишь экспериментальная версия оболочки. В ней запросто могут найтись ошибки и недоработки. Обо всех проблемах, пожалуйста, сообщайте лично или через "Issues" на GitHub.

### Как добавить свой модуль?

В директории `modules` есть четыре каталога — по одному на каждый блок. Переходите в соответствующую папку и создаёте файл с именем формата `<номер_модуля_в_блоке>.h`. В нём должна быть функция с именем `<буква_блока><номер_модуля_в_блоке>`, причём буква блока именно прописная. Что эта функция принимает и что должна возвращать, можно подсмотреть в `interface/call/*.h`.

Чтобы включить добавленный модуль в проект, нужно раскомментировать соответствующую строчку в `config.h`. Для сборки достаточно скомпилировать `main.c`.

Доступные структуры и функции описаны в `template.h`. Пожалуйста, не пользуйтесь функциями выделения и освобождения памяти. Разрешено использовать небольшие массивы фиксированного размера.

И наконец, помните: ваш код - произведение искусства. Только от вас зависит, насколько приятно будет читать его другому человеку. Расставляйте отступы и пробелы, не делайте код слишком скученным, пишите комментарии. Почитайте [Linux kernel coding style](https://www.kernel.org/doc/html/v4.10/process/coding-style.html).

### Как добавить наработки в основной репозиторий?

1. Сделать копию репозитория кнопкой `Fork` (наверху справа) или подтянуть изменения с помощью "Compare", если уже есть клон репозитория;

2. Внести необходимые изменения и сделать коммиты;

3. Сделать `Pull request`. При этом могут возникнуть конфликтные ситуации — тем не менее, не отклоняйте запрос. Будем смотреть и вносить соответствующие правки.
