---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1703f9e7a8b03c1fdc2f83120c56a3097cac0eee
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684128"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var secureScoreControlProfile = new SecureScoreControlProfile
{
    VendorInformation = new SecurityVendorInformation
    {
        Provider = "SecureScore",
        ProviderVersion = null,
        SubProvider = null,
        Vendor = "Microsoft"
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"assignedTo", ""},
        {"comment", "control is reviewed"},
        {"state", "Reviewed"}
    }
};

await graphClient.Security.SecureScoreControlProfiles["NonOwnerAccess"]
    .Request()
    .UpdateAsync(secureScoreControlProfile);

```