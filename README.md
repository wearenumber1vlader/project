#	Проект по информатике

>	https://ru.wikipedia.org/wiki/Презентация_(значения)
>>Презентация (способ представления информации) — информационный или рекламный инструмент, позволяющий сообщить нужную информацию об объекте презентации в удобной для получателя форме.
>>>Мультимедийная презентация — набор слайдов и спецэффектов (слайд-шоу), текстовое содержимое презентации, заметки докладчика, а также раздаточный материал для аудитории, хранящиеся в одном файле.

---

#	Презентация будущего	#

### Цели
Создать веб-презентацию
### Задачи

Сравнение

##	Инструкция

###	Для учителей и учеников

###	человек разбирается в коде
####	источники [1]https://github.com/hakimel/reveal.js/blob/master/README.md), [2]http://qaru.site/tags/reveal.js/info
[1](https://github.com/hakimel/reveal.js/blob/master/README.md)файл README.md(с англ. на рус.) инструкция разработчиков, [2](http://qaru.site/tags/reveal.js/info) чужой перевод 2014,[3] мой перевод
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

>> [2]Иерархия разметки должна быть `.reveal > .slides > section`, где `<section>` представляет один слайд и может повторяться бесконечно. Если вы поместите несколько `<section>` внутри другого `<section>`, они будут показаны как вертикальные слайды. Первым из вертикальных слайдов является "корень" остальных (вверху), и он будет включен в горизонтальную последовательность. Например:

> 	<div class="reveal">
		<div class="slides">
			<section>Single Horizontal Slide</section>
			<section>
				<section>Vertical Slide 1</section>
				<section>Vertical Slide 2</section>
			</section>
		</div>
	</div>



