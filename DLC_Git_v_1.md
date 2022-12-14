# DLC к Git
## Знакомство с удаленными репозирориями
В начале данного DLC стоит зарегистрироваться и авторизоваться на сайте GitHub [https://github.com].

Не забудь познакомить программу Git с собой по средством команд:
- git config --global user.name "Твой НикНейм"
- git config --global user.name Твой@эмейл
## Работа с удаленным репозиторием
Вначале всего найдем через __*поисковое окно*__ чужой удаленный репозиторий.  
С помощью иконки __*Copy*__ копируем адрес удаленного репозитория.  
Затем возвращаемся в программу GIT и вводим в ней следущую команду:

```
git clone + Скопированный адрес удаленного репозитория
```

Теперь можно подробнее посмотреть скаченный удаленный репозиторий.
## Работа с ограниченным удаленным репозиторием
Что если вы захотели поучавствовать в ограниченном проекте?
Выход есть!  
Вначале всего найдем через __*поисковое окно*__ .Ограниченный удаленный репозиторий.  
Затем yажмем иконку  __*Fork*__ .  
Таким образом мы полностью копируем ограниченный удаленный репозиторий нашим на наш аккаунт GitHUb.  
Мы также клонируем его в отдельную папочку на нашем компьютере путем команды:

```
git clone + Скопированный адрес удаленного репозитория
```
__Чтобы сохранить ту информацию что ты исправил, либо добавил в удаленный репозиторий - пропиши команду:__

```
git push
```
Данная команда служит обновлением информации в удаленном репозитории.
Затем на GitHub у тебя должна появиться индикатор __*Compare & pull request*__ - нажми на нее.
Добавиш описание и информацию, затем отправляешь.

## Создание собственного репозитория
Предположим ты создал Папку (локальный репозиторий) и файл в котором уже есть несколько каммитов.  
Как выгрузить этот репозиторий на GitHub?
Следуй по следущему пути:  
1. Обязательно Авторизуйся как в Git, так и в GitHub
2. В GitHub около своего профиля нажми на +, а затем на словосочетание __*NEW REPOSITORY*__
3. Назови свой удаленный репозиторий
4. В Git прописываешь команды по очереди:  
    - git remote add origin http://github...
    - git branche -M main
    - git push -u origin main
5. Бывает возникает ошибка тогда, после команд пропиши:  
    - git remote set-url origin http://github...
6. Затем снова:  
    - git push -u origin main

Теперь твой репозиторий есть и в GitHub.

## Обновление данных с удаленного репозитория GitHub в локальный репозиторий Git
Предположим ты поработал в Удаленном репозитории и сохранил изменения, но на локальном репозитории у тебя устаревшие данные.

Как обновить данные в локальном репозитории?  
Пропиши команду:

```
git pull
```
