---
tags:
  - practice
permalink: false
---

Для динамики всегда используйте `transform` и `opacity`, избегайте изменения остальных свойств (типа `left`, `top`, `margin`, `background` и т. д.).

Таким образом вы дадите браузеру возможность оптимизировать отрисовку, отчего страница станет отзывчивее.

Для анимаций, которые необходимо перерисовывать на каждый фрейм, используйте `requestAnimationFrame` и его [полифил](https://gist.github.com/paulirish/1579671).

Это сделает тяжёлую анимацию менее рваной.