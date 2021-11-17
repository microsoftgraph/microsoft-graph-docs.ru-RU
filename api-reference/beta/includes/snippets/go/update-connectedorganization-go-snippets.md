---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 216f5937195a4ac2b6fed9ec16be77e592c091ca
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61028861"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewConnectedOrganization()
displayName := "Connected organization new name"
requestBody.SetDisplayName(&displayName)
description := "Connected organization new description"
requestBody.SetDescription(&description)
state := "configured"
requestBody.SetState(&state)
options := &msgraphsdk.ConnectedOrganizationRequestBuilderPatchOptions{
    Body: requestBody,
}
connectedOrganizationId := "connectedOrganization-id"
graphClient.IdentityGovernance().EntitlementManagement().ConnectedOrganizationsById(&connectedOrganizationId).Patch(options)


```