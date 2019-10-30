#	Проект по информатике

>	https://ru.wikipedia.org/wiki/Презентация_(значения)
>>Презентация (способ представления информации) — информационный или рекламный инструмент, позволяющий сообщить нужную информацию об объекте презентации в удобной для получателя форме.
>>>Мультимедийная презентация — набор слайдов и спецэффектов (слайд-шоу), текстовое содержимое презентации, заметки докладчика, а также раздаточный материал для аудитории, хранящиеся в одном файле.

## Как это работает
>	Развитие веб-технологий уже давно увело нас от сайтов-документов, где единственным развлечением было ходить по синим ссылкам. Сегодня с помощью HTML, CSS и JavaScript можно не только сделать приложение, но и даже написать интерфейс для полноценной операционной системы, как в случае с Firefox OS.
Как это применить к презентациям? Ты просто пишешь презентацию в HTML, Маркдауне или даже в формате YAML, запускаешь результат в браузере, выходишь в полноэкранный режим и начинаешь свой рассказ. Такие презентации прекрасно слушаются пультов, позволяют анимировать переходы, вставлять картинки и видео, помимо привычного текста и списков.
https://habr.com/ru/company/xakep/blog/185490/

---

#	Презентация будущего	#

### Цели
Создать веб-презентацию
### Задачи
1.	Сравнить способы создания презентанций

## Сравнение


###	Reveal.js

>	Reveal.js — движок презентаций Хаким Эль-Хаттаба, привлекающий своей простотой, 3D-эффектами и специальным онлайн-сервисом для создания презентаций rvl.io.
>> 	рабочая ссылка https://slides.com/
>
>	Дело было в 2011 году, шведский разработчик Хаким Эль-Хаттаб готовил доклад про SVG к местной конференции и так заигрался с 3D-возможностями в CSS, что построил на них простой движок для презентаций. Назвал он его тоже просто: CSS 3D Slideshow. Трехмерные эффекты и двухуровневая навигация настолько полюбились публике, что движок получил развитие под новым названием Reveal.js. Проект обзавелся не только новым именем, но и другими серьезными вещами, вроде документации, поддержки сообщества и репозитория на GitHub, однако не утратил изначальной простоты: темное поле с высветом посередине, белые буквы по центру и впечатляющие 3D-пролеты. Но Хаким не успокоился на этом и сделал целый сервис, который позволяет создавать презентации на движке Reveal.js и хранить их на сайте.
Одна из интересных особенностей этого движка — возможность писать содержимое слайдов в формате Маркдаун. Конвертацией этого текста в HTML на лету занимается специальный скрипт.https://habr.com/ru/company/xakep/blog/185490/ Впервые опубликовано в журнале «Хакер» от 05/2013.
Автор: Вадим Макеев, евангелист компании Opera, pepelsbey

### Impress.js

>	Impress.js — движок презентаций Бартека Шопки с 3D-пролетами, развивающий подход Prezi «поверхность с идеями» с помощью открытых технологий прямо в браузере.
Презентация движка impress.js Бартека Шопки начинается провокационно: вам демонстрируют скучные белые слайды и задают вопрос «А не устали ли вы от однообразных презентаций?» — один слайд, второй, третий… и тут, при переходе на четвертый, все меняется. Вы оказываетесь на большой поверхности, где хитрым образом разбросаны все идеи, составляющие презентацию, и переход к следующей сопровождается замысловатым пролетом, от которого захватывает дух.
Появившийся в 2011 году движок impress.js развивает подход «поверхности с идеями» сервиса для создания презентаций Prezi и соединяет ее c новыми доступными в браузерах технологиями, используя анимацию и 3D-возможности CSS, как Reveal.js. И если Prezi — это коммерческий сервис на закрытой платформе Flash, то impress.js — это открытая библиотека, работающая прямо в браузере без плагинов и тарифных планов.
https://habr.com/ru/company/xakep/blog/185490/ Впервые опубликовано в журнале «Хакер» от 05/2013.
Автор: Вадим Макеев, евангелист компании Opera, pepelsbey


### "Раньше было лучше"
##	Инструкция

###	Для учителей и учеников

###	человек разбирается в коде
####	источники [1]https://github.com/hakimel/reveal.js/blob/master/README.md), [2]http://qaru.site/tags/reveal.js/info
[1](https://github.com/hakimel/reveal.js/blob/master/README.md)файл README.md(с англ. на рус.) инструкция разработчиков, [2](http://qaru.site/tags/reveal.js/info) чужой перевод 2014,[3] мой перевод, комментарии
- [Редактор Интернета](#Для учителей и учеников)
- [Installation](#installation)
  - [Basic setup](#basic-setup)
  - [Full setup](#full-setup)
  - [Folder Structure](#folder-structure)
- [Инструкции](#Инструкции)
  - [Разметка](#Разметка)
  - [Markdown](#markdown)
  - [Element Attributes](#element-attributes)
  - [Slide Attributes](#slide-attributes)
- [Configuration](#configuration)
- [Presentation Size](#presentation-size)
- [Dependencies](#dependencies)
- [Ready Event](#ready-event)
- [Auto-sliding](#auto-sliding)
- [Keyboard Bindings](#keyboard-bindings)
- [Vertical Slide Navigation](#vertical-slide-navigation)
- [Touch Navigation](#touch-navigation)
- [Lazy Loading](#lazy-loading)
- [API](#api)
  - [Slide Changed Event](#slide-changed-event)
  - [Presentation State](#presentation-state)
  - [Slide States](#slide-states)
  - [Slide Backgrounds](#slide-backgrounds)
  - [Parallax Background](#parallax-background)
  - [Slide Transitions](#slide-transitions)
  - [Internal links](#internal-links)
  - [Fragments](#fragments)
  - [Fragment events](#fragment-events)
  - [Code syntax highlighting](#code-syntax-highlighting)
  - [Slide number](#slide-number)
  - [Overview mode](#overview-mode)
  - [Fullscreen mode](#fullscreen-mode)
  - [Embedded media](#embedded-media)
  - [Stretching elements](#stretching-elements)
  - [Resize Event](#resize-event)
  - [postMessage API](#postmessage-api)
- [PDF Export](#pdf-export)
- [Theming](#theming)
- [Speaker Notes](#speaker-notes)
  - [Share and Print Speaker Notes](#share-and-print-speaker-notes)
  - [Server Side Speaker Notes](#server-side-speaker-notes)
- [Plugins](#plugins)
- [Multiplexing](#multiplexing)
  - [Master presentation](#master-presentation)
  - [Client presentation](#client-presentation)
  - [Socket.io server](#socketio-server)
- [MathJax](#mathjax)
- [License](#license)
## Инструкции
### Разметка
[1]Here's a barebones example of a fully working reveal.js presentation:
```html
<html>
	<head>
		<link rel="stylesheet" href="css/reveal.css">
		<link rel="stylesheet" href="css/theme/white.css">
	</head>
	<body>
		<div class="reveal">
			<div class="slides">
				<section>Slide 1</section>
				<section>Slide 2</section>
			</div>
		</div>
		<script src="js/reveal.js"></script>
		<script>
			Reveal.initialize();
		</script>
	</body>
</html>
```
</html>

>> [2]Иерархия разметки должна быть , где `<section>` представляет один слайд и может повторяться бесконечно. Если вы поместите несколько `<section>` внутри другого `<section>`, они будут показаны как вертикальные слайды. Первым из вертикальных слайдов является "корень" остальных (вверху), и он будет включен в горизонтальную последовательность. Например:


