---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5efe02a18b6441db1738836fcca5833a19c25219
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176494"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissions = await graphClient.Sites["{sitesId}"].Permissions
    .Request()
    .GetAsync();

```