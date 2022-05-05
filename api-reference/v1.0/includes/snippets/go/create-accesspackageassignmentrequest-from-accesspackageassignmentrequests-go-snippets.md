---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d5b4119e90d2787f5a91a9ae3fd9c295300a069a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220692"
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
options := &msgraphsdk.AssignmentRequestsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AssignmentRequests().Post(options)


```