---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6711947e4381592b2a671a11c203f17a953e73fa99338690e1d792f9dad6c188
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57263070"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "message-value";

await graphClient.Teams["{team-id}"].Schedule.TimeOffRequests["{timeOffRequest-id}"]
    .Decline(message)
    .Request()
    .PostAsync();

```