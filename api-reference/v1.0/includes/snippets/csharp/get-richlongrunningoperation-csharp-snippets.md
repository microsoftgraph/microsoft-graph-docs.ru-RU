---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 254965554b9c8d790bad85ac9cccf10d2303c011
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315839"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var richLongRunningOperation = await graphClient.Sites["{site-id}"].Operations["{richLongRunningOperation-id}"]
    .Request()
    .GetAsync();

```