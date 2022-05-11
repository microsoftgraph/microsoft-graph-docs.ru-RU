---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 413286d114a183b336ad1a334b3ce58430706a2d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65342175"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/odata/groups('1a9db3ab-0acf-4808-99ae-e8ed581cb2e0')",
}
mobilityManagementPolicyId := "mobilityManagementPolicy-id"
groupId := "group-id"
graphClient.Policies().MobileAppManagementPoliciesById(&mobilityManagementPolicyId).IncludedGroupsById(&groupId).Post(requestBody)


```