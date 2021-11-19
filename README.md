# Лабораторная работа №6
*Первым шагом мы создаем копию [репозитория](https://github.com/Kurtyanik/LR6/) в личное хранилище.*

![image](https://github.com/4018KSigachevaDN/LR6/blob/master/images/1.png)

*Затем настраиваем клиент git, вводим имя пользователя и email. Комманды: `git config --global user.name <username>`; `git config --global user.email <email>`.*

![image](https://github.com/4018KSigachevaDN/LR6/blob/master/images/2.png)

*Клонируем удалённый репозиторий на компьютер. Комманда: `git clone <url>`.*

![image](https://github.com/4018KSigachevaDN/LR6/blob/master/images/3.png)

*Добавляем файл через интерфейс GitHub. Комманда: `cd LR6/`.*

![image](https://github.com/4018KSigachevaDN/LR6/blob/master/images/4.png)

*Поддтягиваем изменения в локальный репозиторий. Комманда: `git pull`.*

![image](https://github.com/4018KSigachevaDN/LR6/blob/master/images/5.png)

*Посмотрим коммиты ветки master. Комманда: `git log`.*

![image](https://github.com/4018KSigachevaDN/LR6/blob/master/images/6.png)

*Просмотрим существующие ветки в текщем репозитории, затем перейдем в ветку branch1. Комманды: `git branch`; `git checkout branch1`.*

![image](https://github.com/4018KSigachevaDN/LR6/blob/master/images/7.png)

*Посмотрим коммиты ветки branch1. Комманда: `git log`.*

![image](https://github.com/4018KSigachevaDN/LR6/blob/master/images/8.png)

*Подробно рассмотрим коммиты. Комманда: `git log -p`.*

![image](https://github.com/4018KSigachevaDN/LR6/blob/master/images/9.png)

*Выполняем слияние в ветку master. Комманда: `git merge branch1`.*

*Разрешаем возникший конфликт: в теории конфликт возник из-за того, что файл mergefile.txt не отслеживается. Проверив это и убедившись, добавляем файл для отслеживания, оставляем коммит. Команды:`git status`; `git add mergefile.txt`; `git commit -m "Branches"`.*

![image](https://github.com/4018KSigachevaDN/LR6/blob/master/images/10.png)
![image](https://github.com/4018KSigachevaDN/LR6/blob/master/images/11.png)

*Удаляем побочную ветку после успешного слияния. Комманда: `git branch -d branch1`*

![image](https://github.com/4018KSigachevaDN/LR6/blob/master/images/12.png)

*Создаем изменения и фиксируем их, оставляя комментарии,несколько раз. Команды:`echo hello > change1.txt/change2.txt`; `git add change1.txt/change2.txt`; `ggit commit -m "Change1.txt/Change2.txt"`*

![image](https://github.com/4018KSigachevaDN/LR6/blob/master/images/13.png)
![image](https://github.com/4018KSigachevaDN/LR6/blob/master/images/14.png)

*Просмотр комментариев.*

![image](https://github.com/4018KSigachevaDN/LR6/blob/master/images/15.png)
![image](https://github.com/4018KSigachevaDN/LR6/blob/master/images/16.png)

*Делаем «хард» откат коммита. Комманда: `git reset --hard HEAD~1`*

![image](https://github.com/4018KSigachevaDN/LR6/blob/master/images/17.png)

*Создаем ветку для отчёта. Комманда: `git branch report`*

![image](https://github.com/4018KSigachevaDN/LR6/blob/master/images/18.png)

*Оформляем отчёт в файле README.md *

*Получаем итоговую историю операций.  Комманда: `git log`*

![image](https://github.com/4018KSigachevaDN/LR6/blob/master/images/19.png)
![image](https://github.com/4018KSigachevaDN/LR6/blob/master/images/20.png)

После редактирования отчета, его нужно будет сохранить и произвести команды `git add` и `git commit`.

В конце работы необходимо будет отправить все локальные изменения в сетевое хранилище GitHub командой `git push`.
