---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e28a54eddbab4c8595fbff370f66b6b7e051a2d7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65341024"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewNamedLocation()
displayName := "Named location with unknown countries and regions"
requestBody.SetDisplayName(&displayName)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.countryNamedLocation",
    "countriesAndRegions":  []String {
        "US",
        "GB",
    }
    "includeUnknownCountriesAndRegions": true,
}
result, err := graphClient.Identity().ConditionalAccess().NamedLocations().Post(requestBody)


```