---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cab6b04f3f4f07f2b4f003acb014826021563ce0
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340522"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
sessionId := "22553876-f5ab-4529-bffb-cfe50aa89f87"
requestBody.SetSessionId(&sessionId)
availability := "Available"
requestBody.SetAvailability(&availability)
activity := "Available"
requestBody.SetActivity(&activity)
expirationDuration := "PT1H"
requestBody.SetExpirationDuration(&expirationDuration)
userId := "user-id"
graphClient.UsersById(&userId).Presence().SetPresence(user-id).Post(requestBody)


```