---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a745b63aff4ffea0d90117a4725b885dbcedd12c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65343373"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.B2xUserFlowsRequestBuilderGetQueryParameters{
    Expand: "identityProviders",
}
options := &msgraphsdk.B2xUserFlowsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Identity().B2xUserFlows().GetWithRequestConfigurationAndResponseHandler(options, nil)


```