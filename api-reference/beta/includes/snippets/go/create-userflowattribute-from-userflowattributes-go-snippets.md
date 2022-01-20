---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b4d3dc79966e229155b1b6adeb1769a6768a6aff
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62138329"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentityUserFlowAttribute()
displayName := "Hobby"
requestBody.SetDisplayName(&displayName)
description := "Your hobby"
requestBody.SetDescription(&description)
dataType := "string"
requestBody.SetDataType(&dataType)
options := &msgraphsdk.UserFlowAttributesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Identity().UserFlowAttributes().Post(options)


```