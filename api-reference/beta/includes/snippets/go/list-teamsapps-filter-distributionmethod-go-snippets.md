---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b926c3cbc27512772d6efb3ad8eaf1936342c822
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65314411"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.TeamsAppsRequestBuilderGetQueryParameters{
    Filter: "distributionMethod%20eq%20'organization'",
}
options := &msgraphsdk.TeamsAppsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.AppCatalogs().TeamsApps().GetWithRequestConfigurationAndResponseHandler(options, nil)


```