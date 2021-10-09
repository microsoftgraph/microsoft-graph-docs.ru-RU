---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 62f147968434eb53d4c959e204e9ca0c90c85d799f74ef6d94f3b502b65e65ba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57141030"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "2c891f12-928d-4da2-8d83-7d2434a0d8dc"
};

await graphClient.DirectoryRoles["{directoryRole-id}"].Members.References
    .Request()
    .AddAsync(directoryObject);

```