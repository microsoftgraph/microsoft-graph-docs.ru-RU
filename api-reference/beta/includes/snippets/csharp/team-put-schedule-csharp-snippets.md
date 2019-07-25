---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1079684b3063183e2e93b2ceb9b7e899e2d186b8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716970"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schedule = new Schedule
{
    Enabled = true,
    TimeZone = "America/Chicago"
};

await graphClient.Teams["{teamId}"].Schedule
    .Request()
    .PutAsync(schedule);

```