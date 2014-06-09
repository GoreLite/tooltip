# jQuery toolTip
Скрипт, в виде jQuery плагина, для показа простых дизайнерских подсказок на странице.

## Подключение:

Подключаем библиотеку jQuery 1.10.0+
 - Подключаем плагин [js/tool.tip.js](js/tool.tip.js)
 - Подключаем скрипт для нужного нам элемента:
```js
$('document').ready(function(){
    $('.js_this_tooltip').toolTip();
});
```
 - Прописываем стили для .tooltip (есть в примере в [css/styles.css](css/styles.css). (стили выделены /*THIS CSS*/)

## Параметры:

**interval** - интервал в ms перед затуханием подсказки. Возможные значения от: _0_. Значение по умолчанию: _200_;

**duration** - длительность в ms эфекта затухания. Возможные значения от: _0_. Значение по умолчанию: _200_;

**left** - смещение в px по горизонтали относительно центра элемента;

**top** - смещение в px по вертикали относительно верха элемента;

**content** - jQuery объект содержащий контент для тултипа;

**action** - альтернативный event для вызова тултипа Возможные значения: любой тригер для элемента. Нарпимер: _"click"_, _"change"_, _"my_event"_;