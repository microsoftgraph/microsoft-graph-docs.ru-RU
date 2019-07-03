---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 82d8a96c21aae5396d2e8339429f7e57bae8cf09
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35514724"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permission = await graphClient.Me.Drive.Items["{item-id}"].Permissions["{perm-id}"]
    .Request()
    .GetAsync();

```