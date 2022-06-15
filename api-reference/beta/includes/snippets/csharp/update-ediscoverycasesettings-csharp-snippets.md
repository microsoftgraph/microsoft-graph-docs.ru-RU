---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a98601a7cc7cdb7716c310965ff77c1e3ee2a296
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092444"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoveryCaseSettings = new Microsoft.Graph.Security.EdiscoveryCaseSettings
{
    RedundancyDetection = new RedundancyDetectionSettings
    {
    },
    TopicModeling = new TopicModelingSettings
    {
    },
    Ocr = new OcrSettings
    {
    }
};

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Settings
    .Request()
    .UpdateAsync(ediscoveryCaseSettings);

```