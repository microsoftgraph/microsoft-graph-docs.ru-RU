---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 25679830b69b9849bb19bcbd8abdbdd30c86fa5e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022517"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewNamedLocation()
displayName := "Updated named location without unknown countries and regions"
requestBody.SetDisplayName(&displayName)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.countryNamedLocation",
    "countriesAndRegions":  []String {
        "CA",
        "IN",
    }
    "includeUnknownCountriesAndRegions": false,
}
options := &msgraphsdk.NamedLocationRequestBuilderPatchOptions{
    Body: requestBody,
}
namedLocationId := "namedLocation-id"
graphClient.Identity().ConditionalAccess().NamedLocationsById(&namedLocationId).Patch(options)


```