# HelloGit
Попытка разобраться с системой GitHub

Хотела сделать приватным, но, похоже, нельзя приватный репозиторий отправить в список(Star), так что пусть висит публичным. Я ж официально чайник :)

https://www.youtube.com/watch?v=HQ76QwYorOk  // Разбиралась по этому видео

Еще полезные команды:

Downloading from GitHub:
0) Download and install Git itself!
1) Create a folder on your computer
2) Launch GitBash
3) cd "pathToYourFolder" (you SHIFT+INSERT to paste)
4) git clone https://github.com/LinkedInLearning/databases-pf-784293.git

-- Чтобы создать папку, нужно "создать файл", и перед названием нового файла дописать название папка/

*****************************************
Я попыталась загрузить готовый проект с IDEA
https://www.youtube.com/watch?v=zM6z57OtR2Q  // по этому видео
И при слиянии двух веток (почему вообще появились отдельно master и отдельно main, если я всё из IDEA выгружала, это не должна была быть одна ветка изначально?)
появилась ошибка: main and master are entirely different commit histories
и вроде как нечему делать слияние, и у меня висит pull-request, который нельзя осуществить.
Помогло, ожидаемо, stackoverflow :

git checkout master   
git branch main master -f    
git checkout main  
git push origin main -f 

Потребовалась дополнительная авторизация на гихабе, но ветки объединились и теперь выглядят нормально.

*******************************************

Я хотела структурировать проекты на гитхабе так же, как у меня все привычно лежит по папкам. Но это пока не получается.

Можно создать подпапки в репозитории и загрузить туда файлы. Но это будет не более чем флешка, потому что слить репозиторий == слить проект. И ветки, и коммиты идут только на репозиторий, их не назначить на отдельные подпапки.

Задание на завтра: погуглить, можно ли как-то структурировать репозитории? Тэгами какими-то, может быть?
Нашла два варианта...

1) Stars-Lists, тэги на репозитории, можно отмечать и чужие

2) Я вижу, на гитхабе уже есть конспекты пары книг, которые я хотела сюда отправить. И в них я вдруг столкнулась с мыслью, что... а кто сказал, что один репозиторий - одна программа? просто создается проэкт, в котором много исполняемых файлов... так что получается, что может быть репозиторий на книгу, а в ней уже - разбитые по папкам или без них, - отдельные проэкты. И никого не смущает, что нельзя просто скачать репозиторий и получить отдельный исполняемый проэктик. Тогда почему меня должно смущать?
