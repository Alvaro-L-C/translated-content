---
title: Полифил
slug: Glossary/Polyfill
tags:
  - Глоссарий
  - JavaScript
  - Полифил
original_slug: Glossary/Polifill
---
Полифил — это фрагмент кода (в сети — обычно JavaScript), который позволяет использовать современную функциональность в более старых браузерах, которые не поддерживают ее по умолчанию.

Например, полифил можно использовать, чтобы эмулировать функциональность {{cssxref("text-shadow")}} в IE7 с помощью нативных фильтров браузера, или рем и медиавыражения, динамически меняя стилизацию в нужных случаях с помощью JavaScript, или что-либо еще, что вам потребуется.

Из-за меньшей производительности и ограниченной функциональности нельзя использовать исключительно полифилы. Нативная реализация API быстрее и с ней можно сделать больше, чем с помощью полифила. Например, [полифил Object.create](/ru/docs/Web/JavaScript/Reference/Global_Objects/Object/create#polyfill) может эмулировать только то, что доступно для ненативной реализации Object.create.

В других случаях полифилы нужны, чтобы разрешить ситуации, когда браузеры реализуют одни и те же возможности разными способами. Тогда полифил использует нестандартные возможности конкретного браузера, чтобы в результате определенная функциональность была совместима с действующими стандартами JavaScript. Хотя такое применение полифилов и редкость сейчас, во времена IE6 и Netscape, когда каждый браузер реализовывал JavaScript очень по-разному, оно было широко распространено. [Первая версия JQuery](https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.js) была ранним примером полифила. Она представляла собой компиляцию из обходных путей, специфических для определенных браузеров, которая предоставляла JavaScript-разработчикам единый API для всех браузеров. В то время одной из наибольших проблем было заставить сайт работать на всех устройствах: браузеры настолько существенно различались, что порой код приходилось писать совершенно по-разному и разрабатывать разные пользовательские интерфейсы, исходя из используемого пользователем браузера. Таким образом, у JavaScript-разработчиков был доступ только к очень лимитированному количеству JavaScript API, которые работали более или менее одинаково во всех браузерах. Сейчас использование полифилов для взаимодействия со специфичными для браузера реализациями возможностей менее распространено, так как современные браузеры в большинстве своем имеют большой набор стандартизированных API.

## Узнать больше

### Общая информация

- [Что такое полифил?](http://webknowledge.ru/chto-takoe-polyfill/) (перевод статьи Реми Шарпа, создателя термина «полифил»)
