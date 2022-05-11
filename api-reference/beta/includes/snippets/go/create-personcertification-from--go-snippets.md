---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4a123124fc231c3c41127adc29ed98fdbc49aee0
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340053"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonCertification()
certificationId := "KB-1235466333663322"
requestBody.SetCertificationId(&certificationId)
description := "Blackbelt in Marketing - Brand Management"
requestBody.SetDescription(&description)
displayName := "Marketing Blackbelt - Brand Management"
requestBody.SetDisplayName(&displayName)
thumbnailUrl := "https://iame.io/dfhdfdfd334.jpg"
requestBody.SetThumbnailUrl(&thumbnailUrl)
webUrl := "https://www.iame.io/blackbelt"
requestBody.SetWebUrl(&webUrl)
result, err := graphClient.Me().Profile().Certifications().Post(requestBody)


```