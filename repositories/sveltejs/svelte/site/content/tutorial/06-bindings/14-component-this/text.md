---
title: Привязка к экземплярам компонентов
---

Так же, как вы можете привязываться к элементам DOM, вы можете привязываться к самим экземплярам компонентов. Например, мы можем привязать экземпляр `<InputField>` к переменной `field` так же, как и при привязке элементов DOM

```html
<InputField bind:this={field} />
```

Теперь мы можем программно взаимодействовать с этим компонентом, используя `field`.

```html
<button on:click="{() => field.focus()}">
    Focus field
</button>
```

> Обратите внимание, что мы не можем сделать `{field.focus}`, так как поле не определено при первом отображении кнопки и выдает ошибку.