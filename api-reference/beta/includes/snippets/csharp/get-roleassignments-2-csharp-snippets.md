---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ed266c3a55a9b99278ef7ff7bd28c0227dd1f42b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959080"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignments = await graphClient.RoleManagement.Directory.RoleAssignments
    .Request()
    .GetAsync();

```