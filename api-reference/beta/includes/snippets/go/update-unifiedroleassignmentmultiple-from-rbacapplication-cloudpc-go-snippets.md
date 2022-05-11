---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d8e6acc5f078dd16fe2c5483724f760ff5b5f8aa
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65342400"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUnifiedRoleAssignmentMultiple()
displayName := "NewName"
requestBody.SetDisplayName(&displayName)
description := "A new roleAssignment"
requestBody.SetDescription(&description)
unifiedRoleAssignmentMultipleId := "unifiedRoleAssignmentMultiple-id"
graphClient.RoleManagement().CloudPC().RoleAssignmentsById(&unifiedRoleAssignmentMultipleId).Patch(requestBody)


```