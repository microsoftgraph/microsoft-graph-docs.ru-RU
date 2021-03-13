---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f4b92be366e588669607b7067fe2caa7a3622bcd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800261"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryAudit = await graphClient.AuditLogs.DirectoryAudits["{directoryAudit-id}"]
    .Request()
    .GetAsync();

```