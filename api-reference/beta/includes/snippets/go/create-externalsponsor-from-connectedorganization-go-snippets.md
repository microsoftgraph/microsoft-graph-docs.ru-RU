---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 03900e56210b10671e195b34d5fe901cdca6cad2
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719754"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/users/{id}",
}
connectedOrganizationId := "connectedOrganization-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().ConnectedOrganizationsById(&connectedOrganizationId).ExternalSponsors().$ref().Post(requestBody)


```