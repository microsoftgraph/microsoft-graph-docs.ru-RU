---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b741feeb3e804fe643601be0b1d2337d23ec95a22397f3a0e900c876ed556a25
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57143557"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sourceCollection = new Microsoft.Graph.Ediscovery.SourceCollection
{
    DisplayName = "Quarterly Financials search"
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections["{ediscovery.sourceCollection-id}"]
    .Request()
    .UpdateAsync(sourceCollection);

```