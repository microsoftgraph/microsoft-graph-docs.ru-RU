---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 36a49544f1167f130e9ca133cfb3f2ea09c31840
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461413"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignments = await graphClient.RoleManagement.Directory.RoleAssignments
    .Request()
    .Filter("principalId eq 'a98eb769-7bd4-4489-86f6-ad96e1d58b62'")
    .GetAsync();

```