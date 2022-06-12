Форкаем проект KotlinAsFirtst2020
Клонируем на компьютер
git clone https://github.com/Konstantin-Erastov/KotlinAsFirst2020
Указываем в качестве upstream-my
git remote add upstream-my https://github.com/Konstantin-Erastov/KotlinAsFirst2021
git fetch upstream-my
Создаём ветку backport, копируем туда коммиты из upstream-my
Нужно указывать upstream-theirs и сделать merge c master
git remote add upstream-theirs https://github.com/yrmint/KotlinAsFirst2021
git fetch upstream-theirs
git merge -s ours upstream-theirs/master
Создаём файл remotes
Помещаем туда вывод git remote -v
И коммитим в master
git remote -v > remotes
git add remotes
git commit -m "remotes"
Нужно создать файл howto.md и записать все действия
touch howto.md
git add howto.md
git commit -m "howto"
В конце загружаем на github
