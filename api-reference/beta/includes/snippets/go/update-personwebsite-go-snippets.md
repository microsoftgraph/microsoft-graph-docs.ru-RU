---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 99a75849e39640a371a4874fada40c916e561d4e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65342877"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonWebsite()
description := "Lyn Damer play in the Women's 1st Division (Toppserien) in Norway"
requestBody.SetDescription(&description)
personWebsiteId := "personWebsite-id"
graphClient.Me().Profile().WebsitesById(&personWebsiteId).Patch(requestBody)


```