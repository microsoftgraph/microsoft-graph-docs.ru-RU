---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6ff22b0ce1b0726e5e0da3c55a1355c281ddabbb
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65341320"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/groups/{groupId}",
}
printerShareId := "printerShare-id"
groupId := "group-id"
graphClient.Print().SharesById(&printerShareId).AllowedGroupsById(&groupId).Post(requestBody)


```