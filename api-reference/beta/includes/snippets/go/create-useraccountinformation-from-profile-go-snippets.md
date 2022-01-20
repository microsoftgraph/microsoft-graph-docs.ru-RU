---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ff5359fc0f4bbeb53272447f36f6928ad9c779ad
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132905"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUserAccountInformation()
allowedAudiences := "organization"
requestBody.SetAllowedAudiences(&allowedAudiences)
countryCode := "NO"
requestBody.SetCountryCode(&countryCode)
options := &msgraphsdk.AccountRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().Account().Post(options)


```