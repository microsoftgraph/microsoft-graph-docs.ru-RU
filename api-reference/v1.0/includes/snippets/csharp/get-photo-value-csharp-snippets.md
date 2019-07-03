---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fcde4b8ff38a06313b1e8adfe9ac0c199bb1d416
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35515270"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var Stream = await graphClient.Users["{id|userPrincipalName}"].Photo.Content
    .Request()
    .GetAsync();

```