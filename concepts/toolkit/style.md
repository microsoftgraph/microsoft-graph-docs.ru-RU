---
title: Стилизация набора средств Microsoft Graph
description: Использование настраиваемых свойств CSS для изменения стилей компонентов
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 41262c4e58973d84f4fec56a6d5abe8dfaf555ef
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243072"
---
# <a name="styling-components-in-the-microsoft-graph-toolkit"></a>Компоненты стилей в наборе инструментов Microsoft Graph

Используйте настраиваемые свойства CSS, чтобы изменить стили компонентов.

Каждый компонент документирует набор настраиваемых [свойств CSS](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) , которые можно использовать для изменения внешнего вида и поведения определенных элементов. Пример:

```css
mgt-person {
  --avatar-size: 34px;
}
```

Внутренние элементы компонента не могут быть применены, если не указать настраиваемое свойство CSS. Дочерние элементы компонента размещаются в [теневой модели DOM](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM).

Для большей гибкости рассмотрите возможность использования [настраиваемых шаблонов](./templates.md).

## <a name="disable-the-shadow-dom-experimental"></a>Отключение теневой модели DOM (экспериментальная версия)

Вы можете отключить теневую модель DOM и внутренние элементы с прямым стилем, используя обычные таблицы стилей браузера, задав для `useShadowDom` свойства static `MgtBaseComponent` класса значение false, прежде чем использовать какие бы то ни было Теги.


```html
<script type="module">
  import { MgtBaseComponent } from './dist/es6/components/baseComponent.js';
   MgtBaseComponent.useShadowRoot = false;
</script>

<script type="module" src="./dist/es6/components/mgt-tasks/mgt-tasks.js"></script>
````
