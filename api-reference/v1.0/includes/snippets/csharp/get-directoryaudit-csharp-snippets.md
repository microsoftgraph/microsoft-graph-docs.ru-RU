---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6b9bc131b594351a1546a32763bf6f2f79463783
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945205"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryAudit = await graphClient.AuditLogs.DirectoryAudits["{id}"]
    .Request()
    .GetAsync();

```