---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 692a702d0b02aff4ed704838ced7f8aa62290648
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096607"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEmailAuthenticationMethod()
emailAddress := "kim@contoso.com"
requestBody.SetEmailAddress(&emailAddress)
options := &msgraphsdk.EmailMethodsRequestBuilderPostOptions{
    Body: requestBody,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).Authentication().EmailMethods().Post(options)


```