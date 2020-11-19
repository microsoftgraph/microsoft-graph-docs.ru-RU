---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cb9b1ce27391e7b794439e43a933246613aefa63
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49350505"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.AccessReviews.Definitions["04e5c3b2-9db2-40d3-a204-128f4956ae8e"].Instances["70463350-742e-4909-bfa5-bc23447bd002"]
    .SendReminder()
    .Request()
    .PostAsync();

```