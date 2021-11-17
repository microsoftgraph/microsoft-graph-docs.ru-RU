---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 84ba852202f1006389a43975ab011b9177bee2cd
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61034160"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
tenantId := "String"
requestBody.SetTenantId(&tenantId)
options := &msgraphsdk.TenantSearchRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.TenantRelationships().ManagedTenants().TenantGroups().TenantSearch().Post(options)


```