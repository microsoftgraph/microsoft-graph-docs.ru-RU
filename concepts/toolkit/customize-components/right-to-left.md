---
title: Отображение компонентов Microsoft Graph Toolkit справа налево
description: Описание поддержки отображения справа налево для компонентов Microsoft Graph Toolkit.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 224526fb2b514a1821cd66c9b4b3d9aee51328de
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658626"
---
# <a name="display-microsoft-graph-toolkit-components-right-to-left-rtl"></a><span data-ttu-id="9ea28-103">Отображение компонентов Microsoft Graph Toolkit справа налево</span><span class="sxs-lookup"><span data-stu-id="9ea28-103">Display Microsoft Graph Toolkit components right-to-left (rtl)</span></span>

<span data-ttu-id="9ea28-104">Компоненты Microsoft Graph Toolkit поддерживают двунаправленные исправления для наборов знаков с написанием справа налево.</span><span class="sxs-lookup"><span data-stu-id="9ea28-104">The Microsoft Graph Toolkit components support bidirectional markup for right-to-left language scripts.</span></span>

<span data-ttu-id="9ea28-105">Чтобы изменить направление для всех компонентов на странице, задайте для атрибута `dir` в документе `html` или теге `body` значение `rtl`, как показано в следующих примерах.</span><span class="sxs-lookup"><span data-stu-id="9ea28-105">To change the direction of all components on the page, set the `dir` attribute on the document `html` or `body` tag to `rtl`, as shown in the following examples.</span></span>

```html
<body dir="rtl"></body>
```

<span data-ttu-id="9ea28-106">или</span><span class="sxs-lookup"><span data-stu-id="9ea28-106">or</span></span>

```html
<html dir="rtl"></html>
```

![справа налево](../images/rightToLeft.png)
