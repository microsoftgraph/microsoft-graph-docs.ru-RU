---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 173ef06347859d5b0a509e77c722f00f5b0de296
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805285"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var thumbnails = await graphClient.Me.Drive.Items["{driveItem-id}"].Thumbnails
    .Request()
    .GetAsync();

```