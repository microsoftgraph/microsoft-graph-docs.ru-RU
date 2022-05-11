---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 53da850d67e3e800b89582cbb1912e33a4a054ba
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65343436"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "emailAddress": "kim@contoso.com",
}
userId := "user-id"
emailAuthenticationMethodId := "emailAuthenticationMethod-id"
graphClient.UsersById(&userId).Authentication().EmailMethodsById(&emailAuthenticationMethodId).Put(requestBody)


```