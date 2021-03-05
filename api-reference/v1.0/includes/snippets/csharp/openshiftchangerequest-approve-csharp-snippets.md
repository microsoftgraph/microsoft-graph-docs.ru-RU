---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7cbed4da940a668e6d58e0f21b6a4364dea78924
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448181"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "message-value";

await graphClient.Teams["{id}"].Schedule.OpenShiftChangeRequests["{openShiftChangeRequestId}"]
    .Approve(message)
    .Request()
    .PostAsync();

```