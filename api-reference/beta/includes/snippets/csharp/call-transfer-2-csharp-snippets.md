---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1c20fb312ebe1607a30e49aebdfa32848a6abb2f
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214532"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transferTarget = new InvitationParticipantInfo
{
    EndpointType = EndpointType.Default,
    Identity = new IdentitySet
    {
        User = new Identity
        {
            Id = "550fae72-d251-43ec-868c-373732c2704f",
            DisplayName = "Heidi Steen",
            AdditionalData = new Dictionary<string, object>()
            {
                {"tenantId", "72f988bf-86f1-41af-91ab-2d7cd011db47"}
            }
        }
    },
    ReplacesCallId = "e5d39592-99bd-4db8-bca8-30fb894ec51d",
    AdditionalData = new Dictionary<string, object>()
    {
        {"languageId", "en-us"},
        {"region", "amer"}
    }
};

await graphClient.Communications.Calls["{call-id}"]
    .Transfer(transferTarget,null)
    .Request()
    .PostAsync();

```