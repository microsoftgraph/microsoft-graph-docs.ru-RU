---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 78eb796bab4c718e8d3ecbccc31b97c3398f9a38ecb5e0a6cdbab246f9742496
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57260578"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tiIndicator = new TiIndicator
{
    AdditionalInformation = "additionalInformation-after-update",
    Confidence = 42,
    Description = "description-after-update"
};

await graphClient.Security.TiIndicators["{tiIndicator-id}"]
    .Request()
    .Header("Prefer","return=representation")
    .UpdateAsync(tiIndicator);

```