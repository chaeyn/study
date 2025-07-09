## input type number 중 spinner 제거

```css
/* 웹킷 기반 브라우저 (Chrome, Safari 등)*/
input::-webkit-outer-spin-button,
input::-webkit-inner-spin-button {
  -webkit-appearance: none;
  margin: 0;
}

/* Firefox */
input[type="number"] {
  appearance: textfield;
  -moz-appearance: textfield;
}
```
