1. Создать внешний репозиторий c названием JSON.
+ нажать `+` `New repository`

2. Клонировать репозиторий JSON на локальный компьютер.
+ `cd /Users/igori/Documents/github`
+ `git clone https://github.com/igorlipskii/json.git`

3. Внутри локального JSON создать файл “new.json”.
+ `touch new.json`

4. Добавить файл под гит.
+ `git add new.json`

5. Закоммитить файл.
+ `git commit -m "add new file .json"`

6. Отправить файл на внешний GitHub репозиторий.
+ `git push`

7. Отредактировать содержание файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON.
+ `vim new.json`
+ `i` — перейти в режим редактирования

```json
{
	"Name": "Igor Lipskii",
	"Age": 33,
	"Pet": "No pets",
	"Salary": {
		"Junior": "80.000 rub",
		"Middle": "190.000 rub",
		"Senior": "320.000+ rub"
		}
}
```
+ `esc` `:` `wq`

8. Отправить изменения на внешний репозиторий.
+ `git add new.json`
+ `git commit -m  "wrote information about myself`
+ `git push`

9. Создать файл preferences.json
+ `touch preferences.json`

10. В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате JSON.
+ `vim new.json`
+ `i` — перейти в режим редактирования

```json
{
	"My preferences": {
		"Film": "John Carter",
		"Series": "La casa de papel",
		"Food": [
			"pasta",
 			"vegetables",
			"meat"
		],
		"Season": "Summer",
		"Place to visit": [
			"USA",
			"Japan",
			"New Zealand"
		]
	}
}
```
+ `esc` `:` `wq`

11. Создать файл sklls.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON
+ `vim new.json`
+ `i` — перейти в режим редактирования
```json
{               
        "Skills": {
                "1": "Basic theory (What is testing, bug reports, documentation, types, methods, testing directions, etc.)",
                "2": "What is a client-server architecture.",
                "3": "HTTP Methods of requests to the server.",
                "4": "HTTP server response codes.",
                "5": "Structures of HTTP requests and responses.",
                "6": "What is JSON, XML. Their structure.",
                "7": "API testing via Postman (JS, API autotests).",
                "8": "Removing and reading logs from an external server.",
                "9": "Sniffing http web traffic via Charles and Fiddler.",
                "10": "Dev Tools of web browsers (Google Chrome, FireFox).",
                "11": "VPN (How it works, why you need it, how to use it, tool options).",
                "12": "Mobile testing.",
                "13": "Feature iOS, Android, guidelines.",
                "14": "Building iOS applications on XCode. (Those who do not have a Mac computer, just look).",
                "15": "Building Android applications on Android Studio.",
                "16": "ADB (android device management).",
                "17": "Setting up proxy and vpn on iOS and Android.", 
                "18": "Interception (sniffing) of mobile traffic via Charles and Fiddler on iOS and Android.",
                "19": "Command line (terminal) Linux (copying, creating, viewing, moving files on servers without a graphical interface)",
                "20": "Basics of bash scripting, automation of routine tasks on the server.",
                "21": "Access to remote servers.",
                "22": "SQL basics (Create, Delete, Drop, Insert Into, Select, From, Where, Join).",
                "23": "Postgres database (installation, configuration and use).",
                "24": "Non-relational database Redis (installation, configuration and use).",
                "25": "Load testing in Jmeter.",
                "26": "Scrum development methodology.",
                "27": "Python. (Learning the basics. Creating a client-server application)."
                }
}
```
+ `esc` `:` `wq`

12. Отправить сразу 2 файла на внешний репозиторий.
+ > `git add preferences.json skills.json`
или `git add {preferences,skills}.json`

+ `git commit -m  "add skills and preferences files"`
+ `git push`
+ > одной командой `git add {preferences,skills}.json && git commit -m "add 2 files and commit and push" && git push`

13. На веб интерфейсе создать файл bug_report.json.
+ нажать `add new file` `create new file` пишем название файла

14. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
+ в `commit new file` пишем `create bug_report.json`

15. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON.
+ нажать `edit this file`

```json
{
	"Project": "Calculator",
	"ID": 88,
        "Summary": "Результат умножения неверен",
	"Description": "Результат равен ожидаемому результату +2",
	"Steps to reproduce": {
		"Step 1": "Открыть сайт https://nuix.github.io/SDET/senior-sdet/stagingCalc/index.html",
		"Step 2": "Нажать цифру 6",
		"Step 3": "Нажать знак умножения",
		"Step 4": "Нажать цифру 3",
		"Step 5": "Нажать знак равно"
	},
	"Actual result": 20,
	"Expected result": 18,
	"Attachments": ["https://somup.com/c3nq02TjpH"],
	"Severity": "Critical",
	"Priority": "High",
	"Labels": "Smoke",
	"Environment": {
		"Operational system": "macOS Big Sur 11.6.4",
		"Browser version": "Google Chrome 98.0.4758.102"
	},
	"Author": "Igor Lipskii",
	"Test Data": "20.02.2022"
}
```
+ `esc` `:` `wq`

16. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
+ пишем в `Commit changes` `update bug_report`

17. Синхронизировать внешний и локальный репозиторий JSON
+ `git pull`
