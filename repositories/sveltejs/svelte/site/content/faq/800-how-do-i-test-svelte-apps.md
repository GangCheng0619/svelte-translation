---
question: Как мне тестировать Svelte приложения?
---

Мы рекомендуем постараться отделить логику представления от бизнес-логики. Преобразования данных и управление межкомпонентным состоянием лучше вынести из компонентов Svelte наружу. Тестируйте их как обычный JavaScript код. В компонентах же можно протестировать их логику, и помнить что Svelte имеет свои собственные тесты и тестировать то что вы получаете на выходе компилятора нет необходимости.

Существует несколько подходов для тестирования, которые используют наши пользователи. Но обычно все они основываются на компилировании и монтировании компонента, перед выполнением тестов. То есть, придется создавать отдельный бандл для каждого тестируемого компонента. Вы можете подключиться к этому компоненту посредством JSDOM. Если нужен настоящий браузер, можно использовать Puppeteer или Cypress

Некоторые ресурсы, которые могут помочь с юнит-тестами:

- [Svelte Testing Library](https://testing-library.com/docs/svelte-testing-library/example/)
- [Пример использования uvu вместе с JSDOM](https://github.com/lukeed/uvu/tree/master/examples/svelte)
