---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 569b386bc2b64385301967838c18dd776f8b473f6e9ad6407cc1e8dd60467580
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57264966"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskDetections = await graphClient.IdentityProtection.RiskDetections
    .Request()
    .Filter("riskEventType eq 'unfamiliarFeatures' or riskLevel eq 'medium'")
    .GetAsync();

```