---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7e9fe7d726ab891fe1f425609636c7325439a41a3ab2693aa342cc943c34bf59
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57394489"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.RoleManagement.DeviceManagement.RoleAssignments["{unifiedRoleAssignmentMultiple-id}"]
    .Request()
    .DeleteAsync();

```