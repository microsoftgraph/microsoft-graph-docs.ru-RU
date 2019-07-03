---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 09d10529ef5e2287a8ee30a30a3b4ec14cf02426
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35473010"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var auditLogRoot = await graphClient.AuditLogs
    .Request()
    .GetAsync();

```