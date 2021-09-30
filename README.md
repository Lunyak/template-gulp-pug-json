# Сборка GULP + PUG + JSON

Данная сборка позволяет вам быстрее писать код, использовать 
готовые решения, пользоваться преимуществами препроцессоров.

## Как устанавливать?

Для начала вам нужно склонировать данный репозиторий 
к себе на компьютер. Открыть проект в редакторо кода 
и выполнить команду ```npm i``` в терминале. Тем самым
вы установите все зависимости нужные для работы. Вам
останется только запустить нашу сборку.

Запуск проекта производиться коммндой

```sh
npm run dev
```

или просто

```sh
gulp
```

Как работать с JSON файлами
Вам нужно создать файл в папке .src/data/...
Важно что бы этот файл не был пустым иначе будет ошибка
Затем все содержимоей файл при запуске проекта считывается
И автоматичесски помещается в переменную с одноименным название файла
которую вы можете вызвать в pug

 ## К примеру
если у нас естьф файл в папке data
| Файл | Содержимое |
| ------ | ------ |
| main.json | {"name": "text"}|

то в Pug нужно будет вывести следующее
const data = data.main.name
выведет нам "текст"

Все рабочие файлы для разработчика находятся в папке ```src```
