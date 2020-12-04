# LR6
Лабораторная работа №6

**Цель лабораторной работы:** изучение базовых возможностей системы
управления версиями, опыт работы с Git Api, опыт работы с локальным и
удаленным репозиторием. 

**Ход работы:**
1. Создал аккаунт на сайте GitHub ([вот он](https://github.com/caVenikk)).
2. Сделал копию в личное хранилище [отсюда](https://github.com/Kurtyanik/LR6/).
3. Установил Git.
4. После установки настроил клиент Git, введя имя пользователя (4917 Novikov N. I.) и email.<br>
Использовал команды git config --global user.name "4917 Novikov N. I." и git config --global user.email jimolostlal@gmail.com<br>
5. Клонировал удаленный репозиторий на компьютер.<br>
Использовал команду git clone https://github.com/Kurtyanik/LR6/<br>
	![Рисунок 1](/Screenshots/1.png)<br>
	Рисунок 1. Демонстация выполнения пунктов 4 и 5
6. Перешел в ветку branch1, добавил файл и отредактировал его (через интерфейс GitHub). Далее подтянул изменения в локальный репозиторий.<br>
Использовал команды cd LR6, чтобы зайти в локальный репозиторий, git checkout branch1, чтобы перейти в побочную ветку и подтянул изменения с помощью команды pit pull https://github.com/caVenikk/LR6/ branch1<br>
	![Рисунок 2](/Screenshots/2.png)<br>
	Рисунок 2. Добавление и редактирование файла<br>
	![Рисунок 3](/Screenshots/3.png)<br>
	Рисунок 3. Файл в репозитории (в ветке branch1)<br>
	![Рисунок 4](/Screenshots/4.png)<br>
	Рисунок 4. Переход во вторую ветку и подтягивание изменений<br>

***Продолжаем работу локально***

7. Получил историю операций для каждой из веток.
8. То же самое

Использовал команду git log в каждой из веток.

	![Рисунок 5](/Screenshots/5.png)

	Рисунок 5. История операций в ветке branch1

	![Рисунок 6](/Screenshots/6.png)

	Рисунок 6. История операций в ветке master

9. Выполняю слияние в ветку master, разрешив конфликт.

Использовал команды git merge branch1 (в ветке master), vim mergefile.txt (чтобы открыть конфликтующий файл), git add mergefile.txt и git commit.

Этапы видны на рисунках:

	![Рисунок 7](/Screenshots/7.png)

	Рисунок 7. Ввод команды слияние и открытие в редакторе файла, из-за которого происходит конфликт

	![Рисунок 8](/Screenshots/8.png)

	Рисунок 8. Отредактированный файл

	![Рисунок 9](/Screenshots/9.png)

	Рисунок 9. Подтверждение изменения файла

	![Рисунок 10](/Screenshots/10.png)

	Рисунок 10. Проверка выполнения слияния путем просмотра истории операций

10. Удаляю ветку branch1

Использовал команду git branch -D branch1

	![Рисунок 11](/Screenshots/11.png)

	Рисунок 11. Удаление ветки branch1

11. Редактирую созданный мной файл file.txt

Использовал команды vim file.txt, git add file.txt и git commit -m 'Сделал изменения'

	![Рисунок 12](/Screenshots/12.png)

	Рисунок 12. Открытие в редакторе файла

	![Рисунок 13](/Screenshots/13.png)

	Рисунок 13. Редактирование файла

	![Рисунок 14](/Screenshots/14.png)

	Рисунок 14. Подтверждение редактирования файла

12. Делаю "хард" откат коммита

Использовал команду git reset --hard HEAD~1 (чтобы сделать откат одного коммита).

	![Рисунок 15](/Screenshots/15.png)

	Рисунок 15. Откат коммита

13. Создал ветку для отчета командой git ckeckout -b report
14. Оформил отчет в файле README.md, используя markdown синтаксис.
15. Получил историю операций в форматированном виде.

Использовал команду git log --pretty=format:"%h - %ad %an : %s"

	![Рисунок 16](/Screenshots/16.png)

	Рисунок 16. Получение истории операций в форматированном виде

16. Отправляю локальные изменения в сетевое хранилище GitHub.

Использовал команды git add \*, git status и git commit -m 'Добавил скриншоты' 

	![Рисунок 17](/Screenshots/17.png)

	Рисунок 17. Подтверждение добавление всех (практически) скриншотов

	![Рисунок 18](/Screenshots/18.png)

	Рисунок 18. Отправка локальных изменений на сервера GitHub

	![Рисунок 19](/Screenshots/19.png)

	Рисунок 19. Отправка локальных изменений на сервера GitHub

**Вывод:** изучил базовые возможности системы управления версиями, получил опыт работы с Git Api, а также опыт работы с локальным и удаленным репозиторием.
