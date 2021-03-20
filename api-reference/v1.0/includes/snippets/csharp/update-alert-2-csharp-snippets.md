---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 56c46547881c394322863e65235d1f9f5c58457d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945511"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var alert = new Alert
{
    AssignedTo = "String",
    ClosedDateTime = DateTimeOffset.Parse("String (timestamp)"),
    Comments = new List<String>()
    {
        "String"
    },
    Feedback = AlertFeedback.Unknown,
    Status = AlertStatus.Unknown,
    Tags = new List<String>()
    {
        "String"
    },
    VendorInformation = new SecurityVendorInformation
    {
        Provider = "String",
        Vendor = "String"
    }
};

await graphClient.Security.Alerts["{alert-id}"]
    .Request()
    .Header("Prefer","return=representation")
    .UpdateAsync(alert);

```