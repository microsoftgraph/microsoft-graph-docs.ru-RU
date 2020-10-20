---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7c43be70b95b2beaa466ecb7e8664380b16dead5
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601607"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryAudits = await graphClient.AuditLogs.DirectoryAudits
    .Request()
    .GetAsync();

```