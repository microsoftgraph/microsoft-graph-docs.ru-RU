---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 74f317fa3603ccbad5bbe7a37d5a070420033a59
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799275"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directory.FeatureRolloutPolicies["{featureRolloutPolicy-id}"].AppliesTo["{directoryObject-id}"].Reference
    .Request()
    .DeleteAsync();

```