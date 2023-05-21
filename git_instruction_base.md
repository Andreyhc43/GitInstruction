# Памятка по GIT
## Инициализация локального git-репозитория
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
