---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 84bbbf2618c1c02d81587ca95bef16647843aeea
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "44219295"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var swapShiftsChangeRequests = await graphClient.Teams["{teamId}"].Schedule.SwapShiftsChangeRequests
    .Request()
    .GetAsync();

```