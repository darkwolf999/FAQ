<H2> Добавление репозитория </H2>

**Если проект новый (есть только на ПК, требуется залить на удаленный репозиторий):**

1. Создаем репозиторий на гитхабе, желательно с таким же именем, как и имя проекта на ПК (для меньшей путаницы)
2. Открываем git bash.
3. $ **cd source/repos/test**						<span style="color:green">//Переходим в каталог своего проекта</span>
4. $ **git init**							<span style="color:green">//Инициализируем каталог с проектом как локальный репозиторий</span>
5. $ **git remote add origin https://github.com/darkwolf999/test.git**	<span style="color:green">//Добавляем удаленный репозиторий для дальнейшей работы с ним
   "origin" - присвоенное имя для удаленного репозитория, чтобы не вводить каждый раз ссылку на него. Имя может быть любым</span>
6. $ **git add .**								<span style="color:green">//Добавляем в локальный репозиторий все файлы из каталога и вложенных папок (Индексируем их)</span>
7. $ **git commit -m "First commit"**					<span style="color:green">//Фиксируем изменения на локальном репозитории</span>
8. Если гит напишет Please tell me who you are, вводим следующие команды:  
   $ **git config --global user.name "user"**				<span style="color:green">//Имя пользователя</span>  
   $ **git config --global user.email user@example.com**			<span style="color:green">//Почта, привязанная к гитхабу</span>
9. $ **git push origin master**						<span style="color:green">//Отсылаем проект на удаленный репозиторий</span>
10. Может потребовать ввести логин пароль для гитхаба

**Если проект есть только на удаленном репозитории, и его необходимо скачать на ПК для дальнейшей работы:**

1. $ **cd source/repos**					<span style="color:green">//Переходим в папку со всеми проектами на ПК</span>
2. $ **git clone https://github.com/darkwolf999/test.git**	<span style="color:green">//Копируем проект с удаленного репозитория на ПК</span>
3. $ **cd test** 						<span style="color:green">//Переходим в каталог с проектом</span>  
По мере изменения проекта на ПК
4. $ **git add .**						<span style="color:green">//Добавляем в локальный репозиторий все файлы из каталога и вложенных папок (Индексируем их)</span>
5. $ **git commit -m "First commit"**			<span style="color:green">//Фиксируем изменения на локальном репозитории</span>
6. $ **git push origin master**				<span style="color:green">//Отсылаем проект на удаленный репозиторий</span>

<H2> Прочие команды </H2>

$ **git remote -v**		<span style="color:green">//Просмотреть удаленный репозиторий и ассоциированное с ним имя</span>  
$ **git pull** 		<span style="color:green">//Обновить проект на локальном репозитории, если он был изменен на удаленном</span>