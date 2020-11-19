---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d217254ea6d30d4ce7f13287b8b282516ae2ac2f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49221943"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var decisions = await graphClient.Me.PendingAccessReviewInstances["70a68410-67f3-4d4c-b946-6989e050be19"].Decisions
    .Request()
    .Skip(0)
    .Top(100)
    .GetAsync();

```