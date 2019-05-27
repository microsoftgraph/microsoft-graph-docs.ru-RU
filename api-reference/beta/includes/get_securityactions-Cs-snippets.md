---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8966cc8cff64e7e98537747be28a760e40df5ea1
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446297"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityActions = await graphClient.Security.SecurityActions
    .Request()
    .GetAsync();

```