---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8632a3ca72576a0eb24005cc6389c76e87279c1d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477329"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var registeredDevices = await graphClient.Me.RegisteredDevices
    .Request()
    .GetAsync();

```