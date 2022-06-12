Форкаем проект KotlinAsFirtst2020

Клонируем на компьютер
git clone https://github.com/Konstantin-Erastov/KotlinAsFirst2020

Указываем в качестве upstream-my
1)git remote add upstream-my https://github.com/Konstantin-Erastov/KotlinAsFirst2021
2)git fetch upstream-my

Создаём ветку backport, копируем туда коммиты из upstream-my

Нужно указывать upstream-theirs и сделать merge c master
1)git remote add upstream-theirs https://github.com/yrmint/KotlinAsFirst2021
2)git fetch upstream-theirs
3)git merge -s ours upstream-theirs/master

Создаём файл remotes
Помещаем туда вывод git remote -v
И коммитим в master
1)git remote -v > remotes
2)git add remotes
3)git commit -m "remotes"

Нужно создать файл howto.md и записать все действия
touch howto.md
1)git add howto.md
2)git commit -m "howto"

В конце загружаем на github
