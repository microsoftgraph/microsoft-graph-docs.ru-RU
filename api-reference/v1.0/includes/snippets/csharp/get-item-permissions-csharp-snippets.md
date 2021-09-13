---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 166f858f969633fe6f7bbdc239ebd20f7bf060ba0b427e3388df3ef31f1a8a19
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57429361"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissions = await graphClient.Me.Drive.Items["{driveItem-id}"].Permissions
    .Request()
    .GetAsync();

```