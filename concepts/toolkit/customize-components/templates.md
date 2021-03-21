---
title: Шаблоны в microsoft Graph набор средств
description: Используйте настраиваемые шаблоны для изменения контента компонента.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 1db3f315cd89932481a0a2325eecae19592d9276
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963283"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a>Шаблоны в microsoft Graph набор средств

Большинство компонентов Microsoft Graph набор средств поддерживают использование настраиваемого шаблона для изменения содержимого компонента.

Все веб-компоненты поддерживают шаблоны на основе `<template>` элемента. Например, чтобы переопредить шаблон компонента, добавьте элемент `<template>` внутри компонента.

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

Если вы используете компоненты Microsoft Graph набор средств React, вы можете использовать React для оформления шаблонов. Подробные сведения [см. в материале Use the toolkit with React.](../get-started/mgt-react.md)

## <a name="data-type"></a>Тип данных

Каждый компонент может иметь несколько частей, которые можно шаблонить. Например, в компоненте можно шаблонить отдельные события, отдельные заглавные разделы, представление загрузки, отсутствие представления `mgt-agenda` данных и т. д. Чтобы указать шаблон, используйте `data-type` атрибут в шаблоне. Например, для шаблона каждого события `mgt-agenda` в , используйте тип `event` данных, как показано.

```html
<mgt-agenda>
  <template data-type="event"> </template>
</mgt-agenda>
```

Если `data-type` нет, весь компонент будет заменен шаблоном. Вы также можете использовать `data-type="default"` для той же цели.

## <a name="binding-data"></a>Привязка данных

Многие шаблоны позволяют связывать данные, которые передаются в шаблон в качестве контекста данных. Например, шаблон в компоненте передает объект, который можно `event` `mgt-agenda` использовать непосредственно в `{event}` шаблоне. Чтобы расширить выражение, `event.subject` например, используйте двойные фигурные скобки.

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

> **Примечание:** Вы также можете расширить объекты, такие как или и они `{{event}}` `{{this}}` будут отрисовки в качестве строк JSON. Это может быть полезно при разработке шаблонов.

### <a name="change-binding-syntax"></a>Изменение синтаксиса привязки

По умолчанию для расширения выражения используются двойные фигурные скобки ( `{{expression}}` ). Однако этот синтаксис можно изменить для сред, в которых уже используется синтаксис двойной фигурной скобки. Например, в следующем примере используются двойные квадратные скобки ( `[[expression]]` ).

```ts
import { TemplateHelper } from '@microsoft/mgt';

TemplateHelper.setBindingSyntax('[[', ']]');
```

## <a name="data-context-helper-properties"></a>Свойства помощника контекста данных

Следующие свойства также можно использовать с объектом контекста данных в шаблонах.

| Свойство | Описание                                                                                                    |
|----------|----------------------------------------------------------------------------------------------------------------|
| $index   | Числовая индексация элемента, отрисовываемого при цикле `data-for` с .                                     |
| $parent  | Если шаблон отрисовка внутри другого шаблона, это свойство позволяет получить доступ к родительскому контексту данных. |

В следующем примере показано, как использовать `$index` свойство в цикле data-for.

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

### <a name="this"></a>{{this}}

Чтобы помочь отламыть контекст данных, можно использовать в `this` выражениях привязки. Простейшая форма заключается в добавлении `{{this}}` в любом месте шаблона.

```html
<template data-type="event">
  <div>
    {{this}}
  </div>
</template>
```

