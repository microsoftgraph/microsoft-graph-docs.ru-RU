---
title: Отображение компонентов Microsoft Graph Toolkit справа налево
description: Описание поддержки отображения справа налево для компонентов Microsoft Graph Toolkit.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: fce2d055ae5e859fe65d06edffb99039b8e258bec601f33b3ada8f5b2c671f1e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129554"
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
