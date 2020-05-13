---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d445039ee440477a8b0c68dcf368973d17182030
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "44219298"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "message-value";

await graphClient.Teams["{teamId}"].Schedule.SwapShiftsChangeRequests["{swapShiftChangeRequestId}"]
    .Approve(message)
    .Request()
    .PostAsync();

```