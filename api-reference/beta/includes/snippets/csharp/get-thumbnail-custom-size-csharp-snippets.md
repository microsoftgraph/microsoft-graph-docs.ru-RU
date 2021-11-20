---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4389e0f704dbd14318c7d9ec12cfe6daa4743783e0e36e77842aeb8ff32b020d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57320528"
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