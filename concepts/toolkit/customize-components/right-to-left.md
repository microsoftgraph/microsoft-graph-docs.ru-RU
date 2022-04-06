---
title: Отображение компонентов Microsoft Graph Toolkit справа налево
description: Описание поддержки отображения справа налево для компонентов Microsoft Graph Toolkit.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 189ffe24f42b2302d0992bcc5ca63c9cd7ff6934
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589226"
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
