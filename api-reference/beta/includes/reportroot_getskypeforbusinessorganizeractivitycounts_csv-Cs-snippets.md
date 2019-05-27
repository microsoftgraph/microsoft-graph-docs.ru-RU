---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 412cd0e8241fcc316f4fc7178856e5b7e0b0e526
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34464295"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessOrganizerActivityCounts = await graphClient.Reports.GetSkypeForBusinessOrganizerActivityCounts('D7')
    .Request()
    .GetAsync();

```