---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 734fd7fdece0c80fa973e2c979bf0c0bb182fc4d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620672"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRole = new DirectoryRole
{
    RoleTemplateId = "roleTemplateId-value"
};

await graphClient.DirectoryRoles
    .Request()
    .AddAsync(directoryRole);

```