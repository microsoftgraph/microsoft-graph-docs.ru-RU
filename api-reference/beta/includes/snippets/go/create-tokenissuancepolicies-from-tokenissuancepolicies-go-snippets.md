---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 255c35aae1008b494bf5d639c6bfa1c034493baf
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65343175"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTokenIssuancePolicy()
requestBody.SetDefinition( []String {
    "definition-value",
}
displayName := "displayName-value"
requestBody.SetDisplayName(&displayName)
isOrganizationDefault := true
requestBody.SetIsOrganizationDefault(&isOrganizationDefault)
result, err := graphClient.Policies().TokenIssuancePolicies().Post(requestBody)


```