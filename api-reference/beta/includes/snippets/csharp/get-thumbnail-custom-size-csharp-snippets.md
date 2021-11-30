---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 504a7ade6cb453782250243f75d7071646895bc4
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2021
ms.locfileid: "61228380"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("select", "c300x400_crop")
};

var thumbnails = await graphClient.Me.Drive.Items["{driveItem-id}"].Thumbnails
    .Request( queryOptions )
    .GetAsync();

```