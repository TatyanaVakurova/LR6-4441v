# LR6
Лабораторная работа №6

Система контроля версий

Работу  выполнил: студент группы 4441в Вакурова Татьяна Александровна

**Цель работы:** *изучение базовых возможностей системы
управления версиями, опыт работы с Git Api, опыт работы с локальным и
удаленным репозиторием.*

**1. Сделана копия в личное хранилище из https://github.com/Kurtyanik/LR6/ (Fork)**

**2. Установлен Git (https://git-scm.com/).**

**3. После установки настроен клиент Git**

    git config --global user.name "4441в Vakurova Tatyana"
    git config --global user.email "vakurovatatyana@mail.ru"
**4. Клонирование репозитория на компьютер**

    git clone https://github.com/TatyanaVakurova/LR-4441v
**5. Добавлен файл, подтянуты изменения в репозиторий**

    touch new_file.txt
    git pull origin master
**6. Получена история операций для каждой из веток**

    git log --all --decorate --oneline --graph
**7. Просмотрены последние изменения**
    
    git log
**8. Создание новой ветки**

    git checkout -b feature/new-feature
   
**9. Выполнено слияниие в ветку master, разрешив конфликт(убрать символы)**

    git checkout master
    git merge -b feature/new-feature
**10. Удалена побочную ветку после успешного слияния**

    git branch -d feature/new-feature
**11. Сделаны изменения и зафиксированы, оставлены комментарии. Также сделан откат коммита**

    echo "Another update" >> new_file.txt
    git add new_file.txt
    git commit -m "добавили строчку"
    git resert HEAD~1
**12. Создана ветка для отчета (report)**

    git checkout -b report
**13. На GitHub загружены снимки экрана, сделаные в ходе работы.**

**14. Получена история операций в форматированном виде.**

