---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9bbecb0f4780ce6c3766094ea2a01403b9af7c7b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65343238"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageAssignmentRequest()
requestType := "userAdd"
requestBody.SetRequestType(&requestType)
assignment := msgraphsdk.NewAccessPackageAssignment()
requestBody.SetAssignment(assignment)
assignment.SetAdditionalData(map[string]interface{}{
    "accessPackageId": "d7be3253-b9c6-4fab-adef-30d30de8da2b",
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AssignmentRequests().Post(requestBody)


```