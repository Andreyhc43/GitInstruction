# Памятка по GIT
## Инициализация локального git-репозитория
0. >> git config ...
1. >> git init
2. >> git add .\git_instruction.md      // индексация файла
3. >> git commit -m "Initial commit"    // сохранение коммита

4. >> git log                           // вызов журнала сохранений (--graph)

5. >> git add .\git_instruction.md
6. >> git commit -m "added 5 point"

// производим переименование файла

7. >> git add .\git_instruction_base.md
8. >> git commit -m "Rename file"

||  // при необходимости вернуться в момент со старым названием файла...    
| \
|  9. >> git log                        // копируем первые 4 символа хэш-кода нужного коммита (9469)
|  10. >> git checkout 9469
|  /  \                
| /    11. продолжаем работу с сохраненного коммита                 
|11. >> git checkout master             // возвращаемся обратно на главную ветку последнего коммита
|

9. >> git branch new_branch             // создаем новую ветку
10. >> git branch                       // отображение всех имеющихся веток *-текущая ветка
11. >> git checkout new_branch          // переходим на новую ветку
12. >> git branch branch_for_merge      
13. >> git checkout branch_for_merge    
14. продолжаем работу с файлом...
15. >> git checkout master
16. >> git merge branch_for_merge       // производим слияние веток
17. >> git branch -d branch_for_merge   // удаляем слитую ветку branch_for_merge

18. добавление файла .gitignore


19. >> git clone https://github.com/Andreyhc43/GitInstruction.git  // при необходимости клонируем заранее созданный репозиторий с git-hub
20. >> git push --set-upstream https://github.com/Andreyhc43/GitInstruction.git master // загружаем на сервер нужную ветку
21. указываем пароль аккаунта 