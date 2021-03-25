---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5fd0df330559ed6d29a0b517ec2d63ef0e496c1d
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201339"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "2441b489-4f12-4882-b039-8f6006bd66da"
};

await graphClient.Policies.FeatureRolloutPolicies["{featureRolloutPolicy-id}"].AppliesTo.References
    .Request()
    .AddAsync(directoryObject);

```