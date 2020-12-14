---
title: Шаблоны в microsoft Graph набор средств
description: Используйте настраиваемые шаблоны для изменения содержимого компонента.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 94529f45c95dcfdd56ade2dffc7b4ac7bf48babb
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658592"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a>Шаблоны в microsoft Graph набор средств

Большинство компонентов набор средств Microsoft Graph поддерживают использование настраиваемого шаблона для изменения содержимого компонента.

Все веб-компоненты поддерживают шаблоны на основе `<template>` элемента. Например, чтобы переопредить шаблон компонента, добавьте `<template>` элемент внутри компонента.

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

Если вы используете компоненты Microsoft Graph набор средств React, вы можете использовать React для оформления шаблонов. Подробные сведения [см. в этом наборе инструментов с React.](../get-started/mgt-react.md)

## <a name="data-type"></a>Тип данных

Каждый компонент может иметь несколько частей, которые могут быть шаблоны. Например, в компоненте можно шаблонить отдельные события, отдельные разделы, представление загрузки, без представления `mgt-agenda` данных и т. д. Чтобы указать шаблон, используйте `data-type` атрибут в шаблоне. Например, для шаблона каждого события в `mgt-agenda` , используйте `event` тип данных, как показано.

```html
<mgt-agenda>
  <template data-type="event"> </template>
</mgt-agenda>
```

Если не `data-type` указано, весь компонент будет заменен шаблоном. Вы также можете `data-type="default"` использовать для той же цели.

## <a name="binding-data"></a>Привязка данных

Многие шаблоны позволяют привязыть данные, которые передаются в шаблон в качестве контекста данных. Например, шаблон в компоненте передает объект, который `event` можно использовать непосредственно в `mgt-agenda` `{event}` шаблоне. Чтобы развернуть выражение, `event.subject` например, используйте двойные фигурные скобки.

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

> **Примечание.** Вы также можете развернуть такие объекты, как или они `{{event}}` будут отрисовыты `{{this}}` в качестве строк JSON. Это может быть полезно при разработке шаблонов.

### <a name="change-binding-syntax"></a>Изменение синтаксиса привязки

По умолчанию для расширения выражения используются двойные фигурные скобки ( `{{expression}}` ). Однако можно изменить этот синтаксис для сред, где уже используется синтаксис двойных фигурных скобок. Например, в следующем примере используются двойные квадратные скобки ( `[[expression]]` ).

```ts
import { TemplateHelper } from '@microsoft/mgt';

TemplateHelper.setBindingSyntax('[[', ']]');
```

## <a name="data-context-helper-properties"></a>Свойства помощника для контекста данных

Следующие свойства также можно использовать с объектом контекста данных в шаблонах.

| Свойство | Описание                                                                                                    |
|----------|----------------------------------------------------------------------------------------------------------------|
| $index   | Числовая индексация элемента, отрисовываемого при циклической отрисовки. `data-for`                                     |
| $parent  | Если шаблон отрисовки в другом шаблоне, это свойство позволяет получить доступ к контексту родительских данных. |

В следующем примере показано, как `$index` использовать свойство в цикле для данных.

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

## <a name="conditional-rendering"></a>Условная отрисовка

Отрисовка элементов может потребоваться только в том случае, если условие имеет истинное или ложное на основе контекста данных. Атрибуты `data-if` и выражения могут оцениваться и отрисовки, `data-else` только если засвеяется true или false.

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

## <a name="looping"></a>Циклы

В некоторых случаях объект контекста данных содержит цикл, и вам потребуется зациклить данные. В этом сценарии используйте `data-for` атрибут.

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

В сценариях, где необходимо преобразовывать данные в привязках, привязывать к событиям или просто использовать внешние данные в привязках шаблонов, шаблоны поддерживают привязку к контексту внешних данных. Добавить дополнительный контекст шаблона можно двумя способами:

1. Непосредственно на компоненте.

    Каждый компонент определяет свойство, которое можно использовать для передачи дополнительных данных любому `templateContext` шаблону в компоненте.

    ```ts
    document.querySelector('mgt-agenda').templateContext = {

      someObject: {},
      formatDate: (date: Date) => { /* format date and return */ },
      someEventHandler: (e) => { /* handleEvent */  }

    }
    ```

    Теперь свойства в объекте будут доступны для использования в выражениях привязки `templateContext` в шаблоне.

2. Глобально для всех компонентов.

    Класс предоставляет объект для добавления данных или функций, которые должны быть глобально `TemplateHelper` `globalContext` доступны для всех компонентов.

    ```ts
    import { TemplateHelper } from '@microsoft/mgt';

    TemplateHelper.globalContext.someObject = {};
    TemplateHelper.globalContext.formatDate = (date: Date) => { /* format date and return */ };
    TemplateHelper.globalContext.someEventHandler = (e) => { /* handleEvent */  }
    ```



### <a name="converters"></a>Конвертеры

Во многих случаях может потребоваться преобразовать данные, прежде чем их представить в шаблоне. Например, может потребоваться правильно отформаировать дату перед ее отрисовка. В таких случаях может потребоваться использовать конвертер шаблонов.

Чтобы использовать конвертер шаблонов, сначала необходимо определить функцию, которая будет делать преобразование. Например, можно определить функцию для преобразования объекта события в форматированный диапазон времени.

```ts
document.querySelector('mgt-agenda').templateContext = {

  getTimeRange: (event) => {
    // TODO: format a string from the event object as you wish
    // timeRange = ...

    return timeRange;
  }

}
```

Чтобы использовать преобразователь в шаблоне, используйте его так, как если бы вы использовали функцию в коде кода.

```html
<template data-type="event">
  <div>{{ getTimeRange(event) }}</div>
</template>
```

### <a name="event-or-property-binding"></a>Привязка события или свойства

Этот атрибут позволяет добавить прослушиватель событий или установить значение `data-props` свойства непосредственно в шаблонах.

```html
<template>
    <button data-props="{{@click: myEvent, myProp: value}}"></button>
</template>
```

Реквизиты данных принимают строку с запятой для каждого свойства или обработника событий, которые вы можете захотим установить.

Чтобы добавить обработтель событий, добавьте к имени события префикс `@` . Обработник событий должен быть доступен в `templateContext` элементе.

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


## <a name="template-rendered-event"></a>Событие отображения шаблона

В некоторых случаях может потребоваться получить ссылку на элемент отрисовки. Это может быть полезно, если вы хотите самостоятельно обрабатывать отрисовку содержимого или хотите изменить элемент отрисовки.

В этом сценарии можно использовать событие, которое сгореет после отрисовки `templateRendered` шаблона.

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.addEventListener('templateRendered', (e) => { });
```

Сведения о событии будут содержать ссылку на элемент, который отрисовки, объект контекста данных и тип шаблона.

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

Шаблоны можно стиль обычно с помощью CSS, так как они отрисовки за пределами теневой dom.
