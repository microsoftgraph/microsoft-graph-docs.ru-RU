---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 05fafbd04ea06ebd4b3be2907787220ccacb90a0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806364"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sharedDriveItem = await graphClient.Shares["{sharedDriveItem-id}"]
    .Request()
    .GetAsync();

```