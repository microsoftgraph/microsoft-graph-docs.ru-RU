---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 09d10529ef5e2287a8ee30a30a3b4ec14cf02426
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607709"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var auditLogRoot = await graphClient.AuditLogs
    .Request()
    .GetAsync();

```