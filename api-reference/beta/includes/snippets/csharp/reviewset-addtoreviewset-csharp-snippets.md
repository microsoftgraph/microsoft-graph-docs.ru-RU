---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6fea69eb2de1537899265acda369ea154d86c590
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772887"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sourceCollection = new Microsoft.Graph.Ediscovery.SourceCollection
{
    Id = "1a9b4145d8f84e39bc45a7f68c5c5119"
};

var additionalData = Microsoft.Graph.Ediscovery.DataCollectionScope.LinkedFiles;

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].ReviewSets["{ediscovery.reviewSet-id}"]
    .AddToReviewSet(sourceCollection,additionalData)
    .Request()
    .PostAsync();

```