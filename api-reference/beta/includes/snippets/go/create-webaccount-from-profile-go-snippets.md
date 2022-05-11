---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dc5c407ab0ca62be115fc726979db437e37332cd
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65341150"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewWebAccount()
description := "My Github contributions!"
requestBody.SetDescription(&description)
userId := "innocenty.popov"
requestBody.SetUserId(&userId)
service := msgraphsdk.NewServiceInformation()
requestBody.SetService(service)
name := "GitHub"
service.SetName(&name)
webUrl := "https://github.com"
service.SetWebUrl(&webUrl)
result, err := graphClient.Me().Profile().WebAccounts().Post(requestBody)


```