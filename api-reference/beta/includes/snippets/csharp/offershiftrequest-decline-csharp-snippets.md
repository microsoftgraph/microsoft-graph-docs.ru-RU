---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 547fd503603a8d7b3d06cf27ba81df07ba3dcfa4
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "44216996"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "Sorry, you can't offer this shift.";

await graphClient.Teams["{teamId}"].Schedule.OfferShiftRequests["{offerShiftRequestId}"]
    .Decline(message)
    .Request()
    .PostAsync();

```