---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9cb1178f720c27bae34e07b12e41ba217dcd51af
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65342387"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UserAttributeAssignmentsRequestBuilderGetQueryParameters{
}
options := &msgraphsdk.UserAttributeAssignmentsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
result, err := graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).UserAttributeAssignments().GetWithRequestConfigurationAndResponseHandler(options, nil)


```