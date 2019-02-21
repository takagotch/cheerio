### cheerio
---
https://github.com/cheeriojs/cheerio

```js
const cheerio = require('cheerio')
const $ = cheerio.load('<h2 class="title">Hello</h2>')

$('h2.title').text('Hello')
$('h2').addClass('welcome')

$.html()


const cheerio = require('cheerio');
const $ = cheerio.load('<ul id="fruits"></ul>');

const $ = require('cheerio');
$('ul', '<ul id="fruits"></ul>');

const $ = require('cheerio');
$('li', 'ul', '<ul id="fruits"></ul>');

const $ = cheerio.load('<ul id="fruits"></ul>', {
  normalizeWhitespace: true,
  xmlMode: true
});


$('.apple', '#fruits').text()

$('ul .pear').attr('class')

$('li[class=orange]').html()

$('[xml\\:id="main"]');

$('[xml\\:id="main"]');

$('ul').attr('id')

$('.apple').attr('id', 'favorite').html()

$('input[type="checkbox"]').prop('checked')
$('input[type="checkbox"]').prop('checked', true).val()


$('<div data-apple-color="red"></div>').data()
$('<div data-apple-color="red">').data('apple-color')
const apple = $('.apple').data('kind', 'mac')
apple.data('kind')

$('input[type="text"]').val()
$('input[type="text"]').val('test').html()

$('.pear').removeAttr('class').html()






































```

```
{
  withDomLvl1: true,
  normalizeWhitespace: false,
  xmlMode: false,
  decodeEntities: true
}
```

```
```


