---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 13e9b552365c3bddb84c05ef0c17064286b62aeb
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65343297"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewFieldValueSet()
requestBody.SetAdditionalData(map[string]interface{}{
    "Color": "Fuchsia",
    "Quantity": ,
}
siteId := "site-id"
listId := "list-id"
listItemId := "listItem-id"
graphClient.SitesById(&siteId).ListsById(&listId).ItemsById(&listItemId).Fields().Patch(requestBody)


```