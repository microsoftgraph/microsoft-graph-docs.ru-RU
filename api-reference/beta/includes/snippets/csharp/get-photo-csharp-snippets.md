---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: eac7b203c4b6194a37202b1f709aa94416b60777
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730502"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var profilePhoto = await graphClient.Users["{id|userPrincipalName}"].Photo
    .Request()
    .GetAsync();

```