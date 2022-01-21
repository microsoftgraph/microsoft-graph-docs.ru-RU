---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e628928fdb0a7dd0ab91da939dcb8631a4315ccc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62138282"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identity = new Microsoft.Graph.ExternalConnectors.Identity
{
    Id = "e811976d-83df-4cbd-8b9b-5215b18aa874",
    Type = Microsoft.Graph.ExternalConnectors.IdentityType.User
};

await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Groups["{externalConnectors.externalGroup-id}"].Members
    .Request()
    .AddAsync(identity);

```