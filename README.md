# HelloGit
Попытка разобраться с системой GitHub

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
