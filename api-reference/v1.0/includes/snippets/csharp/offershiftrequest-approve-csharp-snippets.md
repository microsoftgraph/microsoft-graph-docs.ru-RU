---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 92b8feb80e6d75fc41af3cba6a2c594be1328251523e3f846ac14f24713cd619
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57054582"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "Approved!";

await graphClient.Teams["{team-id}"].Schedule.OfferShiftRequests["{offerShiftRequest-id}"]
    .Approve(message)
    .Request()
    .PostAsync();

```