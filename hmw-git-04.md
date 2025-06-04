### Домашнее задание к занятию «Инструменты Git» -- Мельник С.В.

#### Задание

В клонированном репозитории:

Найдите полный хеш и комментарий коммита, хеш которого начинается на aefea.

![задание](https://github.com/DeluxWebSite/devops-netology/blob/master/01.png)

Ответьте на вопросы.

- Какому тегу соответствует коммит 85024d3?

![задание](https://github.com/DeluxWebSite/devops-netology/blob/master/02.png)

- Сколько родителей у коммита b8d720? Напишите их хеши.

Два родителя:

56cd7859e05c36c06b56d013b55a252d0bb7e158

9ea88f22fc6269854151c571162c5bcf958bee2b

- Перечислите хеши и комментарии всех коммитов, которые были сделаны между тегами v0.12.23 и v0.12.24.

![задание](https://github.com/DeluxWebSite/devops-netology/blob/master/04-1.png)
![задание](https://github.com/DeluxWebSite/devops-netology/blob/master/04-2.png)

- Найдите коммит, в котором была создана функция func providerSource, её определение в коде выглядит так: func providerSource(...) (вместо троеточия перечислены аргументы).

git log -S 'func providerSource'

Получили:

commit 5af1e6234ab6da412fb8637393c5a17a1b293663

Date: Tue Apr 21 16:28:59 2020 -0700

commit 8c928e83589d90a031f811fae52a81be7153e82f

Date: Thu Apr 2 18:04:39 2020 -0700

Посмотрим более ранний из них:

git show 8c928e8 | grep "func providerSource"

+func providerSource(services \*disco.Disco) getproviders.Source {

Нашли: это коммит 8c928e83589d90a031f811fae52a81be7153e82f

- Найдите все коммиты, в которых была изменена функция globalPluginDirs.

git log -S 'globalPluginDirs'

Получили 3 коммита: commit 35a058fb3ddfae9cfee0b3893822c9a95b920f4c

Date: Thu Oct 19 17:40:20 2017 -0700

commit c0b17610965450a89598da491ce9b6b5cbd6393f

Date: Mon Jun 12 15:04:40 2017 -0400

commit 8364383c359a6b738a436d1b7745ccdce178df47

Date: Thu Apr 13 18:05:58 2017 -0700

Соответственно, в наиболее раннем из них функция создана, а в следующих отредактирована:

c0b17610965450a89598da491ce9b6b5cbd6393f

35a058fb3ddfae9cfee0b3893822c9a95b920f4c

- Кто автор функции synchronizedWriters?

![задание](https://github.com/DeluxWebSite/devops-netology/blob/master/07-1.png)
![задание](https://github.com/DeluxWebSite/devops-netology/blob/master/07-2.png)
![задание](https://github.com/DeluxWebSite/devops-netology/blob/master/07-3.png)

Автор: Martin Atkins
