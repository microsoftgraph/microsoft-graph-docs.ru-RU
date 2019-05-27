---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1f01c5c796f23d3c1787aa1de246614d305678c8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477309"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var registeredOwners = await graphClient.Devices["{id}"].RegisteredOwners
    .Request()
    .GetAsync();

```