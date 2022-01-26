---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2d82a782619e4199396f62b339eb0535fdf1ff0f
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2022
ms.locfileid: "62227586"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "view";

var password = "ThisIsMyPrivatePassword";

var scope = "anonymous";

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .CreateLink(type,scope,null,password,null,null)
    .Request()
    .PostAsync();

```