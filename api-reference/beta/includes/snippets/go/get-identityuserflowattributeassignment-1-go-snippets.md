---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3f92916de2db312f7a76fc095b52cc08e7ad79c7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60994907"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.UserAttributeAssignmentsRequestBuilderGetQueryParameters{
}
options := &msgraphsdk.UserAttributeAssignmentsRequestBuilderGetOptions{
    Q: requestParameters,
}
b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
result, err := graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).UserAttributeAssignments().Get(options)


```