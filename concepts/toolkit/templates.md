---
title: Шаблоны в наборе инструментов Microsoft Graph
description: Используйте настраиваемые шаблоны для изменения содержимого компонента.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: f0648d0ac1348fbadad6cebe8a022f9445fcf1e3
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243069"
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

Поддерживаются следующие функции шаблонов:

- Используйте двойные фигурные скобки`{{expression}}`(), чтобы развернуть выражение. В предыдущем примере `<mgt-person>` `person` объект передает объект, который можно использовать в шаблоне.
- Используйте атрибуты `data-if` и `data-else` для условной визуализации. Условные выражения, `event.attendees.length > 2` такие как, поддерживаются.
- Используйте `data-for` для повторения элемента.
- Используйте параметр `data-type` для указания части компонента, к которой следует применить шаблон. Если не указать тип, шаблон будет применен ко всему компоненту.

Каждый компонент документирует поддерживаемые `data-type` значения и контекст данных, передаваемых по шаблону.

Шаблоны можно использовать в обычном стиле, так как они отображаются вне теневой модели DOM.
