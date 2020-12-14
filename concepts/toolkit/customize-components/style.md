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
# <a name="styling-components-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="0e0d2-103">Настройка стиля компонентов в microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="0e0d2-103">Styling components in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="0e0d2-104">Каждый набор средств Microsoft Graph документировать набор настраиваемые [свойства CSS,](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) которые можно использовать для изменения внешний вид и компоненты определенных элементов.</span><span class="sxs-lookup"><span data-stu-id="0e0d2-104">Each Microsoft Graph Toolkit component documents a set of [CSS custom properties](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) that you can use to change the look and feel of certain elements.</span></span> <span data-ttu-id="0e0d2-105">Доступные настраиваемые свойства CSS можно найти в каждом из них. Например:</span><span class="sxs-lookup"><span data-stu-id="0e0d2-105">You can find the available custom CSS properties in each component docs. For example:</span></span>

```css
mgt-person {
  --avatar-size: 34px;
}
```

<span data-ttu-id="0e0d2-106">Вы не можете стиль внутренних элементов компонента, если не предоставляете настраиваемого свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="0e0d2-106">You can't style internal elements of a component unless you provide a CSS custom property.</span></span> <span data-ttu-id="0e0d2-107">Эти компоненты находятся в [теневой dom.](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM)</span><span class="sxs-lookup"><span data-stu-id="0e0d2-107">The component child elements are hosted in a [shadow dom](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM).</span></span>

<span data-ttu-id="0e0d2-108">Для большей гибкости рассмотрите возможность использования [пользовательских шаблонов.](./templates.md)</span><span class="sxs-lookup"><span data-stu-id="0e0d2-108">For more flexibility, consider using [custom templates](./templates.md).</span></span>

## <a name="apply-themes"></a><span data-ttu-id="0e0d2-109">Применение тем</span><span class="sxs-lookup"><span data-stu-id="0e0d2-109">Apply themes</span></span>

<span data-ttu-id="0e0d2-110">Доступны две темы: светлая и темная.</span><span class="sxs-lookup"><span data-stu-id="0e0d2-110">Two themes are available - light and dark.</span></span> <span data-ttu-id="0e0d2-111">По умолчанию все компоненты имеют светлую тему.</span><span class="sxs-lookup"><span data-stu-id="0e0d2-111">By default, all components are styled with light theme.</span></span> <span data-ttu-id="0e0d2-112">Чтобы переключиться на темную тему, можно просто применить ее `class="mgt-dark"` к разделу HTML-страницы.</span><span class="sxs-lookup"><span data-stu-id="0e0d2-112">To switch to dark theme, you can simply apply `class="mgt-dark"` to the  section of your HTML page.</span></span> <span data-ttu-id="0e0d2-113">К компонентам внутри этого раздела будет применена темная тема.</span><span class="sxs-lookup"><span data-stu-id="0e0d2-113">The components inside that section will have dark theme applied.</span></span> <span data-ttu-id="0e0d2-114">В следующих примерах покажем, как темы будут применяться в зависимости от структуры HTML.</span><span class="sxs-lookup"><span data-stu-id="0e0d2-114">The following examples show how themes will apply based on how you structure your HTML.</span></span>

<span data-ttu-id="0e0d2-115">Пример 1. Глобальная тема</span><span class="sxs-lookup"><span data-stu-id="0e0d2-115">Example 1: Global theme</span></span>

```html
<body class="mgt-light">
    <!-- light theme will apply to all components in this section -->
    <header><mgt-login></mgt-login></header>
    <article><mgt-agenda></mgt-agend></article>
    <footer></footer>
</body>
```

<span data-ttu-id="0e0d2-116">Пример 2. Тема отдельного компонента</span><span class="sxs-lookup"><span data-stu-id="0e0d2-116">Example 2: Individual component theme</span></span>

```html
<mgt-person-card class="mgt-dark"></mgt-person-card>
```

<span data-ttu-id="0e0d2-117">Пример 3. Региональная тема</span><span class="sxs-lookup"><span data-stu-id="0e0d2-117">Example 3: Regional theme</span></span>

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

<span data-ttu-id="0e0d2-118">Пример 4. Настройка CSS с темой</span><span class="sxs-lookup"><span data-stu-id="0e0d2-118">Example 4: Customize CSS with theme</span></span>

```html
<mgt-people-picker class="mgt-dark custom-class"></mgt-people-picker>
```
```css
mgt-people-picker.custom-class {
    --input-background-color: $custom-background-color;
    --input-border: $custom-input-border;
}
```
