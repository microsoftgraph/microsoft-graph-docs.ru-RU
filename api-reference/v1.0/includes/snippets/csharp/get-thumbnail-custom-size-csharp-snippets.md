---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 307b6c087cbd80f4cb76e8c923d3c65e6db34c5f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791726"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("select", "c300x400_Crop")
};

var thumbnails = await graphClient.Me.Drive.Items["{driveItem-id}"].Thumbnails
    .Request( queryOptions )
    .GetAsync();

```