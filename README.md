# Ripple effect

## Установка

```bash
npm install @qpokychuk/ripple --save
```

## Основа использования

```js
import ripple from '@qpokychuk/ripple';
import '@qpokychuk/ripple/index.css';

ripple.init()
ripple.attach('.btn')
ripple.attach('.waved')

ripple.deAttach('.btn-text') // example class="btn btn-text"

ripple.destroy()

```

## Пользовательские стили

Вы можете редактировать эффект с помощью css

```css
.ripple{
    background: radial-gradient(rgba(255, 255, 255, 0.1) 0,
        rgba(255, 255, 255, 0.2) 40%,
        rgba(255, 255, 255, 0.2) calc(60% - 10px),
        rgba(255, 255, 255, 0.2) 60%,
        rgba(0, 0, 0, 0) calc(60% + 10px));
}
```



| Функция | Аргумент | Описание |
|---|---|---|
| `init`     |                   | Вешает слушатели событий |
| `attach`   | `selector:string` | Добавляет эффект для селектора  |
| `deAttach` | `selector:string` | Убирает эффект для селектора |
| `destroy`  |                   | Убирает слушатели событий |

[Поддержать автора](https://www.tinkoff.ru/rm/yuferov.sergey18/NC17C11734)