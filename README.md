

Hi ![](https://user-images.githubusercontent.com/18350557/176309783-0785949b-9127-417c-8b55-ab5a4333674e.gif)My name is Ivan Ivashchenko
===================================================================================================================================
[![Typing SVG](https://readme-typing-svg.herokuapp.com?color=%2336BCF7&lines=I+am+frontend+developer)](https://git.io/typing-svg)

* ✉️  You can contact me at [ivan86.ivashchenko@gmail.com](mailto:ivan86.ivashchenko@gmail.com)

[![trophy](https://github-profile-trophy.vercel.app/?username=ryo-ma)](https://github.com/ryo-ma/github-profile-trophy)

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra)](https://github.com/anuraghazra/github-readme-stats)

[![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra)](https://github.com/anuraghazra/github-readme-stats)


daniilshat
2 фев 2022 в 22:00
Оформляем README-файл профиля на GitHub
14 мин
114K
GitHub
*
Карьера в IT-индустрии
Социальные сети и сообщества
Летом 2020 года GitHub позволила пользователям создавать персональные README-файлы и с их помощью кастомизировать свои профили. Сама платформа при создании подобного файла предлагает уже готовый шаблон, в который можно вписать свои данные. Но о какой кастомизации может идти речь, если у всех будут одинаково оформленные профили? За почти два года сообщество придумало множество различных способов выделиться и особенно оформить свою страницу на GitHub.


Создаем README.md профиля
Для того чтобы создать README-файл, который будет отображаться в профиле, необходимо создать новый публичный репозиторий с названием, полностью повторяющим никнейм пользователя. Также важно не забыть поставить галочку в поле, предлагающем вместе с репозиторием создать и README.md. Во время настройки репозитория нас поздравит Октокот и сообщит о том, что только что мы создали особенный репозиторий и его содержимое будет отображаться на странице профиля. GitHub автоматически сделает базовый шаблон, в который можно вписать информацию о себе, а можно не вписывать и сделать что-то чуть более интересное.

Официальный профиль Октокота с базовым README профиля
Официальный профиль Октокота с базовым README профиля
Для редактирования файла понадобятся знание Markdown-разметки и базовое понимание HTML. Оба навыка не сложны в освоении и интуитивно понятны в том объеме, который необходим для кастомизации профиля. На самом деле можно ограничиться только Markdown, но его особенность в том, что текст автоматически выравнивается по левому краю и нет никакой возможности повлиять на это. А HTML в тандеме с Markdown позволяет контролировать расположение объектов на экране. Для создания интерактивных блоков понадобится понимание того, как устроен сервис GitHub Actions, но нужны тоже только лишь базовые знания. Глубокие понадобятся только в том случае, если захочется создать собственный динамический виджет.

Заголовок
Как уже и говорилось ранее, заголовки можно писать как с помощью Markdown, так и с помощью HTML. Последний способ поможет разместить текст по центру, что мне больше нравится — выделяется на фоне основного текста. Заголовок обычно содержит в себе приветствие, обращенное к посетителю профиля. Имя в моем заголовке оформлено в виде ссылки и ведет на сайт-визитку, в конце расположен эмодзи с машущей рукой, значок анимированный. Второй строчкой можно коротко рассказать о своей деятельности, чтобы посетителю сразу было ясно, с кем он имеет дело.

Заголовок в моем профиле
Заголовок в моем профиле
Оформляется все это дело вот такой нехитрой HTML-конструкцией:

<h1 align="center">Hi there, I'm <a href="https://daniilshat.ru/" target="_blank">Daniil</a> 
<img src="https://github.com/blackcater/blackcater/raw/main/images/Hi.gif" height="32"/></h1>
<h3 align="center">Computer science student, IT news writer from Russia 🇷🇺</h3>
Можно сделать с помощью Markdown, но тогда не получится выровнять текст по центру и будут сложности с гифкой — в Markdown не предусмотрены теги для указания размеров изображения:

# Hi there, I'm [Daniil](https://daniilshat.ru/) ![](https://github.com/blackcater/blackcater/raw/main/images/Hi.gif) 
### Computer science student, IT news writer from Russia 🇷🇺
Некоторые умельцы вовсе отказываются от текстовых заголовков и используют баннеры в их качестве. Баннер можно сделать самостоятельно в любом удобном редакторе изображений или использовать конструкторы, например, REHeader.

Так бы мог выглядеть мой профиль с банером
Так бы мог выглядеть мой профиль с банером
Картинку можно вставить как с помощью Markdown, так и с помощью HTML. Опять же, последний вариант позволяет контролировать расположение изображения и его размер:

![Описание](ссылка)
<img src="путь к файлу" alt="альтернативный текст">
Можно использовать необычные шрифты. К сожалению, нет возможности подключить CSS-стили и полноценно кастомизировать внешний вид текста, но можно найти подходящий шрифт, набрать необходимый текст и вставить в README.md. Для этих целей подойдут сервисы, излюбленные пользователями Twitter и Instagram. Все шрифты из подобных конвертеров включены в таблицу символов Unicode и корректно отображаются на всех современных платформах.

Unicode-шрифт в заголовке
Unicode-шрифт в заголовке
Помимо всего прочего, можно добавить анимированный текст с эффектом печати. В репозитории проекта есть подробная инструкция по настройке блока и советы по развертыванию приложения на собственном сервере. Также разработчик сделал веб-интерфейс для настройки — можно указать все необходимые параметры, а сервис выдаст готовый код для встраивания.

<!---Пример кода-->
[![Typing SVG](https://readme-typing-svg.herokuapp.com?color=%2336BCF7&lines=Computer+science+student)](https://git.io/typing-svg)
Анимированный заголовок
Анимированный заголовок
О себе
После заголовка принято рассказывать о себе, представлять свои навыки, возможности и давать ссылки для обратной связи. Это, конечно же, необязательное условие, можно расположить блоки в любой последовательности, но в этой части статьи рассмотрим именно те инструменты, которые помогут организовать блок «О себе».

Simple Icons — огромная коллекция иконок популярных брендов, компаний, технологий и сервисов в svg-формате. У проекта есть сайт, на котором можно найти удобную иконку и скачать себе, а потом использовать в своем md-файле. Вставлять изображения лучше с помощью HTML — так удобнее задавать необходимый размер.


Markdown Badges — библиотека бейджей с готовыми фрагментами md-кодов для вставки. Коллекция обширная, можно найти необходимые языки программирования, технологии и оформить блок, к примеру, навыков.


Shields.io — инструмент для генерации кастомных бейджей. Можно выбрать из готовых шаблонов и подогнать под свой случай, а можно настроить полностью с нуля.

Статистика
В README-файл профиля можно добавлять различные виджеты со статистическими данными о себе и свой деятельности на GitHub. Данные автоматически обновляются с некоторой периодичностью и в профиле всегда отображается актуальная информация:

GitHub Trophy — добавляет в профиль трофеи и ачивки. Награды показывают, насколько пользователь активно ведет свой профиль. Для выбора доступно более десяти различных цветовых схем, что позволяет настроить виджет под свой стиль оформления. Также можно выбрать различные варианты расположения наград и включить фильтрацию. Для добавления необходимо вставить следующий md-код в свой файл, параметр username= необходимо заменить на свой никнейм на платформе.

[![trophy](https://github-profile-trophy.vercel.app/?username=ryo-ma)](https://github.com/ryo-ma/github-profile-trophy)

Longest streak stats — добавляет виджет, показывающий актуальную продолжительность ежедневных сессий на GitHub, самую длинную сессию за все время и суммарное количество вкладов в сообщество. Автор виджета предлагает подробную инструкцию по его настройке, но вместе с этим предоставляет и визуальный конструктор, позволяющий настроить необходимую цветовую схему. Кроме этого, в репозитории разработчика имеется руководство по развертыванию приложения на собственном сервере. Если вставлять код из примеров, то параметр user= надо заменить на свой никнейм, если создавать собственный дизайн в конструкторе, то система выдаст необходимый код для вставки.

[![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=DenverCoder1)](https://git.io/streak-stats)

Top Languages Card — виджет, выводящий статистику по часто используемым языкам в репозиториях пользователя. Можно выводить информацию как по всем репозиториям в профиле, так и только по избранным. Есть возможность удалить некоторые языки и никогда не показывать их в поле активности. Также можно выбрать компактный и более подробный вид карточки. Есть поддержка разных цветовых схем. При вставке кода необходимо заменить параметр username= на свой никнейм.

<!---Для компактной версии-->
[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra&layout=compact)](https://github.com/anuraghazra/github-readme-stats)

<!---Для подробной версии-->
[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra)](https://github.com/anuraghazra/github-readme-stats)

GitHub Stats Card — карточка от разработчика прошлого виджета. Виджет выводит основную информацию о деятельности пользователь на платформе — общее количество звезд, коммитов и вкладов в сообщество. Также карточка отображает оценку пользователя, сравнивая его деятельность с другими юзерами GitHub. Доступно около десятка уже готовых тем, но можно настроить и уникальную. Ненужные позиции в статистике можно скрыть. Для вставки все так же надо скопировать код, добавить в свой файл и заменить параметр username= на актуальный.

[![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra)](https://github.com/anuraghazra/github-readme-stats)

GitHub Extra Pins — и уже третья карточка все от того же самого разработчика. GitHub позволяет закреплять на странице профиля не более 6 репозиториев, но если этого мало, то можно добавить их в README-файл в виде карточки и не ограничиваться только 6 проектами. Для вставки надо заменить параметры username= на актуальный никнейм, repo= на название необходимого репозитория, а в скобках указать ссылку на сам репозиторий.

[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=anuraghazra&repo=github-readme-stats)](https://github.com/anuraghazra/github-readme-stats)

Codewars — баннер со статистикой сервиса с задачами для программистов. Виджет показывает количество решенных задач и актуальный уровень пользователя на платформе. Ссылки на карточки можно найти в своем профиле, нажав на кнопку «View Profile Badges» под аватаркой. Цветовые схемы нельзя выбрать и нет широкой возможности кастомизации, но доступны три размера — большой, маленький и крошечный. Если сложно найти, то можно скопировать код для карточки необходимого размера, заменить оба поля username на актуальный никнейм на платформе Codewars и вставить в свой md-файл.

Большой (large):  
[![codewars](https://www.codewars.com/users/username/badges/large)](https://www.codewars.com/users/username)   

Маленький (small):  
[![codewars](https://www.codewars.com/users/username/badges/small)](https://www.codewars.com/users/username) 

Крошечный (micro):  
[![codewars](https://www.codewars.com/users/username/badges/micro)](https://www.codewars.com/users/username) 

LeetCode Readme Stats — виджет будет полезен любителям порешать задачки на сервисе LeetCode. Карточка выводит данные о количестве решенных задач с распределением по уровню сложности. Есть две темы — светлая и темная. Также у автора имеется инструкция по настройке отслеживания статистики с помощью GitHub Actions. Параметр username= необходимо заменить на актуальный.

Светлая тема:  
[![KnlnKS's LeetCode stats](https://leetcode-stats-six.vercel.app/api?username=KnlnKS)](https://github.com/KnlnKS/leetcode-stats)


Темная тема:  
[![KnlnKS's LeetCode stats](https://leetcode-stats-six.vercel.app/api?username=KnlnKS&theme=dark)](https://github.com/KnlnKS/leetcode-stats)

GitHub Profile Views Counter — небольшой бейдж, выводящий информацию о количестве посетителей профиля. В поиске GitHub можно найти несколько репозиториев с реализацией виджета, но устроены они приблизительно одинаково, поэтому рассмотрим на примере самого популярного. Бейдж можно персонализировать, выбрав цвет из готовых или указать необходимый в шестнадцатеричной системе, на выбор есть три разных дизайна и возможность изменить исходный текст бейджа. Для вставки надо заменить поле your-github-username на соответствующее своему никнейму.

![](https://komarev.com/ghpvc/?username=your-github-username)

Github Readme Activity Graph — виджет с графиком активности на платформе за последний месяц. Для персонализации имеется более 10 готовых тем, поэтому можно спокойно подобрать что-то подходящее под свои нужды. Если ничего не понравится, то у разработчика есть подробная инструкция по кастомизации. Вставка производится уже привычным способом — копируем код, меняем параметр username= на нужный и вставляем в свой md-файл.

[![Ashutosh's github activity graph](https://activity-graph.herokuapp.com/graph?username=Ashutosh00710)](https://github.com/ashutosh00710/github-readme-activity-graph)

GitHub Readme StackOverflow — виджет позволяет делиться статистикой вклада в сообщество StackOverflow. На выбор есть две темы и два размера карточки. Для вставки в свой README профиля надо скопировать код, заменить параметр userID= на свой. С помощью параметра theme= можно выбрать нужную тему — ligh и dark, а с помощью layout= размер — default и compact. Своего профиля на StackOverflow у меня нет, поэтому продемонстрирую все на примере аккаунта автора виджета.

Светлая большая:  
[![Omid Nikrah StackOverflow](https://github-readme-stackoverflow.vercel.app/?userID=6558042)](https://stackoverflow.com/users/6558042/omid-nikrah) 

Темная большая:   
[![Omid Nikrah StackOverflow](https://github-readme-stackoverflow.vercel.app/?userID=6558042&theme=dark)](https://stackoverflow.com/users/6558042/omid-nikrah)  

Светлая маленькая:   
[![Omid Nikrah StackOverflow](https://github-readme-stackoverflow.vercel.app/?userID=6558042&layout=compact)](https://stackoverflow.com/users/6558042/omid-nikrah)

Темная маленькая:   
[![Omid Nikrah StackOverflow](https://github-readme-stackoverflow.vercel.app/?userID=6558042&layout=compact&theme=dark)](https://stackoverflow.com/users/6558042/omid-nikrah)

GitHub Profile Summary Cards — еще одна библиотека карточек, выводит основную информацию по популярным языкам, график активности и общие сведения об аккаунте. Встраивать можно как с помощью Markdown, так и с помощью GitHub Actions. Для выбора доступно ровно десять цветовых схем. В репозитории есть инструкция, но также имеется и веб-приложение для генерации необходимых ссылок. Код для вставки (username= меняем на свой ник, а theme= на название темы из списка):

Карточка профиля: 
![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=daniilshat&theme=solarized_dark)

Статистика языков в коммитах:
![](https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=daniilshat&theme=solarized_dark)

Статистика языков в репозиториях:
![](https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=daniilshat&theme=solarized_dark)

Статистика профиля:
![](https://github-profile-summary-cards.vercel.app/api/cards/stats?username=daniilshat&theme=solarized_dark)

Данные по коммитам за сутки:
![](https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=daniilshat&theme=solarized_dark)

### Skills


<p align="left">
<a href="https://git-scm.com/" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/git-colored.svg" width="36" height="36" alt="Git" /></a>
<a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/javascript-colored.svg" width="36" height="36" alt="JavaScript" /></a>
<a href="https://developer.mozilla.org/en-US/docs/Glossary/HTML5" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/html5-colored.svg" width="36" height="36" alt="HTML5" /></a>
<a href="https://www.w3.org/TR/CSS/#css" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/css3-colored.svg" width="36" height="36" alt="CSS3" /></a>
</p>


### Socials

<p align="left"> <a href="https://www.github.com/MaxSmirnov01" target="_blank" rel="noreferrer"><img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/socials/github-dark.svg" width="32" height="32" /></a></p>

### Badges

<b>My GitHub Stats</b>

<a href="http://www.github.com/MaxSmirnov01"><img src="https://github-readme-stats.vercel.app/api?username=MaxSmirnov01&show_icons=true&hide=&count_private=true&title_color=ef4444&text_color=ffffff&icon_color=0891b2&bg_color=22272e&hide_border=true&show_icons=true" alt="MaxSmirnov01's GitHub stats" /></a>
