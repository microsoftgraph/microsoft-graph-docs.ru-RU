---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b9d8f2c6601cf1e93dacb75ee149db41bd22f0d3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65339972"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUnifiedRoleDefinition()
description := "Update basic properties of application registrations"
requestBody.SetDescription(&description)
displayName := "Application Registration Support Administrator"
requestBody.SetDisplayName(&displayName)
requestBody.SetRolePermissions( []UnifiedRolePermission {
    msgraphsdk.NewUnifiedRolePermission(),
    SetAdditionalData(map[string]interface{}{
        "allowedResourceActions":  []String {
            "microsoft.directory/applications/basic/read",
        }
    }
}
unifiedRoleDefinitionId := "unifiedRoleDefinition-id"
graphClient.RoleManagement().Directory().RoleDefinitionsById(&unifiedRoleDefinitionId).Patch(requestBody)


```