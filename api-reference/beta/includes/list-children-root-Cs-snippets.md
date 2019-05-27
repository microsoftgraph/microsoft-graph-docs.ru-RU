---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f90a569405e1aad5554e85bd469f26f4c1f26fa2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444407"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children = await graphClient.Me.Drive.Root.Children
    .Request()
    .GetAsync();

```