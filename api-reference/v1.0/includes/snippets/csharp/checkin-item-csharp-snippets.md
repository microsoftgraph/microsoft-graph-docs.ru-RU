---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fd4f3fda3f3c8854e11c4cd29ba05edc1fa186de
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809117"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "Updating the latest guidelines";

await graphClient.Drives["{drive-id}"].Items["{driveItem-id}"]
    .Checkin(null,comment)
    .Request()
    .PostAsync();

```