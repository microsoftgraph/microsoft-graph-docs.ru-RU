---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4f08fc624dee66f6c8137dc7d6974c4348057277
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629305"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSubscriptions = await graphClient.DeviceManagement.VirtualEndpoint.Snapshots
    .GetSubscriptions()
    .Request()
    .GetAsync();

```