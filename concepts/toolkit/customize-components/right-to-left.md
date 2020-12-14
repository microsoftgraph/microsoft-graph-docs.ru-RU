---
title: Отображение компонентов набор средств Microsoft Graph справа налево (rtl)
description: Описывает поддержку справа налево (rtl) в компонентах набор средств Microsoft Graph.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 224526fb2b514a1821cd66c9b4b3d9aee51328de
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658626"
---
# <a name="display-microsoft-graph-toolkit-components-right-to-left-rtl"></a><span data-ttu-id="e0096-103">Отображение компонентов набор средств Microsoft Graph справа налево (rtl)</span><span class="sxs-lookup"><span data-stu-id="e0096-103">Display Microsoft Graph Toolkit components right-to-left (rtl)</span></span>

<span data-ttu-id="e0096-104">Компоненты microsoft Graph набор средств поддерживают двухнаправленную разметку для языковых сценариев справа налево.</span><span class="sxs-lookup"><span data-stu-id="e0096-104">The Microsoft Graph Toolkit components support bidirectional markup for right-to-left language scripts.</span></span>

<span data-ttu-id="e0096-105">Чтобы изменить направление всех компонентов на странице, установите для атрибута документа или тега следующий атрибут, как показано в `dir` `html` `body` `rtl` следующих примерах.</span><span class="sxs-lookup"><span data-stu-id="e0096-105">To change the direction of all components on the page, set the `dir` attribute on the document `html` or `body` tag to `rtl`, as shown in the following examples.</span></span>

```html
<body dir="rtl"></body>
```

<span data-ttu-id="e0096-106">или</span><span class="sxs-lookup"><span data-stu-id="e0096-106">or</span></span>

```html
<html dir="rtl"></html>
```

![справа налево](../images/rightToLeft.png)
