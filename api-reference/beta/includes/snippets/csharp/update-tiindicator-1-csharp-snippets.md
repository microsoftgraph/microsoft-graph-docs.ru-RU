---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b124edd202ca641b82aea05f194500de07197b76a74ebf20159e6c8ebfd40292
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57315012"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tiIndicator = new TiIndicator
{
    Description = "description-updated"
};

await graphClient.Security.TiIndicators["{tiIndicator-id}"]
    .Request()
    .UpdateAsync(tiIndicator);

```