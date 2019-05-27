---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 112694ccc79930dd7af19a4ae708cb44c5065f44
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441236"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveActivityFileCounts = await graphClient.Reports.GetOneDriveActivityFileCounts('D7')
    .Request()
    .GetAsync();

```