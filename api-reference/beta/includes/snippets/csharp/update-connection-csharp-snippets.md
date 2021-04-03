---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2bf54783a1512f084e61a694d75a69b3022cf740
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573724"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalConnection = new Microsoft.Graph.ExternalConnectors.ExternalConnection
{
    Name = "Contoso HR Service Tickets",
    Description = "Connection to index HR service tickets"
};

await graphClient.Connections["{externalConnectors.externalConnection-id}"]
    .Request()
    .UpdateAsync(externalConnection);

```