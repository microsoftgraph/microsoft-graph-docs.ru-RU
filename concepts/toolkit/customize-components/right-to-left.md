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
# <a name="display-microsoft-graph-toolkit-components-right-to-left-rtl"></a>Отображение компонентов Microsoft Graph Toolkit справа налево

Компоненты Microsoft Graph Toolkit поддерживают двунаправленные исправления для наборов знаков с написанием справа налево.

Чтобы изменить направление для всех компонентов на странице, задайте для атрибута `dir` в документе `html` или теге `body` значение `rtl`, как показано в следующих примерах.

```html
<body dir="rtl"></body>
```

или

```html
<html dir="rtl"></html>
```

![справа налево](../images/rightToLeft.png)
