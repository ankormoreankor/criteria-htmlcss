# Ошибки в консоли

- В консоли в developer tools **не должно** быть ошибок javascript, возникших в ваших файлах. Ошибки возникают, например, когда вы используете переменную, в которой ничего не содержится.

## Правильно

```js
/* Modal */

const modalOverlay = document.querySelectorAll('.modal-overlay');

if (modalOverlay) {
  modalOverlay.addEventListener('click', event => {
    event.preventDefault();
  })
}
```

## Неправильно

```js
/* Modal */

const modalOverlay = document.querySelectorAll('.modal-overlay'); // modalOverlay === undefined

modalOverlay.addEventListener('click', event => {
  event.preventDefault();
})

Uncaught TypeError: Cannot read property 'addEventListener' of null at script.min.js:1
```
