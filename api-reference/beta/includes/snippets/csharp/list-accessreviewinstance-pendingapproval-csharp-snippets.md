---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 64c6f528a614758f0c49eb79e80c9a3b020f5bb8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222048"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var pendingAccessReviewInstances = await graphClient.Me.PendingAccessReviewInstances
    .Request()
    .Expand("definition")
    .Skip(0)
    .Top(100)
    .GetAsync();

```