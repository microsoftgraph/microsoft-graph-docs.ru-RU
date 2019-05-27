---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b5dadceffe4a144129eface19ad1f73c0022873f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465925"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var functions = await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs["{jobId}"].Schema.Functions()
    .Request()
    .GetAsync();

```