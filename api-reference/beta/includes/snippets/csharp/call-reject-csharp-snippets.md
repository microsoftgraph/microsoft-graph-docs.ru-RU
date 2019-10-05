---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fe9a302015230efb5a6547f3ef316d7635a4209d
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402321"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reason = RejectReason.Busy;

await graphClient.App.Calls["57dab8b1-894c-409a-b240-bd8beae78896"]
    .Reject(reason,null)
    .Request()
    .PostAsync();

```