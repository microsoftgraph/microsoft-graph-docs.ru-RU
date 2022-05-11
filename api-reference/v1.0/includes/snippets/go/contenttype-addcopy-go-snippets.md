---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4cc1190ccd18caddcc13a6f332ac0f2b7c49a158
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65342076"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewContentTypeRequestBody()
contentType := "https://graph.microsoft.com/v1.0/sites/{site-id}/contentTypes/0x0101"
requestBody.SetContentType(&contentType)
siteId := "site-id"
listId := "list-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).ContentTypes().AddCopy(site-id, list-id).Post(requestBody)


```