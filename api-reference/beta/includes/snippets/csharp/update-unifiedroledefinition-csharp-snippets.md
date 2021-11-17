---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d1375f72dad7f90b837bd5e34c231aac8e4f3f6dd247bb466bb4ccd1315bfefa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57141678"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleDefinition = new UnifiedRoleDefinition
{
    Description = "Update basic properties of application registrations",
    DisplayName = "Application Registration Support Administrator",
    RolePermissions = new List<UnifiedRolePermission>()
    {
        new UnifiedRolePermission
        {
            AllowedResourceActions = new List<String>()
            {
                "microsoft.directory/applications/basic/read"
            }
        }
    }
};

await graphClient.RoleManagement.Directory.RoleDefinitions["{unifiedRoleDefinition-id}"]
    .Request()
    .UpdateAsync(unifiedRoleDefinition);

```