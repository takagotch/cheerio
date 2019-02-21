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

$('.pear').hasCass('pear')
$('.apple').hasCass('fruit')
$('li').hasCass('pear')

$('.pear').addClass('fruit').html()
$('.apple').addClass('fruit red').html()

$('.pear').removeClass('.pear').html()
$('.apple').addClass('red').removeClass().html()

$('<form><input name="foo" value="bar" checked /><input name="foo" value="qux" checked /></form>').serialize()

$('<form><input name="foo" value="bar" /></form>').serializeArray()

$('#fruits').find('li').length
$('#fruits').find($('.apple')).length

$('.pear').parent().attr('id')

$('.orange').closest()
$('.orange').closest('.apple')
$('.orange').closest('li')
$('.orange').closest('#fruits')
$('.apple').next().hasClass('orange')

$('.apple').nextAll()
$('.apple').nextAll('.orange')

$('.apple').nextUntil('.pear')

$('.orange').prev().hasClass('apple')

$('.pear').prevAll()
$('.pear').prevAll('.orange')

$('.pear').prevUtil('.apple')

$('li').slice(1).eq(0).text()
$('li').slice(1, 2).length

$('.pear').siblings().length
$('.pear').siblings('.orange').length

$('#fruits').children().length
$('#fruits').children('.pear').text()

const fruits = [];

$('li').each(function(i, elem) {
  fruits[i] = $(this).text();
});

fruits.join(', ');


$('li').map(function(i, el) {
  return $(this).text();
}).get().join(' ');


$('li').filter(funciton(i, el) {
  return $(this).attr('class') === 'orange';
}).attr('class');

$('li').not('.apple').length;

$('li').not(function(i, el) {
  return $(this).attr('class') === 'orange';
}).length;

$('ul').has('.pear').attr('id');
$('ul').has($('.paer')[0]).attr('id');

$('#fruits').children().first().text()

$('.pear').sibilings().length

$('.pear').sibilings('.orange').length

$('#fruits').children().length

$('#fruits').chldren('.pear').text()

$('#fruits').contents().length

const fruits = [];
$('li').each(function(i, elem) {
  fruits[i] = $(this).text();
});

fruits.join(', ');

$('li').map(function(i, el) {
  return $(this).text();
}).get().join(' ');

$('li').filter('.orange').attr('class');

$('li').filter(function(i, el) {
  return $(this).attr('class') === 'orange';
}).attr('class')

$('li').not('.apple').length;

$('li').not(function(i, el) {
  return $(this).attr('class') === 'orange';
});

$('ul').has('.pear').attr('id');

$('ul').has($('.pear')[0]).attr('id');

$('#fruits').children().first().text()

$('#fruits').children().last().text()

$('li').eq(0).text()
$('li').eq(-1).text()

$('li').get(0).tagName

$('li').get().length

$('.pear').index()

$('.orange').index('li')

$('.apple').index($('#fruit, li'))

$('li').eq(0).end().length

$('.apple').add('.orange').length

$('li').eq(0).addBack('.orange').length

$('ul').append('<li class="plum">Plum</li>')
$.html()

$('<li class="plum">Plum</li>').appendTo('#fruits')
$.html()

$('<li class="plum">Plum</li>').prependTo('#fruits')
$.html()

$('.apple').after('<li class="plum">Plum</li>')
$.html()

$('<li class="plum">Plum</li>').insertAfter('.apple')
$.html()

$('.apple').before('<li class="plum">Plum</li>')
$.html()

$('<li class="plum">Plum</li>').insertBefore('.apple')
$.html()

$('.pear').remove()
$.html()

const plum = $('<li class="plum">Plum</li>')
$('.pear').replaceWith(plum)
$.html()

$('ul').empty()
$.html()

$('.orange').html()
$('#fruits').html('<li class="mango">Mango</li>').html()

$('.orange').text()
$('ul').text()

const refFruit = $('<div class="red-fruit"></div>')
$('.apple').wrap(redFruit)

const healthy = $('<div class="healthy"></div>')
$('li').wrap(healthy)

$.html()

$.html('.pear')

const $ = cheerio.load('<media:thmbnail url="http://www.foo.com/keyframe.jpg" width="75" height="50" tiem="12:05:01.1.123"/>');

$.xml()

const $ = cheerio.load('This is <em>content</em>.')
$.text()

const $ = cheerio.load('<div>This is <em>content</em></div>')
cheerio.text($('div'))

$('li').toArray()

const moreFruits = $('#fruits').clone()

$.root().append('<ul id="vegatables"></ul>').html();

const $ = cheerio.load('<html><body>Hello, <b>word</b></body></html>');
$.prototype.logHtml = function() {
  console.log(this.html());
};

$('body').logHtml();
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
make setup
make test
```


