---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 051d105d460887a9600af349986cfd987783343a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779656"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agentGroups = await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].AgentGroups
    .Request()
    .Expand("publishedResources")
    .GetAsync();

```