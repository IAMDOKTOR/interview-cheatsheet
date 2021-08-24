__this__ - это ключевое слово, используемое в JavaScript, которое имеет особое значение, зависящее от контекста в котором оно применяется.
__Контекст__ (а если точнее - контекст выполнения) - это среда, в которой выполняется код JavaScript. 
Под средой я подразумеваю значение this, переменных, объектов и функций, к которым код JavaScript имеет доступ в конкретный момент времени.

Хороший пример на практике. Запустите это в браузере:

```javascript
function test(){
    alert(this);
}
test();      // window
new test();  // test
```

Подробнее:
https://www.youtube.com/watch?v=kb0Af7dzCTs
https://proweb63.ru/help/js/kontekst-vyipolneniya-funkczii-v-javascript
https://habr.com/ru/company/ruvds/blog/422089/
