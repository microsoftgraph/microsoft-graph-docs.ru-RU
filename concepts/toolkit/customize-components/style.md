---
title: Стилизация компонентов в microsoft Graph набор средств
description: Используйте пользовательские свойства CSS для изменения стилей компонентов Microsoft Graph набор средств microsoft.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 6d3c565ff2455643d0435936a34add1dda0c6578
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589207"
---
# <a name="styling-components-in-the-microsoft-graph-toolkit"></a>Стилизация компонентов в microsoft Graph набор средств

Каждый Graph набор средств майкрософт документировать набор пользовательских свойств [CSS](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties), которые можно использовать для изменения внешний вид определенных элементов. Доступные настраиваемые свойства CSS можно найти в каждом компонентном docs. Например:

```css
mgt-person {
  --avatar-size: 34px;
}
```

Вы не можете стиль внутренних элементов компонента, если вы не предоставите настраиваемого свойства CSS. Компонентные детские элементы находятся в [теневом dom](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM).

Для большей гибкости рассмотрите возможность использования [пользовательских шаблонов](./templates.md).

## <a name="apply-themes"></a>Применение тем

Доступны две темы : светлая и темная. По умолчанию все компоненты в стиле светлой темы. Чтобы перейти на темную тему, можно просто применить `class="mgt-dark"` к разделу страницы HTML. Компоненты в этом разделе будут иметь темную тему. В следующих примерах покажите, как будут применяться темы в зависимости от структуры HTML.

Пример 1. Глобальная тема

```html
<body class="mgt-light">
    <!-- light theme will apply to all components in this section -->
    <header><mgt-login></mgt-login></header>
    <article><mgt-agenda></mgt-agend></article>
    <footer></footer>
</body>
```

Пример 2. Тема отдельных компонентов

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

Пример 4. Настройка CSS с помощью темы

```html
<mgt-people-picker class="mgt-dark custom-class"></mgt-people-picker>
```
```css
mgt-people-picker.custom-class {
    --input-background-color: $custom-background-color;
    --input-border: $custom-input-border;
}
```
