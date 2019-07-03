---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 87af03c3fae97ba3e40abd0c4d41f746e8ef266f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35472675"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var secureScoreControlProfile = new SecureScoreControlProfile
{
    AssignedTo = "",
    Comment = "control is reviewed",
    State = "Reviewed",
    VendorInformation = new SecurityVendorInformation
    {
        Provider = "SecureScore",
        ProviderVersion = null,
        SubProvider = null,
        Vendor = "Microsoft"
    }
};

await graphClient.Security.SecureScoreControlProfiles["NonOwnerAccess"]
    .Request()
    .UpdateAsync(secureScoreControlProfile);

```