Так как JavaScript можно использовать в выражениях привязки, у вас также есть доступ к объекту, который позволяет использовать (или любой другой [`console`](https://developer.mozilla.org/docs/Web/API/Console) `console.log(this)` API) в `console` шаблонах.

```html
<template data-type="event">
  <div>
    {{console.log(this)}}
  </div>
</template>
```

## <a name="conditional-rendering"></a>Условное отрисовка

Отрисовка элементов может потребоваться только в том случае, если условие является верным или ложным на основе контекста данных. Атрибуты `data-if` `data-else` и выражения могут оцениваться и отрисовки только в том случае, если они верны или ложны.

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

## <a name="looping"></a>Цикл

Будут случаи, когда объект контекста данных содержит цикл, и вам потребуется цикл данных. Для этого сценария используйте `data-for` атрибут.

```html
<template data-type="event">
  <ul>
    <li data-for='attendee in event.attendees'>
      {{ attendee.displayName }}
    </li>
  </ul>
</template>
```

## <a name="template-context"></a>Контекст шаблона

В сценариях, в которых необходимо преобразовать данные в привязки, привязать к событиям или просто использовать внешние данные в привязках шаблонов, шаблоны поддерживают привязку к внешнему контексту данных. Дополнительный контекст шаблона можно добавить двумя способами:

1. Непосредственно на компоненте.

    Каждый компонент определяет свойство, которое можно использовать для передачи дополнительных данных любому `templateContext` шаблону в компоненте.

    ```ts
    document.querySelector('mgt-agenda').templateContext = {

      someObject: {},
      formatDate: (date: Date) => { /* format date and return */ },
      someEventHandler: (e) => { /* handleEvent */  }

    }
    ```

    Свойства объекта теперь будут доступны для использования в выражениях `templateContext` привязки в шаблоне.

2. Глобально для всех компонентов.

    Класс предоставляет объекту возможность добавлять данные или функции, которые должны быть глобально `TemplateHelper` `globalContext` доступны для всех компонентов.

    ```ts
    import { TemplateHelper } from '@microsoft/mgt';

    TemplateHelper.globalContext.someObject = {};
    TemplateHelper.globalContext.formatDate = (date: Date) => { /* format date and return */ };
    TemplateHelper.globalContext.someEventHandler = (e) => { /* handleEvent */  }
    ```



### <a name="converters"></a>Преобразователи

Во многих случаях перед тем, как представить их в шаблоне, может потребоваться преобразовать данные. Например, перед отрисовки может потребоваться правильное форматирование даты. В этих случаях может потребоваться использовать конвертер шаблонов.

Чтобы использовать конвертер шаблонов, сначала необходимо определить функцию, которая будет делать преобразование. Например, можно определить функцию преобразования объекта события в отформатированный диапазон времени.

```ts
document.querySelector('mgt-agenda').templateContext = {

  getTimeRange: (event) => {
    // TODO: format a string from the event object as you wish
    // timeRange = ...

    return timeRange;
  }

}
```

Чтобы использовать конвертер в шаблоне, используйте его так, как если бы вы использовали функцию в коде позади.

```html
<template data-type="event">
  <div>{{ getTimeRange(event) }}</div>
</template>
```

### <a name="event-or-property-binding"></a>Привязка события или свойства

Атрибут позволяет добавлять слушателя событий или устанавливать значение `data-props` свойства непосредственно в шаблонах.

```html
<template>
    <button data-props="{{@click: myEvent, myProp: value}}"></button>
</template>
```

Реквизит данных принимает запятую, делимитированную строку для каждого свойства или обработника событий, которые может потребоваться установить.

Чтобы добавить обработник событий, пристройте имя события с `@` помощью . Обработник событий должен быть доступен в `templateContext` элементе.

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

Args события, контекст данных и корневой элемент шаблона передаются обработчиве событий в качестве параметров.


## <a name="template-rendered-event"></a>Событие отрисовки шаблона

В некоторых случаях может потребоваться получить ссылку на отрисовка элемента. Это может быть полезно, если вы хотите самостоятельно обрабатывать отрисовку контента или изменить отрисовку элемента.

В этом сценарии можно использовать событие, которое загорелось после отрисовки `templateRendered` шаблона.

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.addEventListener('templateRendered', (e) => { });
```

Сведения о событии будут содержать ссылку на отрисовка элемента, объект контекста данных и тип шаблона.

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

## <a name="styling"></a>Стиль

Шаблоны можно в обычном режиме стилизовать с помощью CSS, так как они отрисовыются за пределами теневого дома.
