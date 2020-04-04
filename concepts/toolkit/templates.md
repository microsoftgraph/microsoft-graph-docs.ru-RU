---
title: Шаблоны в наборе инструментов Microsoft Graph
description: Используйте настраиваемые шаблоны для изменения содержимого компонента.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 46a1f9b771f358de6099bf1266c10c4c1ebe0cb0
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144263"
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

## <a name="data-context-helper-properties"></a>Вспомогательные свойства контекста данных

Следующие свойства также можно использовать с объектом контекста данных в шаблонах.

| Свойство |  Описание |
| --- | --- | --- |
| $index | Числовой индекс элемента, отображаемого в `data-for`цикле. |
| $parent | Если шаблон отображается в другом шаблоне, это свойство позволяет получить доступ к родительскому контексту данных. |

В приведенном ниже примере показано, как `$index` использовать свойство в цикле обработки данных.

```html
<mgt-person>
  <mgt-person-card>
    <template data-type="additional-details">
      <span data-for="language in languages">
        {{ language.displayName }}<span data-if="$index < languages.length - 1">, </span>
      </span>
    </template>
  </mgt-person-card>
</mgt-person>
```

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

## <a name="templatecontext"></a>темплатеконтекст

Каждый компонент в наборе инструментов Microsoft Graph определяет `templateContext` свойство, которое можно использовать для передачи дополнительных данных в любой шаблон компонента. 

```ts
document.querySelector('mgt-agenda').templateContext = {

  someObject: {},
  formatDate: (date: Date) => { /* format date and return */ },
  someEventHandler: (e) => { /* handleEvent */  }

}
```

Теперь свойства `templateContext` объекта станут доступны для использования в выражениях привязки в шаблоне.

Это может быть полезен во многих сценариях, таких как преобразование данных в привязки или привязывание к событиям. 

### <a name="converters"></a>Типов

Во многих случаях может потребоваться преобразовать данные перед их представлением в шаблоне. Например, вам может потребоваться правильно отформатировать дату перед отображением. В таких случаях может потребоваться использование конвертера шаблонов.

Чтобы использовать конвертер шаблонов, сначала необходимо определить функцию, которая будет выполнять преобразование. Например, вы можете определить функцию для преобразования объекта события в отформатированный диапазон времени.

```ts
document.querySelector('mgt-agenda').templateContext = {

  getTimeRange: (event) => {
    // TODO: format a string from the event object as you wish
    // timeRange = ...

    return timeRange;
  }

}
```

Чтобы использовать конвертер в шаблоне, используйте его, как если бы вы использовали функцию в коде программной части.

```html
<template data-type="event">
  <div>{{ getTimeRange(event) }}</div>
</template>
```

### <a name="event-or-property-binding"></a>Привязка события или свойства

`data-props` Атрибут позволяет добавить прослушиватель событий или задать значение свойства непосредственно в шаблонах. 

```html
<template>
    <button data-props="{{@click: myEvent, myProp: value}}"></button>
</template>
```

Свойства Data/PROPS принимают строку с разделителями запятыми для каждого свойства или обработчика событий, который может потребоваться задать. 

Чтобы добавить обработчик событий, добавьте к имени события префикс `@`. Обработчик события должен быть доступен в `templateContext` элементе.

```ts
document.querySelector('mgt-agenda').templateContext = {

  someEventHandler: (e, context, root) => { /* handleEvent */  }

}
```

```html
<template>
    <button data-props="{{@click: someEventHandler}}"></button>
</template>
```

Аргументы события, контекст данных и корневой элемент шаблона передаются обработчику событий в качестве параметров.


## <a name="template-rendered-event"></a>Событие, отображаемое в шаблоне

В некоторых случаях может потребоваться получить ссылку на визуализированный элемент. Это может быть удобно, если вы хотите самостоятельно обработать отображение контента или изменить отображаемый элемент.

В этом сценарии можно использовать `templateRendered` событие, которое срабатывает после отображения шаблона.

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

  if (templateType === 'event') {
    element.querySelector('.some-button').addEventListener('click', () => {});
  }
});
```

## <a name="styling"></a>Изменении

Шаблоны можно обычно отформатировать с помощью CSS, так как они отображаются вне теневой модели DOM.
