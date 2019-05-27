---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 64e3eda9e9f75d4ccd2f5770d828837f2493076a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436336"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Drives["{driveId}"]
    .Request()
    .GetAsync();

```