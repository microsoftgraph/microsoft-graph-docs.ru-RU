---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d65e79e1aba634997ac4168430f84caa35a5a38a
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66099542"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMessage()
subject := "Annual review"
requestBody.SetSubject(&subject)
body := msgraphsdk.NewItemBody()
requestBody.SetBody(body)
contentType := "HTML"
body.SetContentType(&contentType)
content := "You should be proud!"
body.SetContent(&content)
requestBody.SetToRecipients( []Recipient {
    msgraphsdk.NewRecipient(),
emailAddress := msgraphsdk.NewEmailAddress()
    SetEmailAddress(emailAddress)
address := "rufus@contoso.com"
    emailAddress.SetAddress(&address)
}
requestBody.SetExtensions( []Extension {
    msgraphsdk.NewExtension(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "microsoft.graph.openTypeExtension",
        "extensionName": "Com.Contoso.Referral",
        "companyName": "Wingtip Toys",
        "expirationDate": "2015-12-30T11:00:00.000Z",
        "dealValue": ,
    }
}
result, err := graphClient.Me().Messages().Post(requestBody)


```