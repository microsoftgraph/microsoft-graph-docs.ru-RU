---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3bada9522e05456be2a3b74b21cd79c29bf32fb8
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961407"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrants = await graphClient.Groups["{group-id}"].PermissionGrants
    .Request()
    .GetAsync();

```