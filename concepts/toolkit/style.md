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
# <a name="styling-components-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="c98eb-103">Компоненты стилей в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c98eb-103">Styling components in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="c98eb-104">Используйте настраиваемые свойства CSS, чтобы изменить стили компонентов.</span><span class="sxs-lookup"><span data-stu-id="c98eb-104">Use CSS custom properties to modify the component styles.</span></span>

<span data-ttu-id="c98eb-105">Каждый компонент документирует набор [настраиваемых свойств CSS](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) , которые можно использовать для изменения внешнего вида и поведения определенных элементов.</span><span class="sxs-lookup"><span data-stu-id="c98eb-105">Each component documents a set of [CSS custom properties](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) that you can use to change the look and feel of certain elements.</span></span> <span data-ttu-id="c98eb-106">Например:</span><span class="sxs-lookup"><span data-stu-id="c98eb-106">For example:</span></span>

```css
mgt-person {
  --avatar-size: 34px;
}
```

<span data-ttu-id="c98eb-107">Внутренние элементы компонента не могут быть применены, если не указать настраиваемое свойство CSS.</span><span class="sxs-lookup"><span data-stu-id="c98eb-107">You can't style internal elements of a component unless you provide a CSS custom property.</span></span> <span data-ttu-id="c98eb-108">Дочерние элементы компонента размещаются в [теневой модели DOM](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM).</span><span class="sxs-lookup"><span data-stu-id="c98eb-108">The component child elements are hosted in a [shadow dom](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM).</span></span>

<span data-ttu-id="c98eb-109">Для большей гибкости рассмотрите возможность использования [настраиваемых шаблонов](./templates.md).</span><span class="sxs-lookup"><span data-stu-id="c98eb-109">For more flexibility, consider using [custom templates](./templates.md).</span></span>

## <a name="disable-the-shadow-dom-experimental"></a><span data-ttu-id="c98eb-110">Отключение теневой модели DOM (экспериментальная версия)</span><span class="sxs-lookup"><span data-stu-id="c98eb-110">Disable the shadow dom (experimental)</span></span>

<span data-ttu-id="c98eb-111">Вы можете отключить теневую модель DOM и внутренние элементы с прямым стилем, используя обычные таблицы стилей браузера, задав для `useShadowDom` свойства static `MgtBaseComponent` класса значение false, прежде чем использовать какие бы то ни было Теги.</span><span class="sxs-lookup"><span data-stu-id="c98eb-111">You can disable the shadow dom, and directly style internal elements using normal browser stylesheets, by setting the static property `useShadowDom` of the `MgtBaseComponent` class to false before using any MGT tags.</span></span>


```html
<script type="module">
  import { MgtBaseComponent } from './dist/es6/components/baseComponent.js';
   MgtBaseComponent.useShadowRoot = false;
</script>

<script type="module" src="./dist/es6/components/mgt-tasks/mgt-tasks.js"></script>
````
