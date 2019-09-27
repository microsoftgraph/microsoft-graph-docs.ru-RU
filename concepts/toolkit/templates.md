---
title: Шаблоны в наборе инструментов Microsoft Graph
description: Используйте настраиваемые шаблоны для изменения содержимого компонента.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b9ef4b9422d84886fa4df76618b6cdf14def2378
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275712"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a>Шаблоны в наборе инструментов Microsoft Graph

Используйте настраиваемые шаблоны для изменения содержимого компонента.

Все веб-компоненты поддерживают шаблоны на основе `<template>` элемента. Например, чтобы переопределить шаблон компонента, добавьте `<template>` элемент в компонент.

```html
<mgt-agenda>
  <template data-type="event">
      <div>{{event.subject}}</div>
      <div data-for='attendee in event.attendees'>
          <mgt-person person-query="{{attendee.emailAddress.name}}">
            <template>
              <div data-if="person.image">
                <img src="{{person.image}}" />
              </div>
              <div data-else>
                {{person.displayName}}
              </div>
            </template>
          </mgt-person>
      </div>
  </template>
</mgt-agenda>
```

## <a name="data-type"></a>Тип данных

Каждый компонент может иметь несколько частей, которые можно использовать в шаблоне. Например, в `mgt-agenda` компоненте можно зашаблонировать отдельные события, заголовки отдельных разделов, Загрузка представления, без представления данных и т. д. Чтобы указать шаблон, используйте `data-type` атрибут для шаблона. Например, чтобы указать шаблон для каждого события в `mgt-agenda`, используйте тип `event` данных, как показано ниже.

```html
<mgt-agenda>
  <template data-type="event"> </template>
</mgt-agenda>
```

Если этот `data-type` параметр не указан, весь компонент будет заменен на шаблон. Вы также можете использовать `data-type="default"` для этой цели.

## <a name="binding-data"></a>Привязка данных

Многие шаблоны позволяют привязать данные, которые передаются шаблону в качестве контекста данных. Например, `event` шаблон в `mgt-agenda` компоненте передает `{event}` объект, который можно использовать непосредственно в шаблоне. Чтобы развернуть выражение, например `event.subject`, используйте двойные фигурные скобки.

```html
<template data-type="event">
  <div>{{event.subject}}</div>
</template>
```

Этот формат также можно использовать в атрибутах:

```html
<template data-type="event">
  <a href="{{ event.onlineMeetingUrl }}" />
</template>
```

> **Примечание:** Вы также можете развернуть такие объекты, `{{event}}` как, и они будут отображаться как строки JSON. Это может быть удобно при разработке шаблонов.

## <a name="conditional-rendering"></a>Условная визуализация

Вы можете отображать элементы только в том случае, если условие имеет значение true или false в зависимости от контекста данных. Атрибуты `data-if` и `data-else` могут оценивать выражение и отображать только значения true и false.

```html
<mgt-person person-query="john doe">
  <template>
    <div data-if="person.image">
      <img src="{{ person.image }}" />
    </div>
    <div data-else>
      {{ person.displayName }}
    </div>
  </template>
</mgt-person>
```

## <a name="looping"></a>Циклов

Существуют случаи, когда объект контекста данных содержит цикл, и вам потребуется перебрать данные. В этом случае используйте `data-for` атрибут.

```html
<template data-type="event">
  <ul>
    <li data-for='attendee in event.attendees'>
      {{ attendee.displayName }}
    </li>
  </ul>
</template>
```

## <a name="converters"></a>Типов

Во многих случаях может потребоваться преобразовать данные перед их представлением в шаблоне. Например, вам может потребоваться правильно отформатировать дату перед отображением. В таких случаях может потребоваться использование конвертера шаблонов.

Чтобы использовать конвертер шаблонов, сначала необходимо определить функцию, которая будет выполнять преобразование. Например, вы можете определить функцию для форматирования даты.

```ts
getTimeRange(event) {
  // TODO: format a string from the event object as you wish
  // timeRange = ...

  return timeRange;
}
```

Затем определите новый конвертер для элемента и присвойте ему имя по своему усмотрению.

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.templateConverters["myConverter"] = getTimeRange;
```

Чтобы использовать конвертер в шаблоне, используйте тройные фигурные скобки.

```html
<template data-type="event">
  <div>{{{ myConverter(event) }}}</div>
</template>
```

Вы также можете использовать встроенные функции, не определяя Конвертер шаблонов.

```html
<template data-type="event">
  <div>{{{ event.subject.toUpperCase() }}}</div>
</template>
```

## <a name="template-rendered-event"></a>Событие, отображаемое в шаблоне

В некоторых случаях может потребоваться получить ссылку на визуализированный элемент. Это может быть удобно для добавления прослушивателей событий в элементы шаблона. В этом случае вы можете использовать `templateRendered` событие.

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.addEventListener('templateRendered', (e) => { });
```

Сведения о событии будут содержать ссылку на отображаемый элемент, объект контекста данных и тип шаблона.

```ts
agenda.addEventListener('templateRendered', (e) => { 
  let templateType = e.detail.templateType;
  let dataContext = e.detail.context;
  let element = e.detail.element;

  if (type === 'event') {
    element.querySelector('.some-button').addEventListener('click', () => {});
  }
});
```

## <a name="styling"></a>Изменении

Шаблоны можно обычно отформатировать с помощью CSS, так как они отображаются вне теневой модели DOM.
