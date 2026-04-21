git init - Инициализирует новый репозиторий в текущей директории

git status - Показывает текущее состояние рабочего каталога

git remote add origin git@github.com:molchanovas83-svg/git-project.git - Добавляет удалённый репозиторий к локальному

git remote -v - убедиться что репозитории связаны

git push -u origin master - Устанавливаете связь между веткой в которой вы находитесь и веткой master на удалённом сервере

git add --all - Добавляет все изменения в репозиторий

git commit -m "создание первого коммита" - Создаёт коммит с указанным сообщением

git push - Загружает изменения из локального репозитория в удалённый



Статусы git:

untracked - неотслеживаемый файл

tracked - отслеживаемый файл

staged - Файл попадает в staging area и переходит статус staged после выполнения git add .

modified - файл был изменён



Жизненный цикл:

```mermaid

graph LR;

&#x20; untracked -- "git add" --> staged;

&#x20; staged -- "git commit" --> tracked/comitted;

&#x20; tracked/committed -- "изменение в файле" --> modified/changed;

&#x20; modified/changed -- "git add" --> staged;



``` 

