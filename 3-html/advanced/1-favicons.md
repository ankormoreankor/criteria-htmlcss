# Фавиконки

К каждой странице **должны** быть подключены иконки с помощью `<link rel="icon">` с указанием размера иконки. Иконки **не должны** быть в формате ICO.

- Фавиконки в размерах 16 × 16 и 32 × 32 в формате PNG.
- Тач-иконка 152×152 в формате PNG.

## Правильно

```html
<link rel="icon" type="image/png" sizes="16x16" href="16.png">
<link rel="icon" type="image/png" sizes="32x32" href="32.png">
<link rel="apple-touch-icon" href="152.png">
```

## Неправильно

```html
<link rel="icon" href="favicon.ico">
```
