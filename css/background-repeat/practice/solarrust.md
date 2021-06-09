---
tags:
  - practice
permalink: false
---

`background-repeat` — свойство простое. Написано повторять — повторяем фон. Написано не повторять — не повторяем.

🛠 Чаще всего в работе встречается значение свойства `background-repeat: no-repeat`.

🛠 Повторение фона может пригодиться, если создаётся паттерн в качестве фона как в [примере](#пример).

🛠 С помощью повторения фона и линейного градиента (`linear-gradient`) можно создавать полосатые фоны.

```html
<div class="element"></div>
```

```css
.element {
  height: 100vh;
  background-image: linear-gradient(
    #49a16c 50px,
    #064236 0
  ); /* Линейный градиент */
  background-size: auto 100px; /* Размер фона: 50 пикселей серая полоска
                                + 50 пикселей чёрная полоска */
  background-repeat: repeat-y; /* Повторяем фон по вертикали */
}
```

<iframe title="Паттерн градиентом" src="../demos/gradient.html"></iframe>