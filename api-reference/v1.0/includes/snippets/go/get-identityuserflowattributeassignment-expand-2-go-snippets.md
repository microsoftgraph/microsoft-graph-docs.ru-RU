---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 58ae6d33529d8aa6159a95f214e801d7c53a451b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65341242"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UserAttributeAssignmentsRequestBuilderGetQueryParameters{
    Expand: "userAttribute",
}
options := &msgraphsdk.UserAttributeAssignmentsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
b2xIdentityUserFlowId := "b2xIdentityUserFlow-id"
result, err := graphClient.Identity().B2xUserFlowsById(&b2xIdentityUserFlowId).UserAttributeAssignments().GetWithRequestConfigurationAndResponseHandler(options, nil)


```