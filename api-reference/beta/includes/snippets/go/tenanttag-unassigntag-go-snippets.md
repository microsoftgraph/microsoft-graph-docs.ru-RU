---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b330d7fadf4c2b78f5641eab4a0cd9bdf28a8685
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103441"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetTenantIds( []String {
    "String",
}
options := &msgraphsdk.UnassignTagRequestBuilderPostOptions{
    Body: requestBody,
}
tenantTagId := "tenantTag-id"
result, err := graphClient.TenantRelationships().ManagedTenants().TenantTagsById(&tenantTagId).UnassignTag().Post(options)


```