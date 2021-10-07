---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b775ff85a00e3bb9f832f62c032495919dd01f73
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214446"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var supportedRegions = await graphClient.DeviceManagement.VirtualEndpoint.SupportedRegions
    .Request()
    .GetAsync();

```