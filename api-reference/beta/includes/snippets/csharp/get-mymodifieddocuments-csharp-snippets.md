---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: eaf16f187ed1beee1f353efd8c547d523e303097
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332719"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var used = await graphClient.Me.Insights.Used
    .Request()
    .GetAsync();

```