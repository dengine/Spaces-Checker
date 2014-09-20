Spaces-Checker - уведомления о новых событиях на Spaces.ru в реальном времени.

	1. Скачайте .zip архив и распакуйте в какую-нибудь папку.
	3. (не обязательно) Создайте симлинк на check.php (выполнять из-под root или с sudo).
			> ln -s /path/to/check.php /bin/spaces
	3. Предоставьте check.php права запуска.
	 		> chmod +x /path/to/check.php

Использование:

	-a,	--sid
		Указывает SID для входа. Пример: spaces --sid 123
		Обязательный парамерт, если не задан -f или --file.
	-f, --file
		Указывает файл, хранящий SID. Пример: spaces -f .conf
		Обязательный парамерт, если не задан -a или --sid.
	-c, --check
		Указывает события, о которых нужно оповещать.
		Ключевые слова: mail (почта), journal (журнал), feed (лента).
		Пример: spaces --check mail,feed
		Значение по умолчанию: mail,journal,feed.
	-s, --sound
		Указывает события, наступление которых необходимо сопровождать звуком.
		Пример: spaces --sound mail,journal
		Значение по умолчанию: mail,journal,feed.
	-i, --interval
		Устанавливает интервал проверки новых событий.
		Значение по умолчанию: 3.
	-g, --groups
		Указывает, какие группы неоходимо мониторить на наличие новых тем.
		Пример: spaces --groups 79936,5692
	-ngs, --no-group-sound
		Не сопровождать появление новых тем в группах звуком.
		Пример: spaces --no-group-sound

Наслаждайтесь!