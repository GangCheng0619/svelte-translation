# Перевод ресурсов по Svelte

> На данный момент еще не известно в каком виде будет реализовываться внедрение локализации на официальных ресурсах, поэтому, в последствии возможны изменения в структуре и подходах данного репозитория 

## Что переводим
* [Учебник](https://v3.svelte.technology/tutorial) по Svelte V3 ([GitHub](https://github.com/sveltejs/svelte/tree/master/site/content/tutorial))
* [Документацию](https://v3.svelte.technology/docs) по Svelte V3 ([GitHub](https://github.com/sveltejs/svelte/tree/api-reference/site/content/docs))
* [Документацию](https://sapper.svelte.technology/guide) по Sapper ([GitHub](https://github.com/sveltejs/sapper.svelte.technology/tree/master/content/guide))
* [Примеры](https://v3.svelte.technology/repl) ([GitHub](https://github.com/sveltejs/svelte/tree/master/site/content/examples))
* [Блог](https://v3.svelte.technology/blog) ([GitHub](https://github.com/sveltejs/svelte/tree/master/site/content/blog))
* Контент сайта [svelte.technology](https://v3.svelte.technology) ([GitHub](https://github.com/sveltejs/svelte/tree/master/site/src))
* Контент сайта [sapper.svelte.technology](https://sapper.svelte.technology) ([GitHub](https://github.com/sveltejs/sapper.svelte.technology/tree/master/src))
* Контент сайта [svelte-native.technology](https://svelte-native.technology) ([GitHub](https://github.com/halfnelson/svelte-native/tree/master/docs_src/content))


## Как внести свой вклад в перевод
* [Перевести](https://github.com/AlexxNB/svelte3-translation-ru/issues/6) еще не переведенную часть какого-либо ресурса, указанного выше.
* Улучшить существующий перевод: исправить орфографическую, пунктуационную или семантическую ошибку, перфразировать неудачно скомпонованое предложение, устранить несоответствия перевода рекомендациям и т.п. Это нужно делать через систему Pull Request в данном репозитории.

## Рекомендации по переводу

>Данные рекомендации по большей части подсмотрены в [сообществе переводчиков React](https://github.com/reactjs/ru.reactjs.org/blob/master/TRANSLATION.md)

* Оформление перевода должно соответствовать оформлению оригинала. 
* Где это к месту, лучше строить предложения в обезличенной форме(без `мы` и `вы`), но не фанатично, т.к. документация старается быть менее официальной. В любом случае `Вы` и его производные пишите с маленькой буквы
* Всегда используйте букву `ё` (это соблюдать с помощью [данного npm-пакета](https://github.com/hcodes/eyo))
* Используйте знак тире `—` — где нужно тире, и знак дефиса `-` — где нужен дефис. Примеры: как-будто, Svelte — это фреймворк.
* Во всех примерах кода необходимо переводить комментарии и весь текст, который относится к UI, т.е. то, что пользователь увидит при запуске такого примера.
* Перевод лексики, терминов и прочего должны быть согласованы со следующим списком в порядке убывания приоритета:
  * Наш [словарь терминов](DICTIONARY.md) Svelte
  *  [Словарь «Веб-стандартов»](https://github.com/web-standards-ru/dictionary)
  * Аналоги в переводах документации других известных UI-фреймворках(Vue, React, Angular)
  * Попытаться найти рускоязычную документацию, доклады или статьи с использованием нужной лексики
  * Придумать перевод самому 
* Избегать черезмерных англицизмов, при условии, что есть общеупотребительные русские аналоги. `Пропсы`, `билд` и подобное не годятся. Но, например, `бандл` не имеет лучшего русского аналога.
* Ссылки на ресурсы (MDN, Wikipedia) должны вести на русскую версию, если есть соответствующий перевод.
* Иностранные имена переводите с указанием оригинального имени в скобках: *Рич Харрис(Rich Harris)*. При этом обязательно проверьте уже существующий перевод имени в [словаре имён «Веб-стандартов»](https://github.com/web-standards-ru/dictionary/blob/master/names.md)
* Ссылки с названием иностранной статьи в переводе должны быть приведены на языке оригинала, после чего содержать в скобках их русскоязычный перевод.
* Исключайте отсылки на пол читателя (см. секцию 3 на [этой странице](http://www.un.org/ru/gender-inclusive-language/guidelines.shtml))
* Названия статей и заголовки пишутся с одной заглавной буквы («Удаление неиспользуемых стилей», а не «Удаление Неиспользуемых Стилей»).

Чтобы избежать кальки, можно брать смысл предложения, а потом перефразировать так, как объясняли бы старшему коллеге. Если предложение звучит нелепо вслух, то его надо переписать.

Небольшие вольности в переводе допускаются, но только если они помогают передать смысл. Перевод не должен быть ни слишком официальным, ни фамильярным. Истина где-то посередине.

## Где смотреть перевод
На данный момент запущены следующие копии официальных сайтов:
- [svelte.alexxnb.ru](https://svelte.alexxnb.ru)
- [sapper.alexxnb.ru](https://sapper.alexxnb.ru)
- [svelte-native.alexxnb.ru](https://svelte-native.alexxnb.ru)

>На этих сайтах можно просматривать переводы естественных условиях. Сайты собираются и деплоятся автоматически при коммитах в данный репозиторий.

[![Build Status](https://drone.alexxnb.ru/api/badges/AlexxNB/svelte3-translation-ru/status.svg)](https://drone.alexxnb.ru/AlexxNB/svelte3-translation-ru)

## Запуск локальной версии сайта

В репозиторий добавлены npm скрипты, которые позволяют забрать с GitHub текущие версию всех необходимых сайтов, применить все изменения из нашего репозитория переводов и запустить копию сайта на своем компьютере, чтобы сразу видеть перевод в естественных условиях.

```bash
git clone git@github.com:AlexxNB/svelte3-translation-ru.git svelte-translation
cd svelte-translation
npm install

# 1. Скачиваем последнюю версию нужного сайта и применяем к нему перевод
npm run update-svelte 
#...или...
npm run update-sapper 
#...или...
npm run update-svelte-native 

# 2. Запускаем сайт на локальной машине
npm run dev-svelte
#...или...
npm run dev-sapper
#...или...
npm run dev-svelte-native
```

Теперь можно открыть запущенный сайт по адресу [http://localhost:3000]() и посмотреть на него со всеми внесенными изменениями на текущий момент.

При изменении файлов перевода, обновите окно браузера и вы должны будете увидеть изменения.
