---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8932e944315f5b87dc6f0c1894bc7fc91cf89ce8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956072"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalGroupMember = new ExternalGroupMember
{
    Id = "e5477431-1038-484e-bf69-1dfedb97a110",
    Type = ExternalGroupMemberType.Group,
    IdentitySource = IdentitySourceType.AzureActiveDirectory
};

await graphClient.External.Connections["{externalConnection-id}"].Groups["{externalGroup-id}"].Members
    .Request()
    .AddAsync(externalGroupMember);

```