---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b7af6a52452417dcf48dc0d7c0182535f8d559c291502ef9130324f7ca71b93f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57309715"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.PrivilegedAccess["{privilegedAccess-id}"].RoleAssignmentRequests["{governanceRoleAssignmentRequest-id}"]
    .UpdateRequest(null,null,null,null)
    .Request()
    .PostAsync();

```