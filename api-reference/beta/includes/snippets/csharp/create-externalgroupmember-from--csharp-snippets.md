---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e111ef2ddae3fdee9954dd845c83ca068a5ccd09
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808421"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalGroupMember = new ExternalGroupMember
{
    Id = "1431b9c38ee647f6a",
    Type = ExternalGroupMemberType.Group,
    IdentitySource = IdentitySourceType.External
};

await graphClient.External.Connections["{externalConnection-id}"].Groups["{externalGroup-id}"].Members
    .Request()
    .AddAsync(externalGroupMember);

```