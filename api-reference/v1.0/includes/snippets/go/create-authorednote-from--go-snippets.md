---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7c56be5e04334258ec0a997896904010d1e2dcfd
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340247"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthoredNote()
content := msgraphsdk.NewItemBody()
requestBody.SetContent(content)
content := "String"
content.SetContent(&content)
contentType := "text"
content.SetContentType(&contentType)
subjectRightsRequestId := "subjectRightsRequest-id"
result, err := graphClient.Privacy().SubjectRightsRequestsById(&subjectRightsRequestId).Notes().Post(requestBody)


```