---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4fff354ded8060c4026c7e2abcafbf09d5299341
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772852"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outputName = "2020-12-06 Contoso investigation export";

var description = "Export for the Contoso investigation";

var exportOptions = Microsoft.Graph.Ediscovery.ExportOptions.OriginalFiles | Microsoft.Graph.Ediscovery.ExportOptions.FileInfo | Microsoft.Graph.Ediscovery.ExportOptions.Tags;

var exportStructure = Microsoft.Graph.Ediscovery.ExportFileStructure.Directory;

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].ReviewSets["{ediscovery.reviewSet-id}"]
    .Export(exportStructure,outputName,description,null,null,exportOptions)
    .Request()
    .PostAsync();

```