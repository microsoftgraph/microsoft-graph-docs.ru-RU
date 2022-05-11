---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6ce5581612fc390be30c1a85764f7f16ce5aadf7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65341296"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}",
}
deviceId := "device-id"
directoryObjectId := "directoryObject-id"
graphClient.DevicesById(&deviceId).RegisteredOwnersById(&directoryObjectId).Post(requestBody)


```