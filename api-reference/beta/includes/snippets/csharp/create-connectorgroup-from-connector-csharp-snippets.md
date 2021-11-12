---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d57d17572306ed98c6879e611356e1e8b13a666493a1daa44fcd27167c28f8ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57054359"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectorGroup = new ConnectorGroup
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}"}
    }
};

await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].Connectors["{connector-id}"].MemberOf.References
    .Request()
    .AddAsync(connectorGroup);

```