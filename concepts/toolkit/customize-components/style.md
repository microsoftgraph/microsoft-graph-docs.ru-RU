---
title: Настройка стиля компонентов в microsoft Graph набор средств
description: Используйте настраиваемые свойства CSS для изменения стилей компонентов набор средств Microsoft Graph.
localization_priority: Normal
author: beth-panx
ms.openlocfilehash: 33ccc02f182731d494820976632b7cec2425d077
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663927"
---
# <a name="styling-components-in-the-microsoft-graph-toolkit"></a>Настройка стиля компонентов в microsoft Graph набор средств

Каждый набор средств Microsoft Graph документировать набор настраиваемые [свойства CSS,](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) которые можно использовать для изменения внешний вид и компоненты определенных элементов. Доступные настраиваемые свойства CSS можно найти в каждом из них. Например:

```css
mgt-person {
  --avatar-size: 34px;
}
```

Вы не можете стиль внутренних элементов компонента, если не предоставляете настраиваемого свойства CSS. Эти компоненты находятся в [теневой dom.](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM)

Для большей гибкости рассмотрите возможность использования [пользовательских шаблонов.](./templates.md)

## <a name="apply-themes"></a>Применение тем

Доступны две темы: светлая и темная. По умолчанию все компоненты имеют светлую тему. Чтобы переключиться на темную тему, можно просто применить ее `class="mgt-dark"` к разделу HTML-страницы. К компонентам внутри этого раздела будет применена темная тема. В следующих примерах покажем, как темы будут применяться в зависимости от структуры HTML.

Пример 1. Глобальная тема

```html
<body class="mgt-light">
    <!-- light theme will apply to all components in this section -->
    <header><mgt-login></mgt-login></header>
    <article><mgt-agenda></mgt-agend></article>
    <footer></footer>
</body>
```

Пример 2. Тема отдельного компонента

```html
<mgt-person-card class="mgt-dark"></mgt-person-card>
```

Пример 3. Региональная тема

```html
<div class="mgt-light">
    <header class="mgt-dark">
        // login component will have dark theme
        <mgt-login></mgt-login>
    </header>
    <article>
        // agenda component will have light theme
        <mgt-agenda></mgt-agenda>
    </article>
</div>
```

Пример 4. Настройка CSS с темой

```html
<mgt-people-picker class="mgt-dark custom-class"></mgt-people-picker>
```
```css
mgt-people-picker.custom-class {
    --input-background-color: $custom-background-color;
    --input-border: $custom-input-border;
}
```
