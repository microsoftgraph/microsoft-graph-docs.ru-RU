---
title: Отображение компонентов Microsoft Graph Toolkit справа налево
description: Описание поддержки отображения справа налево для компонентов Microsoft Graph Toolkit.
ms.localizationpriority: medium
author: vogtn
ms.openlocfilehash: a573016903f68883dc733e596de2519640a6acac
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129574"
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
