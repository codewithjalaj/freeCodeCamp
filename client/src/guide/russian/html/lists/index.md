---
title: Lists
localeTitle: Списки
---
# Списки

Списки используются для отображения элементов. Существует 3 типа списков.

## Упорядоченные списки

_Упорядоченный список_ используется для описания упорядоченного набора данных. Браузеры обычно отображают упорядоченный список в виде пронумерованного списка. Создайте упорядоченный список, используя `<ol>` .

## Неупорядоченные списки

_Неупорядоченный список_ используется для описания неупорядоченного сбора данных. Браузеры обычно отображают неупорядоченный список в виде маркированного списка. Создайте неупорядоченный список, используя `<ul>` .

## Список элементов

Прямые дети упорядоченных и неупорядоченных списков должны быть элементами списка. Каждый элемент списка заключен в `<li>` . Тег элемента списка может содержать [содержимое потока](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Content_categories#Flow_content) .

## Примеры

Упорядоченный список записывается как

```HTML
<ol> 
  <li>January</li> 
  <li>February</li> 
  <li>March</li> 
 </ol> 
```

и отображается как:

1.  январь
2.  февраль
3.  Март

Неупорядоченный список записывается как

```HTML
<ul> 
  <li>Macintosh</li> 
  <li>Fuji</li> 
  <li>Gala</li> 
 </ul> 
```

и отображается как:

*   макинтош
*   Fuji
*   гала

## Шаблоны стилей

Упорядоченный список может использоваться для множества функций и в нескольких стилях. Поскольку изменение цветных цветов тегов не изменяет цвет самих маркеров, вы можете их стилизовать, сначала удалив традиционные черные пули и вставив их:

Удалить пули:

```CSS
ul { 
  list-style: none; 
  } 
```

Вставьте свой собственный:

```CSS
ul li::before { 
  content: "\2022"; 
  color: orange; 
  display: inline-block; 
  width: 1em; 
  } 
```

Стиль контента добавляет новую маркерную точку, в то время как стиль отображения и ширины создает пространство между пулей и словом. Здесь могут применяться обычные стили шрифтов, если вы хотите сделать пулю более крупной или более смелой.

## Списки описания

Список описаний - это список терминов с описанием каждого термина. Список описаний создается с помощью `<dl>` . Каждый элемент в списке состоит из двух тегов: термин `<dt>` и описание этого термина `<dd>` . Они называются списками определений в HTML 4.

Вот пример списка описания:

```HTML
<dl> 
  <dt>Programming</dt> 
  <dd>The process of writing computer programs.</dd> 
  <dt>freeCodeCamp</dt> 
  <dd>An awesome non-profit organization teaching people how to code.</dd> 
 </dl> 
```

который в итоге выглядит следующим образом:

программирование

Процесс написания компьютерных программ.

freeCodeCamp

Удивительная некоммерческая организация, преподающая людям, как кодировать.

## Дополнительная информация:

*   [Списки HTML на w3schools](https://www.w3schools.com/html/html_lists.asp)